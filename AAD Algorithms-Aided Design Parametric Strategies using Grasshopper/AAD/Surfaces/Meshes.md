---
up:
  - "[[Surface Creation]]"
related:
  - "[[Curves]]"
  - "[[Surfaces]]"
  - "[[Surface Analysis]]"
  - "[[Bezier Curves]]"
  - "[[3D Parametric Equations]]"
  - "[[2D Parametric Equations]]"
  - "[[Nurbs Curves]]"
  - "[[Notion of Surface Curvature]]"
  - "[[Grids]]"
  - "[[SubD Surface Patterns]]"
  - "[[SubD Surface Modeling]]"
date created: 2024-04-03
---
# Meshes (i.e. polygon meshes)

## vs. [[Nurbs Curves|NURBS]] modeling:
- Are mathematical representations expressed as curves and surfaces, providing a precise definition these complex shapes (geometric and freeform).
	- Are **single geometric entities**.
		- Because it can be defined by a singular set of mathematical equations, which defines its form.
			- Though when modeling, the NURBS surfaces and curves can be decomposed into tangible elements that can be extracted.
				- For example, the boundaries can be represented as edges and the surfaces as a face.
		- Where the computation of coordinates is based on one or more parameters:
			- *t* for curves.
			- *uv* for [[Notion of Surface Curvature|surfaces]].
	- Enable powerful manipulation through inherent parametric controls.
		- Degree, control points, weights and knots.
		- Manipulate smooth, freeform surfaces with high precision.
- Can be converted to meshes. 
- Limits:
	- Not always the most efficient or effective method for all types of geometries, especially freeform shapes.
	- Adding detailed features to a NURBS model, such as organic deformations, wrinkles or other intricate details, often requires additional effort that can lead to increased complexity in the model.
		- Where each detail requires its own set of curves and surfaces.
	- While NURBS excels in creating surfaces with high levels of mathematical continuity (C^0, C^1, C^2 continuity), managing this continuity across complex, intersecting surfaces can be challenging. 
![[Pasted image 20240403122920.png|400]]

## Polygon Meshes
### A conceptually different form of modeling than [[Nurbs Curves|NURBS modeling]].
- A set of vertices, edges and faces.
	- Define the shape of a polyhedral object in 3D and solid modeling. 
		- Via approximation by polygon meshes.
- The approximate the surfaces using a large number of polygons - typically triangles and quadrilaterals.
	- The level of detail and smoothness of a mesh is dependent on:
		- The number of polygons used.
			- Increased polygons means increased detail but at a computational cost.
- Are **not** strictly defined by mathematical logic or curves. 
	- Are **not** single geometric entities.
		- Are made through a **set of adjacent polygons** which determines the global shape.
			- And the polygons themselves are sets of elemental components:
				- Vertices, edges, and faces. all three of which defines the shape of the polygon.
- Are **not** actually smooth.
	- The greater the number of polygon faces, and thus the smaller the size of the polygon faces, the greater the appearance of smoothness.
	![[Pasted image 20240403122859.png|300]] ![[Pasted image 20240403123005.png|300]]
### A **set** of **elements**:
- **Vertices**:
	- Are the points defined in the WCS by relative coordinates (x, y, z). 
	- They provide spatial/positional information.
	- This information determines the shape of the polygon mesh's geometry.
- **Edges**:
	- Fundamental to the definition of a mesh's topology.
	- Are the segments that connect the vertices.
	- Do not inherently contain spatial information regarding position.
- **Faces**:
	- Composed of the set of vertices (for a given face) and the set of edges (for a given face).
	- Formed by edges that loop to create to create a **closed shape**.
	- In general, are formed by triangular or quadrangular polygons.
		- Faces are usually **non-planar** polygons.
			- Only **triangular** meshes can be guaranteed to have **planar faces**.
				- Because to be a triangle, the 3 vertices of that triangle **must be coplanar**.
			- Quadrangular meshes are not guaranteed to be planar. 
				- But, quadrangular meshes with planar faces are called **PQ Meshes** (Planar Quadrilateral Meshes).
					- PQ Meshes are fundamental to panelization techniques of freeform architecture.  ^16549d
						- **Quadrilateral**: 
							- A 2D shape with:
							- Four sides. 
							- Four vertices.
							- Four angles.
