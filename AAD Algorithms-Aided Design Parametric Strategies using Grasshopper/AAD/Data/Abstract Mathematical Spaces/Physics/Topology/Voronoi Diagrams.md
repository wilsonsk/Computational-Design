---
up:
  - "[[Data Relationships]]"
related:
  - "[[Scalar Fields]]"
  - "[[SubD Surface Patterns]]"
  - "[[Limits]]"
  - "[[Derivatives]]"
  - "[[Secant Line]]"
date created: 2024-04-12
---
# Voronoi Diagrams
A [[Grids#The Pattern of Pattern Creation|pattern]] Named after the mathematician Georgii Voroni):
The **Voronoi diagram** is a way of dividing space into a number of regions.
- Is the **decomposition** of a **metric space** according to **proximity criteria**.
	- **Partitioning Pattern**:
		- Is based on the **nearest neighbor rule/pattern**.
		- I.e. It is the **partitioning** of a **plane or surface** into **regions aka Voronoi cells** based on **distance** to **points aka seeds/sites/generators** in a **specific subset** of the **plane or surface**. 
			- Where each **region** aka **cell** is associated with **exactly one** **seed/site/generator** aka **point**.
## Voronoi Seeds $(S)$:
A **set** $(S)$ of *n* points ($S_1, S_2, ..., S_n$).
- A **Voronoi diagram** for a set (S), is the decomposition of bi-dimensional space.
	- Which associates a region $V(S_i)$ to each point of $(S)$, so that all points within $V(S_i)$ are **closer** to its own **seed** $(S_i)$ than **another other point of $(S)$** (i.e. any other cell's seed).

We can think of each Voronoi seed as an "attractor" in the sense that each point in the Voronoi cell is "attracted" to its seed by being closer to it than to any other seed.
	However, this attraction is purely a static, geometric relationship based on distance, not a dynamic process.
## Voronoi **Cell** aka region $V(S_i)$:
Encloses **all points** of a plane or surface that are **closer** to its own specific **seed**. than any other cell's.
## Voronoi Edges:
The **boundaries** between the **cells** are **equidistant** from the **nearest two (or more)** **seeds**.
## Voronoi Vertices:
The **points** where **three or more cells meet**.
## Voronoi diagram as a [[Scalar Fields#Distance Fields|Distance Field]]:
Voronoi diagrams are a type of Distance Field.
- And a Distance Field is a type of [[Scalar Fields#Scalar Fields|Scalar Field]].
![[Pasted image 20240409142211.png|300]] ![[Pasted image 20240411141309.png|300]]
 ^dec1a5
## Applications:
Computer graphics (like [[SubD Surface Patterns|SubD Mesh Surface Patterns]]), optimization, spatial analysis, geographical mapping, urban planning, and in simulating natural phenomena (like growth patterns of forests, territorial domains of animals and morphological topology).
## [[SubD Surface Patterns#Voronoi Data Management 3a5b41 Skin (i.e. abstracted "layer")|Voronoi]] Diagrams and [[Discontinuities]]
[[#Voronoi Vertices|Voronoi vertices]] are often **considered points of discontinuity** in the context of the **spatial organization** they represent.
- Not necessarily in the classical mathematical sense of a function being discontinuous. 
	- So direction **of a curve** is not the considered measure of a change in continuity for Voronoi diagrams.
		- But it is the change in the **[[Scalar Fields#Gradient of the Distance Field $ triangledown f$ (where $f$ is a scalar field)|gradient direction]]** for a given point, that is considered the measure of change in continuity. 
### Voronoi Vertex as a Point of [[Discontinuities|Discontinuity]]:
**Discontinuity as a Voronoi seed changes for a given point:**
#### Movement **along** a [[SubD Surface Patterns#^146787|Voronoi edge]]:
- A point remains equidistant from the other corresponding Voronoi seeds.
	- Not "in" any one cell.
#### Movement **across** a Voronoi Edge:
Because of the spatial orientation of a Voronoi vertex being equidistant to at least three Voronoi seeds:
- Even the tiniest movement near a vertex results in a significant and abrupt change in the "nearest Voronoi seed" for that given point that represents the movement.
	- This behavior is described as **discontinuous**:
	- Because the nearest Voronoi seed changes abruptly with minute movements from the the Voronoi vertex.
		- Which would be an abrupt change to the given point's corresponding gradient direction relative to the newly changed Voronoi seed. 
			- This contrasts from slight movements within a given Voronoi cell, where slight movements generally does not change the nearest Voronoi site immediately (due to the orientation relative to the edges of multiple Voronoi cells).
#### Discontinuity (i.e. abrupt changes) in [[Scalar Fields#Gradient|Gradient]] Directions:
If we define a [[Scalar Fields#Distance Fields|distance field]] having points, whose values are their corresponding distances to the nearest Voronoi seed:
- The gradient of this field (representing the direction and rate of fastest (i.e. highest) increase in distance) **does not behave smoothly** around the Voronoi vertices.  
	- As you cross over a Voronoi edge near a vertex, the nearest generator point changes. 
		- This results in an abrupt switch in the direction of the gradient vector. 
			- Since the gradient points away from the nearest generator point, it flips direction as the nearest site changes.
				 - **The direction in which the distance increases most rapidly (i.e. the direction that increases the field value for a given point most maximally), which is directly away from the nearest seed, can change suddenly as you near or cross a vertex
					 - Making the gradient appear "sharp" or "jagged" in its behavior at these points.**
						- This is further indication of discontinuity
#### Smoothness
The gradient of the distance field at a vertex does not behave smoothly because it does not have a single, well-defined direction of change. 
- Instead, the direction of the maximum increase in distance, varies abruptly depending on slight shifts in position relative to multiple nearby generator points.
	
The gradient, which points in the direction you would travel to increase the distance most quickly, will thus point away from whichever site is currently the nearest. 
- This results in a kind of "pinwheel" effect where the gradient direction changes drastically and discontinuously as you circle around the vertex, unlike in other areas where the gradient direction changes gradually as you move.
#### Discontinuity as Topology changes:
Moving through a Voronoi vertex along a small path can result in a change in the topological connectivity of the Voroni cells that meet at the vertex. 
- These points mark changes in the Voronoi cell arrangement.
	- Which can be interpreted as a form of discontinuity. 