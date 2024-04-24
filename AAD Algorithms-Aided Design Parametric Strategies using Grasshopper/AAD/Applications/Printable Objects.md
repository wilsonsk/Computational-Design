---
up:
  - "[[Digital Fabrication]]"
related:
  - "[[Surfaces]]"
  - "[[Meshes]]"
  - "[[Nurbs Curves]]"
date created: 2024-04-18
---
# Printable Objects
The translation of digital ideas to physical objects using 3D printing is currently viable for small scale objects.
	The definition of such an object is constantly changing, as 3D printing advances are constantly changing the qualifications of "small", enabling lager objects to be printed. 

Producing digital models for 3D printing is not technically different from producing conventional 3D models.
	Similar to all forms of fabrication, when using additive fabrication, consideration of real world characteristics are essential, in this case the consideration of selected printing technology as a constraint.
		The **way** **geometry** is **defined** to create a **printable model** is **crucial**.
## Main Characteristics of a Printable 3D Model/Object
Printable 3D models differ from 3D models developed for visualization and rendering.
Printable objects must consider:
- Geometric digital modeling criteria.
- The specifics of the machine that will "rea" and the print the generated code.
- The characteristics of the materials used for printing.
### Geometric Characteristics of a Printable 3D Model/Object
#### 1. Closed (watertight) Geometries
Each surface or mesh has an **"inside"** face and an ***outside face***.
A 3D object is considered **watertight** and printable if **no inner faces are visible.**
![[Pasted image 20240418235112.png|500]]
#### 2. Manifold Mesh
Only manifold models will be printed correctly. 
##### Manifold:
Refers to geometries that do no contain edges shared by more than two faces (*Image A* has no shared/overlapped face between the mesh boxes). 
	Non-manifold geometries can be the result of inconsistent models (*image B*) or overlapped objects (*image C*), issues that are problematic when printing. 
		*For information on [[SubD Surface Patterns#Cull Adjacent (i.e. overlapping) Faces|how to remove overlapped faces from a mesh.]]*
![[Pasted image 20240418235508.png|600]]
#### 3. [[Meshes#Orientable Meshes|Orientable]] Mesh (correct normals)
The geometry must be an orientable mesh.
	I.e. The 3D model must be composed of face normals which follow the same directional logic.
#### 4. No Self-Intersections
The geometry must not be composed of intersecting non-Booleaned (i.e. unioned, etc.) objects. 
### Other Printable 3D Model/Object Constraints
A printable object must also meet the following constraints:
#### 1. Maximum Size (i.e. build volume)
Models/Objects cannot be larger than a maximum size of the **build volume** or **tray size**.
	These values are measured in the $xyz$ dimensions and are specific to each printer.
Models that are larger than build volume can be divided into smaller parts, which can be assembled into the larger component. 
#### 2. Minimum Wall-Thickness
Refers to the minimum thickness that can be printed by a given printer.
The value varies based on the specific technology and material.
	*For example, [[Digital Fabrication#Selective Laser Sintering (SLS)|SLS]] printers can have a minimum wall-thickness of 0.7mm using plastic materials.*
An [[Surfaces#Untrimmed Surface|untrimmed surface]] contains no thickness and is not [[#1. Closed (watertight) Geometries|watertight]]. 
	Therefore is not [[#Printable Objects|printable]]. 
#### 3. Resolution
The horizontal ($xy$) and vertical ($z$) resolutions are based on:
	The specific technology, the material and the overall quality of the desired print. 
The horizontal resolution is the smallest movement that the extruder or print head can make horizontally and is expressed in microns (100 microns = 0.1 mm).
The vertical resolution is the thickness of a 3D printed layer.
Therefore, details smaller than the horizontal or vertical resolutions cannot be printed. 
#### 4. Gravity
The 3D printed object, being a physical object, must obey natural physical laws when printing.
Basic gravity-point tests and simulations can be performed using external software to check models for successful printability. 
## *Example*: Printable 3D Model/Object
### Parametric Modeling of a Vase
Using a common desktop printer with a **build volume** of 200 x 200 x 200 mm, this example will demonstrate a technique to create printable geometries.
![[Pasted image 20240419001133.png|300]]
#### The Algorithm
Overview:
	1. [[#Part I Generate Initial Closed Curve and the Set of Translated Closed Curves, Then Scale Each Translated Curve|Generate Initial Closed Curve and the Set of Translated Closed Curves, Then Scale Each Translated Curve]]
	2. [[#Part II Rotate Each Translated Curve, Then Generate Surface Between Them|Rotate Each Translated Curve, Then Generate Surface Between Them]]
	3. Transform into Watertight Object

#### Part I: Generate Initial Closed Curve and the Set of Translated Closed Curves, Then Scale Each Translated Curve
![[Pasted image 20240423120518.png|600]]
##### 1. Generate Initial Closed Curve
Define a [[Nurbs Curves#Closed NURBS Curves|closed NURBS curve]] i.e. [[Transformations#Point to Curve|Point to Curve Transformation]]
	Within a 100 x 100 mm square. 
##### 2. Generate the Set of Translated Closed Curves
Translate the curve vertically according to a scalar (list of scalars generated by the **Series** component).
Generates a set of translated closed curves with a step size of 10 mm. 
The [[#1. Maximum Size (i.e. build volume)|Build Volume Constraint]] is [[#Parametric Modeling of a Vase|200 mm]].
	Therefore, the (C) input of the **Series** component is set to 18. 
		The resulting geometry will have a $z$ dimension equal to 180 mm. 
##### 3. Scale Each Translated Curve 
The translated closed curves are then scaled using the centroid of each as the center of the scalings.
A **Graph Mapper** component determines the scaling factors.
	Set to *Bezier* in this case.
	Because the $x$ and $y$ [[#1. Maximum Size (i.e. build volume)|Build Volume]] constraints are [[#Parametric Modeling of a Vase|200 mm]], the Y Domain of the **Graph Mapper** component is set between $[0, 2]$ such that the maximum scale factor, 2, will produce geometry within the build volume constraint.   

![[Pasted image 20240423122231.png]]
#### Part II: Rotate Each Translated Curve, Then Generate Surface Between Them
![[Pasted image 20240423193215.png|600]]
##### 1. [[Surface Creation#Rotational (NURBS) Surface Generation|Rotate each translated curve]] around a central axis using the **[[Euclidean Transformations#Rotate Axis component|Rotate Axis]]** component.
The angle of rotation in radians (A) input for each curve is defined using the **Series** component.
##### 2. [[Surface Creation#Lofted (NURBS) Surface Generation|Lofted Surface Generation]] Between the Rotated, Translated Curves
Produces an [[Surfaces#Untrimmed Surface|untrimmed surface]], which is not a [[#2. Minimum Wall-Thickness|printable object]].
![[Pasted image 20240424123327.png]]
#### Part III: Transform into a Watertight Object
![[Pasted image 20240424123725.png|]]
##### 1. Generate a Lower Cap, Then Join Cap to the Surface with a Smooth Edge
*If the cap via **Boundary Surfaces** component and then the wall thickness is assigned via **Mesh Thicken** component, the result would be a printable object but one with undesirable sharp edges.*

To avoid sharp edges:
###### 1. Extract a vertical isocurve from the lofted surface, at a point defined on the curve (curve/item at index 0, of rotated geometry list- i.e. the initial planar profile curve) via the **Evaluate Curve** component with parameter ($t) =1$ (which extends the defined point to the "top" of the curve)
The **Evaluate Curve** component outputs the points associated with the curve at $t=1$, which are then input into a **Surface Closest Point** component which finds that input point on the given surface.
	This then outputs the $uv$ point on the surface which are then input into an **[[Surface Analysis#Isotrim aka SubSrf Component|Isotrim]]** component along with the surface. 
Then the extracted isocurve is joined with a curve defined from the centroid of curve (at index 0) and the starting point of the isocurve. 
![[Pasted image 20240424124805.png]] ^72bc65
###### 2. Generate a Smooth, Freeform [[Nurbs Curves#Non-Planar Curve|Non-Planar Curve]] 
Divide the [[#^72bc65|defined curve]] via **Divide Curve** component.
	This outputs points which when input into the (V) input of a [[Nurbs Curves#NURBS Curve component|**NURBS Curve** component]]
![[Pasted image 20240424130208.png|400]]
###### 3. [[Surface Creation#Translational (NURBS) Surface Generation|Translate the NURBS Surface]] (along a directrix)
![[Pasted image 20240424133330.png|600]]
The generated NURBS curve is translated (revolved in this case) 