---
up:
  - "[[Surface Analysis]]"
related:
  - "[[Surface Strategies]]"
  - "[[Notion of Surface Curvature]]"
  - "[[Gaussian Curvature]]"
  - "[[Mean Curvature]]"
  - "[[Curves]]"
  - "[[Surface Creation]]"
  - "[[Surfaces]]"
  - "[[SubD Surface Patterns]]"
  - "[[Grids]]"
date created: 2024-03-25
---
# Surface Decomposition:
(*see* [[Data#Decomposition/Deconstruction|decompositon]])
## NURBS-surfaces can be visualized as a **geometrical object composed of three geometric entities**:
1. Faces
2. Edges
3. Vertices (*see* [[Points#^96eec9|vertices]])
### For **every surface**: These components can be **extracted**
 1. One **Face** (F<sub>0</sub>): is a **bounded portion** of the surface.
 2. Four **Edges** (E<sub>0</sub>, E<sub>1</sub>, E<sub>2</sub>, E<sub>3</sub>): are **bounded pieces** of curves. 
 3. Four **Vertices** (V<sub>0</sub>, V<sub>1</sub>, V<sub>2</sub>, V<sub>3</sub>): are **points** that lie at the corners.
 ![[Pasted image 20240324104805.png|500]]
### Deconstruct Brep component:
Deconstructs a Brep into its constituent parts.
- Is used to **extract** faces, edges, or vertices from a surface. Extracts the maintained **trimmed** surfaces. 
- Inputs:
	- (B): Base Brep.
- **Outputs**:
	- **Faces (F)**: A list of the **set** of **faces** contained in the Brep.
	- **Edges (E)**: A list of the **set** of **edges** contained in the Brep.
	- **Vertices (V)**: A list of the **set** of **vertices** contained in the Brep.
![[Pasted image 20240324104820.png|500]]
### Brep: Boundary Representation (*see* [[Data#Composition/Construction|composition]])
Describes a way of defining geometric forms using boundaries. 
- Primitives like boxes, cylinders, cones, etc. are defined by boundary representations.
	- I.e. a solid of polysurface is composed of sets of edges and sets of faces, "stitched" together to form a solid object. 
- For example: a NURBS-surface is considered is composed of a set containing one face. 
- So "box" primitive is actually a set of surfaces (which are each composed of sets of faces, etc.) and is NOT a single surface.
	- I.e. the "box" is composed of six surfaces that are **joined** together into a Brep.
		- In order to **extract** the surfaces, the box or Brep has to be **deconstructed** into surfaces using the the **Deconstruct Brep** component. 
			- That is, plugging a Srf component into the **output** of a center box component will produce an error. 
				![[Pasted image 20240324105703.png|500]]
### Splitting a surface using a generic curve:
#### Surface Split component:
Splits a surface via a set of curves that are coincident to the surface. 
	- **For example**: Using a **Geodesic curve**
		- **Geodesic Curve**: a shortest path along a surface between two points. It is analogous to a "straight line" on a plane. 
			- **Geodesics**:
				- On a curved surface, geodesics are the closest equivalent to straight lines in flat, Euclidean geometry. They represent the shortest route between two points on the surface. For example, on a sphere, geodesics are segments of great circles (like the lines of longitude or the equator on Earth).
			- **Not Euclidean Straight Lines**:
				- The concept of a straight line in Euclidean geometry does not directly apply to curved surfaces. On a curved surface, there are no truly "straight" lines in the Euclidean sense. Instead, geodesics fulfill the role of straight lines by minimizing distance between points within the constraints of the surface's geometry.
			- **Inputs**:
				- (S): A given surface.
				- (S): "Start Point" on an edge of the surface.
				- (E): "End Point" on a different edge of the surface.
			![[Pasted image 20240324110236.png|500]]
- The Surface Split component splits a surface (S) at a splitting curve (C) (which in the example was the geodesic curve).
- Output:
	- (F): Two **trimmed** surfaces.
- To create an untrimmed surface from a trimmed surface, the Deconstruct Brep component can be used to extract the edges and create a new surface using the component Edge Surface

### Examples of Decomposition Logic (Deconstruct Brep):
#### A Diagonal Grid:
Applied to a single subsurface:
- A sub-surface is extracted from a surface via Isotrim component (with inputs: a surface and a divide domain^2 components), and a List Item component capturing the 0 index element (subsurface) from the list of subsurfaces.
- The vertices of the sub-surface are extracted via Deconstruct Brep component.
- Each vertex output is itemized separately using a List Item component. 
- Two lines are created between **opposite** vertices:
	- List item 0 and 1.
	- List item 2 and 3.
- This creates a sub-surface with diagonal lines across it.
- Applied to an entire surface: or specifically to **each** sub-surface within the set contained by the surface.
- The entire set of sub-surfaces is extracted from a surface via Isotrim component (with inputs: a surface and a divide domain^2 components).
- The output of the Isotrim component is fed into a Deconstruct Brep component.
- Each vertex output (of the entire surface) is itemized separately using a List Item component. 
- Two lines are created between **opposite** vertices for each sub-surface:
	- List item 0 and 1.
	- List item 2 and 3.
- **But** because the algorithm is defined by connecting the vertices of the sub-surfaces, the diagrid is **not coincident** to the surface, except in for on planar sub-surfaces. 
- The **solution** is to use the Project component to project the diagonal curves onto and coincident with the surface.
	- Inputs:
		- (C): The curve (line in this case) to project onto the surface.
		- (B): The surface on which the curve will be projected.

#### A Space Frame: a [[Grids#3D UVW Volumetric Grids|3D]] truss or structure
- The diagrid algorithm can be extended to a create a **space frame**.
	- Feed the (F) output from the Deconstruct Brep component into the (S) input of the Evaluate Surface component.
	- Use a MD Slider (a bi-dimensional number generator) and set the value to (0.5,0.5) to approximate the center point of the input surface (S).
	- Remember to **reparametrize** the surface (S) in the Evaluate Surface component, as this sub-surface is still parametrized according to the parent surface.
	- The (P) output of the Evaluate Surface component is fed into the start points input (S) of the **Line SDL** component.
	- The normal vector (N) output of the Evaluate Surface component is fed into the direction (D) input of the Line SDL component.
	- The length (L) input of the Line SDL is given an arbitrary value via a number slider or a similar mono-dimensional number generator.
	- The Endpoint component extracts the end points of the line produced by the Line SDL component (L) output.
	- The end point (E) output of that Endpoint component is then fed into the (A) input of a Line component.
	- The vertices (V) output from the original Deconstruct Brep component is finally fed into (B) input of the Line component used in the previous step.
	- This generates a line to a point (in the approximate center of each sub-surface) that is normal to each sub-surface (with a distance or length from that sub-surface as controlled by the mono-dimensional number generator).
		- Then lines from each vertex of the sub-surface is produced to that point

#### Grid of Equidistant Points on a Generic Surface:
**Parametric Space** can be visualized as a **deformed** **Cartesian Grid** which **perfectly fits** an arbitrary **freeform surface**. 
- The **dimensions** of the grid are **dependent** on the **initial domain** as well as its **subdivision**.
	- As a consequence, the **edges do not have the same length** unless the surface curvature is equal to zero.
- **Chebyshev-net**:
- Developed by the Russian mathematician **Pafnuty Lvovich Chebyshev** (1821-1894).
	- A method of clothing curved surfaces by cutting and sewing flat pieces of fabric. 
- This method can be applied to a plane as well as any freeform surface.
	- It solves the requirement that: to generate a grid with equal-length edges, a grid of equidistant points on a surface must be instantiated. 
- A unique Chebyshev-net can be found from:
	- Given two arbitrary transverse curves *u* and *v* starting from an arbitrary point *P* of a surface.
**To find a grid of equidistant points in a [[Grids#Bi-dimensional Pattern|bi-dimensional]] space**:
1. A generic point *P<sub>0</sub>* is used to draw **two orthogonal** curves *u* and *v*. 
2. The desired edge length (L) is defined by drawing a **circle** *circle<sub>0</sb>*	with a radius (L) (i.e. equal to the desired edge length) originating from *P<sub>0</sub>*. 
3. Then intersecting the circle with the **isocurves** *u* and *v* to define *P<sub>1</sub>* and *P<sub>2</sub>*.
4. At the intersection points, *circle<sub>1</sub>* and *cirlce<sub>2</sub>* are drawn with the same radius (L) as the *circle<sub>0</sub>* and thus have their center points at *P<sub>1</sub>* and *P<sub>2</sub>.
5. The circles intersection defines *P<sub>3</sub>*.
6. The process is repeated for the remaining three quadrants to create a grid. 
	![[Pasted image 20240324141558.png|400]]
	
This method can be **extended** to **non-orthogonal curves** *u* and *v*. Resulting in a grid formed by a set of rhombi with equal-length sides. 
- Curves *u* and *v* are **not required** to be straight.
	- Example of a grid of equidistant points calculated from two isocurves on a **flat surface**:
		![[Pasted image 20240324141947.png|400]]
- **[[Grids#Tri-dimensional Pattern|Tridimensional Extension]]** of the bi-dimensional method:
	- Implies a tridimensional geometric construction, meaning a set of spheres are used replacing the set of circles.
	- **Construction** of a Tridimensional net:
		- Define two generic curves *G1* and *G2* on a surface S, and find their intersection, *P<sub>0</sub>*.
			![[Pasted image 20240324142508.png|400]]
		- Then expanding on the bi-dimensional method, a *Sphere<sub>0</sub>* with radius (L) is drawn along *G1* and *G2* (and thus remains on and conforms to the surface) to define *P<sub>1</sub>* and *P<sub>2</sub>*. I.e. the radius of *Sphere<sub>0</sub>* is a **geodesic** curve.
		- *P<sub>3</sub>* is found by intersecting two spheres (*Sphere<sub>1</sub>* and *Sphere<sub>2</sub>*) with the same radius (L) and thus their center points are *P<sub>1</sub>* and *P<sub>2</sub>, with the surface.
			- This generates curves which are intersected to define *P<sub>3</sub>*.
		- This procedure must be iterated and repeated for the remaining three quadrants to generate the complete grid. 
			![[Pasted image 20240324142832.png|400]]
			![[Pasted image 20240324142842.png|400]]
			![[Pasted image 20240324143122.png|400]]
		- What this importantly implies is that a grid of equidistant points can be flattened into a regular square grid:
			![[Pasted image 20240324143232.png|400]]
		- This implication and characteristic is **crucial** to **form freeform structures** (gridshells) starting from planar and deformable elements.
	- **IMPORTANT Concept**:
		- If you are confused about how the radii of the spheres can be "**straight**", remember these are not "Euclidean" straight lines. These are **geodesic** lines or shortest paths that connect the center points of the spheres. (*see the description of geodesics above in this doc*).
		- **Role of Spheres in Geodesic Construction**: 
			- By using spheres of a specific radius to define new points on a surface, the method ensures that these points are equidistant from their respective centers. 
			- The "edges" or lines connecting these points, therefore, are geodesics that represent the shortest path between them on the curved surface. 
			- The use of spheres ensures uniformity in distance and edge length but adapted to the surface's curvature.
		- **The Geodesics** are not just the shortest path between two points in space, but specifically the shortest path **within the constraints of a given surface**.
			- I.e. Geodesics are defined by the surface they lie on. Preventing the geodesic curves from "leaving" the surface to find a shorter route. 