### Orientation
- The **connection-order** of the **vertices**:
	- **Determines** the **orientation** of the **face**.
	- **Distinguishing** the "front face" from the "back face".
	- **Front Facing**:
		- The **edges** that connect **vertices** are in the **counterclockwise** direction.
	- **Back Facing**:
		- The **edges** that connect **vertices** are in the **clockwise** direction.
- **Adjacent Faces**:
	- Are defined as **compatible** if they have the **same orientation**. ^cc83c8
		- A mesh is called **orientable** if it is composed of **compatible** faces.
		![[Pasted image 20240403133123.png|400]]

- For each **face** a **normal vector** can be defined:
	- A **front-facing** mesh has an **outgoing** normal vector.
	- A **back-facing** mesh has **ingoing**  (i.e. incoming) normal vector.
	- An **orientable** mesh has all **normal vectors** oriented in the same direction.
- ###### Flip component: ^34a214
	- Flips the **normals** of a surface based on local or remote geometry.
		- **Local Geometry**:
			- Refers to the intrinsic properties of the surface itself without consideration of the external objects or surfaces.
				- Like the surface's own orientation, curvature, or existing normal direction.
				- Therefore it is a self-contained operation, that ignores the position or presence of other geometrical elements in the model.
		- **Remote Geometry**:
			- Refers to a **point of reference**.
				- That is considered and influences some operation.
					- Is useful in scenarios where the relative orientation of another surface or elements in the environment is crucial. 
	- Inputs:
		- (S): Surface to be flipped.
		- (G): Optional guide (remote geometry) element (i.e. point, surface, object, etc.) to match the orientation of.
	- Outputs:
		- (S): Flipped surface.
		  (R): Result, true if surface was flipped (Boolean).


### Geometry and Topology
A mesh is can kind of be considered a single geometric entity, but:
- Its **geometry** is **defined** by a **set of vertices**.
	- The geometric properties of a mesh dictate its form and dimensions.
		- Crucial for visualizing and understanding its "physical" shape. 
- Its **topology** is **defined** by a **set of edges** and their **relationships to one another** (i.e. connection-logic/orientation).
	- ###### Topology:
		- Refers to how the vertices, edges and faces are interconnected and arranged relative to each other.
			- Crucial for understanding the mesh's structure - how its components are related.
				- Particularly important for operations like:
					- Deformation, subdivision, and simulation.
						- Where the connectivity and relationships between components define how the mesh can change or behave under certain conditions.
		- It describes a mesh's:
			- Connectivity.
			- The adjacency of elements.
			- The overall network of relationships within the mesh.
			- All without necessarily considering the geometric shape.
- *Example*: Two mesh-boxes with same geometry, but different topology:
	![[Pasted image 20240403140527.png|300]]
- *Example*: Two mesh-boxes with same topology, but different geometry:
	![[Pasted image 20240403141312.png|300]]

## Creating Meshes
Meshes are created to represent or approximate surfaces or volumes.
- In the digital space for simulations and visualizations.
- In the real world for manufacturing and construction.

The **process of creating a mesh**:
- Involves generating vertices on a surface (or within a volume) and then connecting theses vertices to form a mesh.
- ###### Defining Vertices:
	- ###### Scanned data:
		- Vertices can come from scanned data.
		- Scanners can capture the surface geometry of objects by thousands or even millions of vertices.
			- These points precisely map the contours and features of a surface.
	- ###### Mathematical models:
		- For objects designed digitally, vertices can be defined through mathematical models and equations.
			- Especially for geometric shapes (spheres, toroids, complex curves, etc.).,
		- CAD software enables designers to create these shapes.
			- Automatically generating vertices according to the specified dimensions and curves.
	- ###### Manual placement:
		- In some design processes, especially during early concept phases or for simpler objects:
			- Vertices can be manually placed by the designer using 3D modeling software.
				- This approaches gives the designer direct control over the mesh's density and detail level.
