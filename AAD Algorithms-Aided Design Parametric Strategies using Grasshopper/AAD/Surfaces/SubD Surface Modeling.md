---
up:
  - "[[Meshes]]"
related:
  - "[[Surfaces]]"
  - "[[Surface Creation]]"
  - "[[Parametric Space]]"
date created: 2024-04-07
---
# Subdivision Surface Modeling (SubD):
A specific alternative to NURBS modeling (A Weaverbird plugin). 
- Specifically beneficial for freeform geometries because it allows for a more intuitive sculpting process, akin to working with "digital clay".
###### Limit Surface:
- Refers to a concept in the subdivision of surfaces.
	- Which is a method used to create smooth and complex shapes from coarse polygonal meshes, through an iterative process of refinement. 
- It is the theoretical surface obtained after applying an infinite number of subdivision steps to the initial polygonal mesh.
	- I.e. The Limit Surface is the surface **defined** by **infinite iterations** of a subdivision algorithm.
- Therefore, **the number of iterations** is **counter proportional** to the **change** in **geometry**.
	- As a result, only a few iterations are usually required to approximate a limit surface.
- **Key characteristics**:
	- Smoothness:
		- The limit surface represents the ultimate smooth form that the subdivision process aims to achieve.
			- With each subdivision step (iteration), the polygonal mesh gets closer to this smooth surface.
	- Convergence:
		- As the number of subdivision steps increases, the subdivided mesh converges (i.e. approaches) to the limit surface.
		- In practice, only a finite number of steps are applied.
			- But the surface approximates the limit surface closely enough for most applications.
	- Mathematical Definition:
		- For many subdivision algorithms (Loop subdivision, Catmull-Clark, etc.), the limit surface can be mathematically defined.
			- It is often described using parametric equations or as the solution to certain differential equations (depending on the subdivision algorithm used).

SubD modeling generates a smooth polygonal surface (approximate **limit surface**) associated with any given input mesh:
- Processes an input mesh, and generates an output mesh that is closer to the **limit surface**.
	- The process starts with a basic form made from a relatively simple polygon mesh (i.e. a low polygon count mesh).
		- Through subdivision you refine and increase number of faces (high face count mesh) and thus the smoothness of a shape iteratively.
			- Enabling a level of smoothness which is quite difficult to obtain using NURBS techniques. 
- **Different SubD algorithms** are employed **depending** on the **type of input mesh** (triangular, quadrilateral, etc.).
	- Particularly:
		- Loop subdivision algorithm:
			- Commonly used for subdividing **triangular meshes**.
		- Catmull-Clark subdivision algorithm:
			- Commonly used for subdividing **quadrilateral meshes**.
## Loop Subdivision Algorithm: Subdividing Triangular Meshes
An **iterative subdivision method** for **triangular** meshes (developed by Charles Loop in 1987).
![[Pasted image 20240409001524.png]]
1. **For every edge in the source mesh**, the **algorithm** adds a **new vertex** at the **mid point**.
2. The **mid points** are **connected** and **every triangle** is **replaced** by **four** **sub-triangles**.

**Each iteration** of the Loop Algorithm **approaches** the **limit surface**.
- Producing limit surfaces that are composed of piecewise quadratic patches.
- **The number of iterations** is **counter proportional** to the **change** in **geometry**.
	- As a result, only a few iterations are usually required to approximate a limit surface.

