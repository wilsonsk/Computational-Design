---
up:
  - "[[SubD Surface Modeling]]"
related:
  - "[[Data Management]]"
  - "[[Grids]]"
  - "[[Parameters]]"
  - "[[Points]]"
  - "[[Surface Creation]]"
  - "[[Surfaces]]"
  - "[[Surface Strategies]]"
  - "[[Surface Decomposition]]"
  - "[[Surface Analysis]]"
  - "[[Derivatives]]"
  - "[[Limits]]"
  - "[[Secant Line]]"
  - "[[Voronoi Diagrams]]"
  - "[[Meshes]]"
date created: 2024-04-09
---
# SubD Surface Patterns

## [[Voronoi Diagrams|Voronoi]] [[Data Management#^3a5b41|Skin]] (i.e. abstracted "layer")
### Implementation Methods:
#### Brute Force:
Involves checking the distance from each point in the space to all generating points to determine the closest one. 
- This brute-force method is not efficient for a large number of generating points.
#### Fortune's Algorithm:
A more efficient sweep-line algorithm that constructs the Voronoi diagram in *$O (nlogn)$* time.
- Which is much faster for computational purposes.
#### [[Meshes#Delaunay Algorithm aka Delaunay Triangulation|Delaunay Triangulation]] (i.e. Delaunay Mesh):
There is a dual relationship between Voronoi diagrams and Delaunay triangulations. 
- Given one, you can construct the other. 
	- The Delaunay triangulation for a set of points produces triangles such that no point is inside the circumcircle of any triangle. 
		- The **edges of the triangles** in Delaunay triangulation are **perpendicular bisectors** of the [[Voronoi Diagrams#Voronoi Edges|Voronoi edges]] in the Voronoi diagram.
			![[Pasted image 20240412211619.png|400]]
## Creating a Voronoi [[Grids#Grid Utilization in NURBS Surface (i.e. Skin) Generation and Pattern Design|Skin]] (i.e. Voronoi surface layer) from a Planar Voronoi Diagram
The procedure is to **define a set of pyramids** to smooth by a subdivision algorithm.
- Each pyramid has a Voronoi cells as a basis.
- Planar:
	- Meaning the diagrams are constructed in 2D, typically within a flat plane.
- Non-Planar:
	- Meaning non flat surfaces.
![[Pasted image 20240409172552.png|600]]
### Voronoi component:
Creates a **planar Voronoi diagram** from a given set of seeds (P), on a plane (Pl) within a containment boundary (B). 
- Inputs:
	- (P): Set of [[Voronoi Diagrams#Voronoi Seeds $(S)$|Voronoi seeds]] for Voronoi diagram.
	- (R): Optional [[Voronoi Diagrams#Voronoi **Cell** aka region $V(S_i)$|Voronoi cell]] radius.
		- If no radius provided, then it defaults to an infinite radius input.
			- Resulting in merged Voronoi cells.
	- (B): Optional containment boundary for diagram.
	- (Pl): Optional base plane. 
		- If no plane provided, then the best-fit plane will be used.
- Outputs:
	- (C): Voronoi cells of the Voronoi diagram. 
	![[Pasted image 20240409142844.png|400]]
- *"Default radius of Voronoi cells with no bounds*:
	![[Pasted image 20240409172335.png|400]]
### [[Discontinuities#Discontinuity|Discontinuity]] component:
Finds all discontinuities (i.e. changes in direction, curvature or derivative) along a curve.
- Inputs:
	- (C): Curve to be analyzed.
	- (L): Level of discontinuity to test for.
		- 1 = C1
		- 2 = C2
		- 3 = Cinfinite
- Outputs:
	- (P): Points at discontinuities.
	- (t): Curve parameters at discontinuities. 
- *For better understanding of **[[Limits#Discontinuity|discontinuities]]** as they pertain to limits and derivatives, see* [[Limits]], [[Derivatives]], [[Secant Line]].
- *For understanding [[Voronoi Diagrams|Voronoi diagrams]] and discontinuity*, see [[Voronoi Diagrams#SubD Surface Patterns Voronoi Data Management 3a5b41 Skin (i.e. abstracted "layer") Voronoi Diagrams and Discontinuities|Voronoi Diagrams and Discontinuity]]
### Voronoi Skin Procedure:
1. The (C) output of the **Voronoi** component is fed into the **Discontinuity** component.
2. Use **Discontinuity** component to return the [[Voronoi Diagrams#Voronoi Vertex as a Point of Discontinuities Discontinuity|discontinuity points]], that is the [[Voronoi Diagrams#Voronoi Vertices|Voronoi vertices]] that define each Voronoi Cell. 
3. The **Discontinuity** component creates a **branch** for each **Voronoi cell** with **$n$ items** (i.e. Voronoi vertices) per cell. 
4. The **centroid** (which is **not** the Voronoi seed) of **every Voronoi cell** is **translated** in the **negative z direction**. 
	- The Voronoi seeds are contained in some kind of point component, and were input earlier in the **Voronoi component**.
5. The **discontinuity points (i.e. Voronoi vertices)** and the **translated centroids**, are merged **into a single list**, via the (D1) and (D2- set to graft) inputs respectively, of the **Merge** component.
6. Take the **grafted output** from the merge and feed it into the (P) input of the **[[Meshes#^5ad95b|Delaunay Mesh]]** component.
	- The **result** after an initial mesh definition via Triangulation:
		- *Is formed by an $n$ number of unique, discontinuous meshes*.
			- *Is not a single joined and welded mesh*.
				![[Pasted image 20240412214602.png|400]]
7. Create continuity between the unique meshes by feeding the (M) output of the **Delaunay Mesh** component into the (M+ set to flatten) input of the [[Meshes#^db8799|Join Meshes and Weld]] component.
	- *The result after [[Meshes#^b0951e|welding]] the vertices and [[Meshes#^59c337|joining]] the meshes:*
		- *Is a single, welded mesh.*
	![[Pasted image 20240412231329.png|400]]
8. Finally, create a [[SubD Surface Modeling|subD mesh]] by feeding the single, welded mesh into a **Catmull-Clark** component. 
	![[Pasted image 20240412233548.png|400]]
	![[Pasted image 20240412233615.png|600]]
	![[Pasted image 20240412233643.png|400]]

### Non-Planar Voronoi Pattern
The previous [[Grids#The Pattern of Pattern Creation|pattern]] can be applied to nonplanar Voronoi diagrams.
- One strategy to enable this is based on **[[Data Relationships#Remap Numbers component|remapping]]**.
	1. Create a Voronoi diagram on the plane. 
	2. Remap the Voronoi vertices (i.e. discontinuity points) in a [[Data Operations#Range component|range]] between a [[Data Operations#Construct Domain component|domain]] of 0 and 1 via the **[[Data Relationships#Remap Numbers component|remapping]]** component. 
		- I.e. Taking the x,y coordinates of these Voronoi vertices, and converting them into new normalized range between 0 and 1. 
			- The vertices can now be applied to any surface that has also be reparametrized to have the same domain. 
				- The surface's *uv* parameters range from 0 to 1 across its length and width. 
		- This is the same domain that a reparametrized surface (i.e. a surface whose domain/bounds have been remapped to 0 and 1) would range between. 
	4. Therefore, **Evaluate Surface** component and **Polyline** component can be used to reproduce the Voronoi diagram onto a freeform surface. 
		1. **Evaluate Surface** component places the remapped vertices onto the surface/
		2. **Polyline** component connects these Voronoi vertices according to the Voronoi structure.
![[Pasted image 20240413000020.png]]
## Fading Pattern
Combines a **subD** algorithm with the **Image Sampler** component to generate a fading [[Grids#Tri-dimensional Pattern|tri-dimensional]] [[Grids#The Pattern of Pattern Creation|pattern]] informed by the grayscale image. 
- [[Grids#Bi-dimensional Pattern|A bi-dimensional pattern (i.e. a 2D grid) is generated from a NURBS surface]]. 
![[Pasted image 20240413001025.png|400]]
### Diamond Panels component (Lunchbox plugin)
Creates/outputs quadrangular (i.e. diamond) and triangular panels on a surface.
- Inputs:
	- (Srf): A surface to panelize.
	- (U): Divisions in the surface *u* direction.
	- (V): Divisions in the surface *v* direction.
- Outputs:
	- Diamonds: Full panel conditions (diamond/quadrangular).
	- Triangles: End panel conditions (triangular)
### Fading Pattern Procedure:
1. Utilize the **Diamond Panels** component to generate a set of sub-surfaces from an input surface (i.e. grid/pattern on a surface).
2. Extract the surface vertices of every sub-surface.
3. Calculate the centroid of every quadrangular sub-surface. 
	![[Pasted image 20240413002551.png|400]]
4. The centroid of each sub-surface is translated according to a scalar factor multiplied by the sub-surface normal unit vector. 
5. The four bounding vertices and translated centroid for each sub-surface are merged into a single Data Tree branch. 
6. The **[[Meshes#Delaunay Algorithm aka Delaunay Triangulation|Delaunay Mesh]]** component is then used to create a mesh pyramid from each branch.
	![[Pasted image 20240413002930.png|400]]
7. The **Image Sample** component is used to generate a list of **non-constant** scalars for the translation of the centroids of the sub-surface.
	- This non-constant scaling of centroids, is what creates the tri-dimensional pattern. 
	![[Pasted image 20240413134145.png]]
	- *The output pyramids at this point, throw an **error** that is a result of the orientation of each pyramid*.
The Orientation Error:
Arising primarily due to the inherent characteristics of how geometries are defined:
- In a complex model with multiple surfaces (i.e. a patterned mesh in this case), the normals of each sub-surface vary- sometimes significantly. 
	- This variation depends on the curvature and changes in the geometry of the underlying surface.
- Specifically, **when the pyramids are generated on these sub-surfaces, each pyramids orientation aligns with the normal at its base point on the sub-surface**.
	- If the surface and thus (sub-surfaces) are not uniform, and is instead "twisted or undulated", the normals at close points can diverge, leading to pyramids that tilt in different directions even if they are close to each other. 
		- So the **Delaunay Mesh** component was trying to create meshes in erroneous planes. 
The solution to the Orientation Error:
Define individual planes for each pyramid of the pattern, each plane taking into consideration more than just the corresponding normal, but also the normals of nearby points or an averaged direction.
**Using Plane Normal Component**:
- **Standardizing Plane Creation**: Generates a z plane based on the normal of the centroid of each sub-surface.
- **Correction of Orientation**: By creating planes based on the normals but managing these planes as separate entities, the solution standardizes how each pyramid is oriented, regardless of the local variability of the surface normals.
**Delaunay Triangulation for Unified Structuring**:
- **Mesh Creation**: Delaunay Triangulation is used to connect these planes into a coherent mesh. It considers points (or in this case, the centroids or reference points of the planes) to create a mesh that maximizes the minimum angle of all the angles of the triangles in the mesh, avoiding "skinny" triangles and ensuring more uniform, aesthetically pleasing tessellations.
- **Grafting Planes**: By [[Data Trees#Graft Tree component/operation|grafting]] the plane inputs to the Delaunay Triangulation component, each plane is treated as an independent unit. 
	- This is required to **match** the format of the **Merge** components output. 
		- I.e. Properly structuring the pyramid input data to be triangulated. 
**Resulting Uniformity**:
- **Consistent Orientation**: With each pyramid based on a standardized plane, all pyramids now follow a uniform orientation that aligns more closely with the overall design intent.
![[Pasted image 20240414151552.png|400]]
![[Pasted image 20240414151607.png|400]]
8. The output of the **Delaunay Mesh** component is flipped, then **merged** with the Triangles output of the **Diamond Panels** component that itself has been converted into a mesh via the **[[Meshes#Mesh Surface / Mesh **UV** component|Mesh UV]]** component.
9. Join and weld the two meshes