- ###### Generating Meshes:
	- Connecting vertices to connect them to form faces. 
##### In Grasshopper
There are several components used to create meshes, and others primitive components that are used to define single components.
- Mesh primitives for defining single components:
	- Plane, box, sphere, etc. 

### Three Main Strategies to Define Meshes in Grasshopper
###### Approaches to **generating** meshes, that is, connecting the vertices to form faces. 
1. Defining meshes by **topology**.
2. Defining meshes by **triangulation**.
3. Defining meshes by a **NURBS** to **mesh** **conversion**.

#### Defining Meshes by Topology
The process of defining mesh faces based on the connection order (i.e. the connection-logic) of the vertices. 
- A **mesh** is defined by a **set of vertices**, and the **direction of the sequence of their connecting edges**, **determines** the mesh's **topology**.
	- The **most basic** mesh:
		- A triangular face with edges connecting three vertices (0, 1, 2).
- ###### Construct Mesh component:
	- Used to build/define a mesh.
		- Inputs:
			- (V): Set of three vertices. 
			- (F): Define by a separate, preceding **Mesh Triangle** component.
				- Specifies the connection-logic (i.e. the topology) of the mesh.
					- **Mesh Triangle** component:
						- Inputs: Sequence of vertices connected by edges. 
							- Each "index" corresponds to a point index of a *uv* grid. 
								![[Pasted image 20240404133937.png|300]]
								- If only one number per input, then it defines a single face.
									- If more than one number per input, it is a list of numbers for that input.
										- Therefore, it is a list of indices for more than one face. 
										- For example:
											- Face 1: 0, 1, 2.
											- Face 2: 2, 1, 3.
												- Where Face 2's (A) input is the first index in the counterclockwise sequence.
											![[Pasted image 20240404181231.png|400]]
							- (A): Index of first face corner (i.e. vertex).
								- Specifying a corner/vertex index via number slider.
							- (B): Index of second face corner (i.e. vertex).
								- Specifying a corner/vertex index via number slider.
							- (C): Index of third face corner (i.e. vertex).
								- Specifying a corner/vertex index via number slider.
			- (C): Optional vertex colors.
		- Outputs:
			- (M): A constructed mesh.
			![[Pasted image 20240404075621.png|400]]
	- In order to create two **compatible** faces, the connection logic must be set as:
		- Face 1: 0, 1, 2.
		- Face 2: 2, 1, 3.
		- Where the (A), (B) and (C) inputs are all given two values.
			![[Pasted image 20240404113234.png|400]]
	- To create a **quadrangular** mesh face, the input (F) of the **Construct Mesh** component must be derived from a **Mesh Quad** component.
		- **Mesh Quad** component:
			- Has **four** Indices of a face corner (i.e. vertex).
				- Specifying a corner/vertex index via number slider.
					![[Pasted image 20240405003948.png]]
			- Can similarily to the **Mesh Triangle** add inputs to increase the number of faces defined by a given component.
#### Defining Meshes by Triangulation
###### "Skinny triangles": 
- When the length of one or two sides of a triangle is significantly longer than the other sides.
	- Leading to a narrow and elongated shape. 
		![[Pasted image 20240405145049.png|300]]
###### Why mesh topology without triangulation algorithms are not optimal for large or complex sets of points:
Mesh **topology** specifies the connection logic (i.e. order) of **vertices** to define a mesh **face**.
- This method can be applied to a small number of points or repeating logics. 
	- However, this technique is not appropriate for large numbers of points. 
-  Can produce "skinny triangles".
	- Skinny triangles are often produced when mesh topology doesn't use a method optimized for distributing triangles evenly across the surface. 
		- Which can lead to inaccurate results if the mesh is used to calculate simulations or conduct analysis as particle-spring systems or finite element method (FEM) analysis.