### Loop Subdivision aka "wbLoop" component:
Performs the **Loop subdivision algorithm** to produce **smooth mesh**. 
- Inputs:
	- (M): The open or closed input mesh, or closed curves list, to subdivide. 
	- (L): The "**Level**" or number of **subdividing iterations** for **each face**.
		- The number of iterations can vary from 1-3.
			- Generally, a simple and schematic input mesh will yield a more refined and polished output mesh.
	- (S): Smooth [[#^7041ea|naked edges]]; Define how to treat the naked edges:
		- (0): Fixed; Naked edges will not move or be modified during subdivision.
			- **Use Case**: This option is useful when you want to preserve specific edges in your design intentionally.
				- Ensuring they maintain their original geometric integrity and positioning.
					- It's helpful for maintaining sharp edges or when the mesh boundary should remain unchanged for design or fitting purposes.
				![[Pasted image 20240409005645.png]]
		- (1): Smooth; The naked edge will tend toward a spline.
			- Meaning they will become smoother and may shift position to create a more continuous, curved boundary.
			- **Use Case**: This is suitable for models where a smoother transition at the boundaries is desired, contributing to an overall smoother and more organically shaped object. 
				- It enhances the aesthetic quality of models where hard edges are not necessary, or a more fluid form is preferred.
		- (2): Corner Fixed; Corner (2-sided vertices) will be fixed, while other naked vertices will tend toward a spline.
			- Vertices that have only two connected edges (i.e. corner vertices) will remain fixed.
			- Naked vertices along naked edges will be allowed to smooth as if tending toward a spline.
			- Meaning the mesh will partially smooth its boundaries, except at corners where geometry will remain "sharp".
			- **Use Case**: This option is particularly useful for designs that require a mix of smooth and sharp features. 
				- For example, a model might have certain areas where a smooth, flowing edge is desirable, but sharp corners are essential for the design's aesthetic or functional aspects.
				![[Pasted image 20240409005715.png]]
- Outputs:
	- (O): The output mesh after the subdividing process.
![[Pasted image 20240409005253.png|400]]
![[Pasted image 20240409005354.png|400]]
- ###### "Naked edges/vertices": ^7041ea
	- Refer to specific characteristics of the mesh's geometry.
		- They indicate its incompleteness or openness.
	- **Naked Edge**:
		- Is an edge of a mesh that **does not have** two adjacent faces.
			- I.e. An edge that belongs to only one polygonal face.
		- In a **closed mesh** (i.e. one that fully **encloses** a volume without any gaps):
			- Every edge is **shared** by **exactly two faces**.
		- Therefore, if a **naked edge** exists:
			- The **mesh is open** at that edge.
		- Can help indicate locations where the mesh might need to be closed off to create a sealed (i.e. closed) volume.
			- **Naked edges delineate the limits of where the algorithm can apply its refinement rules.**
	- **Naked Vertices**:
		- A **vertex** that is **connected** to **naked edges**.
			- Therefore, a naked vertex is part of the mesh's naked edge (i.e. boundary, open edge).
		- It is a vertex that does not have a closed set of faces around it.
		- Naked vertices help identify points of discontinuity or openings in the mesh structure.
			- Serving as an indicator of mesh incompleteness or potential areas for further refinement or closure.
- The Loop algorithm also works for meshes with holes.
	- Once the mesh is subdivided, the hole will become pseudo rounded. 
		![[Pasted image 20240409005901.png]]

## Catmull-Clark Algorithm: Subdividing Quadrangular Meshes
An iterative subdivision algorithm for **quadrangular** and **triangular** meshes. (developed by Edwin Catmull and Jim Clark in 1978).
![[Pasted image 20240409010206.png]]
- For **each face** a new vertices are added iteratively.
### 1. New Face Points
**New "face points" aka vertices** **placed** at the **centroid** of **each face** in the polygon mesh.
- The **position** of the **new face points** are **determined** by the **average of all the vertices** that define that corresponding face. 
	- *$F$ is the "face point" and $V_1, V_2, V_3, V_4$ are the vertices of the polygon*
		![[Pasted image 20240412215423.png]]
### 2. New Edge points 
New "**edge points**" aka vertices **placed** on the **original edge** of a polygon mesh.
- The exact edge point **position** is **determined** by the **average** of the **two vertices of the original edge, and the two new face points corresponding to the two faces that share the original edge**.
	- *$E$ is the edge between vertices $V_1$ and $V_2$, and $E$ is share by faces $F_1$ and $F_2$ which have corresponding new face points $P_{F1}$ and $P_{F2}$, then edge point $P_E$ is calculated as:*
		![[Pasted image 20240412215754.png]]
### 3. Adjusting Original Vertices
Each original vertex is **adjusted** based on its **neighboring original vertices**, the **edges it connects to** and the **adjacent faces**.
- Specifically, the new position $V^1$ of an original vertex $V$ is calculated as a **weighted average** of the **original vertex position**, the **average of the midpoints of all the edges connected to the vertex**, and the **average of all new face points of the faces touching the vertex**.
	![[Pasted image 20240412221045.png]]
		- This step **smooths** the original vertices to better blend with the newly created face and edge points.
### 4. Forming New Faces
The new geometry is constructed by connecting the new points.
- Each original face becomes several smaller, new faces.
	- These new faces are formed by connecting the new face point, new edge points, and the adjusted position of the original vertices. 
### 5. Iteration
Repeat the entire process to the newly produced geometry.
- With each iteration, the mesh becomes smoother and more refined, as more points continue to be added based on the existing mesh geometry.
	- Gradually approximating a smoother surface.
#### *Example: NURBS to Mesh Conversion via Catmull-Clark Algorithm*:
- *Applied to a [[Data Management#^55e72e|Rectangular Based Pattern]]*
- But BEFORE subdividing (into meshes) the individual sub-surface surfaces (via Catmull-Clark algorithm):
	- Each of these sub-surfaces must be converted into a mesh using the **Mesh Surface** component.
![[Pasted image 20240409091304.png]]
##### Mesh Surface:
- Creates a Surface *uv* Mesh.
	- Inputs:
		- (S): Input Surface Geometry.
		- (U): Number of quads in the *u* direction.
		- (V): Number of quads in the *v* direction.
		- (H): Allow faces to overhang trims (Boolean).
		- (Q): Equalize span length (Boolean).
	- Outputs:
		- (M): *uv* Mesh.
	- *Example*:
		- 3 sets of surfaces, each to be converted into a corresponding mesh:
			- Surface set (1): Frames (4 frames per set, each frame is 1*u* x 3*v*).
			- Surface set (2): Lateral Faces (4 lateral faces per set, each is 1*u* x 3*v*).
			- Surface set (3): Lower Faces (1 lower face per set, each is 3*u* x 3*v*).
			![[Pasted image 20240409123318.png|300]]
			![[Pasted image 20240409092959.png|400]]
- When converting a **single surface**:
	- The number of *u* and *v* subdivisions is arbitrary.
		- Because it is only considering a singular, continuous surface without worrying about how it interacts with adjacent surfaces.
- When converting **multiple [[Meshes#^b644d9|merged]] surfaces**:
	- The number of quads *u* and *v* should be set so that edges always meet in the vertices, avoiding T-nodes.
		- ###### T-Nodes:
			- *Example of T-Nodes due to inconsistent u and v counts:*
				- **Left** is the initial mesh conversion of each sub-surface via **Mesh UV** component.
				- **Right** is the subsequent **single mesh** generated by the **[[Meshes#^db8799|Join Meshes and Weld component]]**.
					- Which is used as an input single mesh by **[[#^e2c017|Catmull-Clark Subdivision component]]** component to produce a **smoothed subdivided mesh**.
				![[Pasted image 20240409123004.png]]
			- "Correct" (or desired in this specific case) Non T-Nodes due to consistent *u* and *v* counts such that the nodes can be welded:
				![[Pasted image 20240409123903.png]]
			- Refer to points where the mesh does not align perfectly.
				- Causing T-shaped intersection, rather than a neat grid of quads (four sided polygons).
					- The **stem** of the "T" is the **edge** being intersected.
					- The **horizontal top** of the "T" is the intersecting edge or vertex.
			- These occur when converting NURBS surfaces or other geometric forms into meshes.
				- Especially when dealing with complex shapes, or when multiple surfaces are merged into a single mesh.
		- To avoid T-nodes:
			- Adjusting number of *u* and *v* subdivisions so that the mesh edges of one surface align directly with those of the adjacent surfaces.
				- Allowing vertices to meet without overlapping or creating T-junctions.
- ###### Overhang trims:
	- Means that the mesh surface can extend past these predefined boundaries.
		- Can be particularly useful in complex modeling scenarios where a precise of organic overlap of the surface beyond its strict limits is desired. 
	- By default the edges of a mesh surface will **align** with the **trim curves** that define the **boundary** of the surface.
		- Enabling faces to **overhang** allows for a more complex and less constrained surface creation.
- ###### Equalize Spans:
	- The component will attempt to create divisions or segments that are as equal in length or area as possible.
		- This is in contrast to dividing based on the geometry's natural parameters.
			- Which might not produce evenly spaced segments.
				- Especially in cases where the geometry curves or stretches in various ways.
 - **If** the **nodes align** and **can be welded**:
	 - Than the **[[Meshes#^db8799|Join Meshes and Weld (wbJoin)]]** component can be used to create a **single mesh**.
		 - Which can be smoothed by the **Catmull-Clark Subdivision** component.
			 - By **[[Meshes#^34a214|flipping]]** the Surfaces set (3) (i.e. lower faces), enables the faces will be [[Meshes#^cc83c8|compatible]].
				 - I.e. Changing the orientation of the lower faces (normal directions) to match that of the other faces in the unit sub-surface.
					 - And therefore, can be joined, welded and smoothed.
			![[Pasted image 20240409124232.png|400]] ^c3a045
### Catmull-Clark Subdivision component: ^e2c017
Performs **Catmull-Clark subdivision algorithm** to produce a **smooth mesh**.
- Inputs:
	- (M): The open or closed input mesh, or closed curves list, to subdivide. 
	- (L): The "**Level**" or number of **subdividing iterations** for **each face**.
		- The number of iterations can vary from 1-3.
			- Generally, a simple and schematic input mesh will yield a more refined and polished output mesh.
	- (S): Smooth [[#^7041ea|naked edges]]; Define how to treat the naked edges:
		- (0): Fixed; Naked edges will not move or be modified during subdivision.
		- (1): Smooth; The naked edge will tend toward a spline.
		- (2): Corner Fixed; Corner (2-sided vertices) will be fixed, while other naked vertices will tend toward a spline.
- Outputs:
	- (O): Output subdivided mesh.
*Example*:
- Catmull-Clark algorithm applied to a [[Data Management#^ecb0e6|Hexagonal Based Pattern]]
![[Pasted image 20240409134716.png|400]]
![[Pasted image 20240409134742.png|400]]


