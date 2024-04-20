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