- ###### Topology (i.e. vertex connection order) Problems:
	- Defining a mesh based on topology (i.e. based on connection logic of vertices) can lead to irregular triangle shapes.
		- Especially when applied to complex or large sets of points without the aid of algorithms designed to balance a mesh's properties. 
			- Without considering the spatial distribution of the vertices, the resulting face can vary greatly in size and shape.
				- In large or complex sets, its challenging to maintain consistency in how vertices are connected, leading to irregular mesh faces.
- ###### Irregular Point Distribution:
	- Point distributions: 
		- Refer to the locations of vertices that will be used to construct the mesh.
	- Real world data or complex shapes often have points that are not evenly distributed. 
		- Some areas might be densely populated with points, while others are sparse. 
			- In terms of defining meshes by topology:
				- Faces positioned near densely populated areas might be well proportioned.
					- I.e. these vertices are densely packed together, making it easier to form well-proportioned triangles because the edges connecting these vertices are relatively short and similarly sized. 
				- But those spanning sparser regions can end up being stretched to connect distant points, forming elongated and skinny triangles.
					- I.e. the vertices are farther apart, connecting these distant vertices to form faces, leads to longer edges and, consequently, "skinny triangles".
- ###### Lack of optimization:
	- Without criteria that are considered in triangulation algorithms (minimizing the max angle), a mesh defined purely based on topology lacks the mechanisms to prevent the formation of undesirable triangles shapes.
- ###### Manual or arbitrary face definition: ^c62093
	- Defining a mesh by topology is based on arbitrary or manual decisions.
		- This approach might not take the most efficient or geometrically favorable paths to connect vertices, especially in complex geometries. 
			- As a result, some triangles are stretched or squeezed to fit the arbitrary paths chosen, leading to "skinny triangles".
- ###### Edge loop and closure:
	- Defining a mesh by topology, especially for closed surfaces, requires looping back to close the mesh.
		- This can sometimes force the creation of triangles with awkward angles. 
			- These closure triangles, necessary to seal the mesh, can be disproportionately shaped.
				- Especially if the remaining gap doesn't neatly accommodate a well-proportioned triangle.
##### Triangulation Algorithms
Minimize the difference between triangles in order to get a pseudo-regular mesh, avoiding skinny triangles. 
- They are designed to **evenly distribute** and **optimize** the **shape of triangles** across a mesh.
	- Addressing and preventing the [[#Why mesh topology without triangulation algorithms are not optimal for large or complex sets of points|challenges]] introduced by manual managing of vertex connection-logic (i.e. mesh topology).
###### Delaunay Algorithm aka Delaunay Triangulation:
Named after mathematician Boris Delaunay.
- Is one of the most popular methods because of the output's geometric properties.

The **Delaunay Algorithm** **connects** arbitrary sets of **vertices** by a **geometric procedure** that **maximizes** the **minimum angle of triangulation**.
- The resulting mesh tends to avoid "skinny triangles'".
- Creates the triangulation by:
	- "Choosing" triplets of vertices that meet the following condition:
		- **For any three points that form a triangle (*P$_0$, P$_1$, P$_2$*), the circle that exactly fits around this triangle, called the Delaunay circle, should not have any other points inside.**
			![[Pasted image 20240406002041.png|500]]
	- How it works:
		1. Starting Points:
			- Algorithm begins with a set of points in a plane.
				- These points are the vertices of the triangles that will be created.
		2. Super Triangle:
			- Initially creates "super triangle" which is a triangle large enough to completely contain all the points in the set.
				- Serves as the starting point for the triangulation process.
		3. Adding Points One By One:
			- The points are then added to the triangulation one at a time.
				- For each point added, the algorithm determines which triangle's Delaunay circle (i.e. circumcircle) contains the point.
		4. Triangle Splitting:
			- Once the point is found to lie inside a Delaunay circle, the triangle containing the point in its circumcircle is split into three new triangles.
				- Each new triangle is formed by connecting the added point to one of the original triangle's vertices.
		5. Edge Flipping:
			- After adding a vertex and splitting triangles:
				- The algorithm checks the neighboring triangles to ensure that the Delaunay condition is satisfied.
					- If a neighboring triangle has a point inside the Delaunay circle of the newly formed triangles:
						- The shared edge between these triangles is "flipped" to restore the Delaunay condition.
							- This edge flipping may cause a cascade of further edge flips.
		6. Repeat the Process:
			- This process is repeated for each vertex in the set:
				- Adding one point at a time.
				- Splitting triangles.
				- Flipping edges.
			- Until all the vertices have been added to the triangulation.
		7. Removing the Super Triangle:
			- After all vertices have been added and the Delaunay conditions is satisfied for all triangles:
				- The triangles that were part of the original super triangle are removed.
					- This leaves only the triangles that connect the original set of points in a Delaunay triangulation.
		8. The Result:
			- Is a mesh that convers the initial set of points.
				- This mesh has the properties that it maximizes the angle of all the angles of the triangles (avoiding skinny triangles) and that the Delaunay circle of each triangle does not contain any other point from the set.  
- ###### Delaunay Mesh component:
	![[Pasted image 20240406004537.png|400]]
	- Generates a triangular mesh according to the *Delaunay algorithm*, for a series of defined vertices (i.e. points).
		- Inputs:
			- (P): Series of vertices (i.e. points) from which to generate the triangular mesh.
			- (Pl): (optional) The plane or planes where the algorithm operates.
		- Outputs:
			- (M): Mesh.
	- *Example*:
		- A Tri-dimensional pattern from a freeform surface suing a Delaunay algorithm. 
			1. A triangular grid is created using the **Triangle panels B/ TriB** component (provided by the Lunch Box plugin).
				- ###### Triangle panels B/ TriB component: 
					- Creates triangular panels on a surface.
						- Inputs:
							- (Srf): A surface to be panelized.
							- (U): Number of divisions on the surface in the *u* direction.
							- (V): Number of divisions on the surface in the *v* direction.
						- Outputs:
							- Panels: Panel System.
			1. For each triangle, the centroid is calculated and subsequently moved (i.e. [[Euclidean Transformations#Translations|translated]]) according to the surface's normal vectors.
				- The **[[Surface Analysis#Surface CP|Surface Closest Point component]]** finds the closest point on the referenced surface to an external/input point.
				- The external points are the center of each of the triangular panels.
					- They already exist on the surface (i.e. *are* the *closes points* on the surface), so the **Srf CP** component simply identifies those center points themselves. 
				- The *uv* coordinates of each center is fed into an **Evaluate Surface** component as the *uv* coordinates of a point on the surface under evaluation.
					- From which a normal vector is identified from that point.
						- This is then used by the translation of the center point (in the z direction/normal direction).
			2. The Delaunay algorithm is performed on the three vertices of each triangle merged with the translated centroids.
				- Specifically:
					- The normal vector and plane extracted via the **Evaluate Surface** component, are used to create a plane via the **Plane Normal** component. 
						- This plane is passed into the **Delaunay Mesh** component.
					- The vertices of each triangular panel are extracted via **Deconstruct Brep** component, and passed into the the **Merge** component's Data stream 2 input. 
					- The translated centroid (in z/normal direction) are passed in to the **Merge** component's Data stream 1 input. 
					- The output of the **Merge** component is a Data Tree with branches containing paired:
						-  Translated centroids of the triangles.
						- The three vertices generating those associated centroids.
			1. The **Delaunay Mesh** component composes the vertices using the defined planes into a set of meshes with 3 faces. ^5ad95b
				1. Each face is a triangle using vertices from the original triangular panels, and the translated centroids. 
				![[Pasted image 20240406010614.png|500]]

#### Defining Meshes by NURBS to Mesh Conversion:
Meshes can be defined from a **base NURBS surface**. 
###### Mesh Surface / Mesh **UV** component:
- Converts a NURBS surface into a **Quadrangular Mesh**.
	- By specifying the number of quads in *u* and *v* directions. 
		- To display mesh edges, enable the *Mesh Edges* option (Display > Preview Mesh Edges).
		![[Pasted image 20240406134716.png|500]]
	- A **triangular mesh** can be extracted from a **quad mesh** via a **Triangulate** component (Ursula Frick and Thomas Grabner plugin).
		 ![[Pasted image 20240406134854.png|400]]

Remember that while triangular meshes are **always** planar... 
- ###### Quadrangular meshes are only planar under certain conditions. 
	- ###### *For example*, [[Surface Creation#Rotational NURBS Surfaces|rotational]] and [[Surface Creation#Translational NURBS Surfaces|translational]] NURBS surfaces return **planar quadrilateral** meshes (or **[[#^16549d|PQ Meshes]]**) when converted using the **Mesh uv component** component. 
		- Reasoning:
			- Because of the inherent geometric properties of these surfaces and the way they are constructed:
				- **NURBS Surface Structures**:
					- **NURBS surface**: Is generated by translating a NURBS curve through space, either by:
						- [[Surface Creation#Rotational NURBS Surfaces|Rotational NURBS surface generation]]
						- [[Surface Creation#Translational NURBS Surfaces|Translational NURBS surface generation]]
					- **Control Points Grid**:
						- The surfaces are defined by a grid of control points.
							- The connections between these control points naturally form quadrilaterals, especially when the surface is generated through straightforward processes like rotation or translation.
				- **Rotational NURB Surfaces**:
					- **Generated by Rotation**:
						- When the generator (i.e. profile curve) is rotated around the directrix (i.e. an axis), the resulting surface's control points are laid out in a manner that creates **rings** around the directrix (i.e. axis).
							- Each **ring** is formed by rotating a point on the generator (i.e. profile curve), creating a series of connected quadrilaterals as the rotation progresses.
							![[Pasted image 20240407012558.png]]
				- **Translational NURBS Surfaces**:
					- **Generated by Translation**:
						- The translation process maps out a series of control points along the directrix.
							- Connecting these points across the generator (i.e. profile curve) and directrix (i.e. path) naturally forms quadrilateral segments.
								![[Pasted image 20240407012820.png]]
				- **Advantages of PQ Meshes**:
					- Offer uniform structure that is easier to manipulate, refine and render using standard algorithms.
						- The uniformity also enables the application of textures and the performance of simulations on the surface.
					- Quadrilaterals are efficient for representing surfaces because they can easily be subdivided or coalesced.
						- And they work well with many rendering and mesh manipulation algorithms.
					- PQ Meshes align well with many digital fabrication processes.
						- These processes often prefer or require quadrilateral elements for generating toolpaths or performing structural analysis. 
- ###### Testing for Planarity:
	- **Face Boundaries** component:
		- Extracts each of mesh's edges. 
			- Returning a boundary polyline for each face.
	- **Planar** component:
		- Tests **each boundary polyline** for planarity.
			- Which returns a Boolean, "*true*" or "*false*" for each boundary polyline.
	- Alternatively:
		- **Boundary Surfaces** component:
			- Can be used to **test for planarity**.
				- By definition, the component will draw a surface only if the input curves form a planar boundary. 
		![[Pasted image 20240407112118.png|500]]
###### NURBS to Mesh conversion via Specifying Topology:
![[Pasted image 20240407112228.png|500]]

- An initial referenced surface is divided into sub-surfaces via **Isotrim** operation (**SubSrf + Divide Domain$^2$**).
- The **Deconstruct Brep** component extracts the vertices of each sub-surface.
- The extracted vertices are passed into the **Construct Mesh** component along with a [[#^c62093|manually defined topology]] to generate a set of **quadrilateral meshes**.
- The set of quad meshes is then **joined** into a single mesh via **Mesh Join** component.
	- ###### Joining Meshes: ^59c337
		- Refers to the operation of combining two or more separate mesh objects into a single mesh entity.
			- This process does not inherently alter the geometry of the individual meshes.
				- **Instead it creates a composite mesh that contains all the faces, edges and vertices of the original meshes**.
		- Purpose:
			- Useful for organizaion:
				- Simplifies the scene hierarchy.
				- Prepares meshes for operations that can only be applied to a single mesh entity, rather than multiple mesh entities.
	- ###### Mesh Join component:
		- Joins a set of meshes into a single mesh.
			- Inputs:
				- (M): Meshes to join.
			- Outputs:
				- (M): Joined Mesh.
	- Alternatively:
		- ###### Welding Coincident Vertices: ^b0951e
			- **Refers to the process of merging vertices that occupy the same (or nearly the same) spatial position into a single vertex.**
				- I.e. Merging vertices where their edges are converging together. 
			- Purpose:
				- **Eliminates redundancy**, decreasing complicated mesh editing, analysis and rendering.
					- Simplifies the mesh structure.
				- **Improves Continuity**, decreasing the apparent non-continuous, segmentation (rendering engine might treat these un-welded vertices as separate edges or faces).
					- Increases smoothness, ensuring the mesh is interpreted as a continuous surface.
				- **Facilitates smoothing and subdivision**, creating a continuous mesh without unnecessary vertex splits, which is essential for achieving predictable and desirable results.  
		- ###### Join Meshes and Weld component (*wbJoin*): ^db8799
			- (A Weaverbird plugin) can be used to join meshes and **weld coincident vertices** that are specified by a Boolean toggle.
				- Inputs:
					- (M+): A list of open or closed meshes.
					- (W): Weld indicates if the coincident vertices of the mesh faces should be joined after the union (a Boolean toggle).
				- Outputs:
					- (M): The constructed mesh.
			![[Pasted image 20240407145348.png]]
- ###### Joining Meshes Vs. Merging Meshes: ^b644d9
	- ###### Joining Meshes:
		- Refers to the process of combining multiple mesh entities into a single mesh without necessarily altering the individual vertices or faces of those individual meshes.
	- ###### Merging Meshes:
		- Goes a step further by not only combining multiple mesh objects into one, but also unifying the vertices at the edges with the meshes meet.
			- This can involve [[#^b0951e|welding]] vertices that are within a certain distance of each other.
				- Effectively removing the boundary between the original mesh objects.
					- Creating a seamless single mesh.
###### NURBS to Mesh Conversion and [[Surfaces#Trimmed/Untrimmed Surfaces|Trimmed/Untrimmed Surfaces]]:
Compatible with **untrimmed** surfaces.
- Because untrimmed surfaces **contain** a **rectangular** Isogrid, that can be **converted** into a **set of quad meshes**.

Not Compatible with **trimmed** surfaces.
- Trimmed surfaces that are converted using the **Mesh Surface** component:
	- Will return a polygon mesh that approximates the **original boundary geometry**.
- Trimmed surfaces that are converted using the **Mesh Brep** component:
	- Will return a polygon that preserves the original boundary geometry, but allows for thin triangles.
- The NURBS to mesh conversion method for a **trimmed surface** must be considered case by case.
- A possible strategy to convert a trimmed surface into a mesh:
	1. Adding an arbitrary point *O*.
	2. Dividing the surface's boundary into *N* parts getting *N* points *P*$_i$.
	3. Creating a set of lines from *O* to the subdivision points *P$_i$*.
	4. Dividing the lines into equal parts and connecting the resulting points with a set of polylines.
	5. Splitting the initial surface using the network of lines obtained in *step 3* and *step 4*, to generate a set of trimmed sub-surfaces.
	6. Extract the sub-surfaces' vertices and create the mesh relying on the topology method. 
	![[Pasted image 20240407163400.png|500]]
