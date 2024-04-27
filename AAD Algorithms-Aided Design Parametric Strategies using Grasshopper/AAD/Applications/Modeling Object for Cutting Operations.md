---
up:
  - "[[Digital Fabrication]]"
related:
  - "[[Printable Objects]]"
date created: 2024-04-24
---
# Modeling Object for Cutting Operations
Objects that are unable to be manufactured by means of [[Digital Fabrication#Additive Techniques|additive processes]] can be fabricated using [[Digital Fabrication#(2D) Bi-dimensional Cutting|cutting (i.e. subtractive processes)]] based operations.
## Sectioning
Refers to contouring (contour/section lines) a model in one direction, typically parallel to a chosen axis.
It is a common technique used to build complex shapes by defining planar [[Gaussian Curvature#Developable Surfaces|developable surfaces]].
![[Pasted image 20240424230003.png|600]]
*For example*: A freeform **surface** can be **sliced** into **a set of parallel and planar sections based on an interval equal to the thickness of the material** to be [[Digital Fabrication#CNC Milling machines|milled]]. ^interval-between-sections-planes-equal-to-thickness-of-material
	Upon gluing the **sections** together in sequence, the original surface can be approximated.
If the same surface was milled from a single block of material, it the [[Digital Fabrication#Undercutting|undercuts]] would require the use of 3D milling machines.  ^interval-between-sections
### Continuity Parallel to Section Planes
Sectioning creates [[Continuities|Continuity (i.e. when curves join)|continuity]] (i.e. the smoothness or seamlessness of the surface along and across the sections) parallel to the cut section and .

In the direction parallel to the section planes (i.e. along the face of each slice), the continuity is more straightforward to maintain.
	As each section represents a "snapshot" of the profile of the object at that specific slice. 
	When these slices are aligned and [[Digital Fabrication#Assemblies|assembled]], the continuity along the plane of each section can be visually and physically coherent because the adjacent edges of each section directly correspond to each other. 
### Limited Continuity in the Normal Direction of the Section Planes 
It is actually impossible to get continuity in the direction normal (i.e. perpendicular) to the section-planes.
This is because this relatively perpendicular direction cuts across the natural continuity of the original surface.  
Each section plane is essentially **discrete**, isolated along the slicing axis. 
	There is no material continuity between these slices.
		They are separate pieces of the same material or different materials entirely. 
#### Discrete Nature of Sectioned Pieces
The reason continuity in the normal direction is hard to achieve post-sectioning lies in the physical nature of the process
	When an object is sectioned, whether by sawing, cutting, or using digital fabrication techniques, the process creates individual, discrete pieces.
	Each piece represents a cross-section of the original object at a specific interval. 
###### Gap Creation: 
Each section cut introduces a slight gap where the cutting tool passed through the material, no matter how thin. Even when using very fine cutting tools, this small gap can disrupt the original continuity.
###### Surface Imperfections: 
The act of cutting can introduce imperfections to the surface at the cut line. These might include slight deviations, roughness, or minor deformations that weren't present in the original continuous surface.
###### Alignment and Assembly Challenges: 
When reassembling the sections, aligning them perfectly to the original position can be extremely difficult. Any minor misalignment or inconsistency in the spacing can exacerbate the disruption in continuity. This is especially problematic with complex shapes or materials that are difficult to work with.

A common fabrication technique is to leave a space between each section to create the illusion of continuity in the normal direction. 
	By allowing the viewer’s eye to fill in the gaps, especially if viewed from a distance or certain angles.
![[Pasted image 20240424230133.png|600]]
![[Pasted image 20240424232407.png|600]]
## Uni-Directional Sectioning Algorithm
### General Outline
###### [[#1. Defining the Slicing Direction|1. Define Slicing Direction]]
###### [[#2. Generate Series of Section Planes|2. Generate Series of Section Planes]]
###### [[#3. Defining the Sections (i.e. Intersect the Planes with the Model)|3. Defining the Sections (i.e. Intersect the Planes with the Model)]]
###### [[#4. Convert NURBS curves into Arcs and Segments|4. Convert NURBS curves into **Arcs** and **Segments**]]

![[Pasted image 20240425225209.png]]
#### 1. Defining the Slicing Direction
![[Pasted image 20240425225353.png]]
Using one of the Boundary Edges of the referenced surface, the **origin points** for the **section planes** are defined along this edge. 
	The edges of the referenced surface are extracted, then one of "long" edges is specifically. 
#### 2. Generate Series of Section Planes
1. The end points of this "long" edge are extracted and used to generate a vector between them via **Vector 2Pt** component. 
	This resulting vector becomes the *z-axis* direction of each of the generated plane normals of each point along the edge. 
2. The **Divide Distance** component divides the edge according to a "preset distance" [[#^interval-between-sections|equal to the thickness of the material to mill]] in the (D) input.
	Each of the resulting points are the origin ((O) input) for a plane normal.

Each resulting Plane Normal of each division point (i.e. origin points for each section plane) is then **intersected** with the initial referenced surface via **Brep | Plane** (i.e. **Sec**) component.
###### Brep | Plane (i.e. Sec) component 
Solves intersection events for a Brep and a plane (i.e. a section).
- Inputs
	- (B): Base Brep.
	- (P): Section plane.
- Outputs
	- (C): Section curves.
	- (P): Section points. 
#### 3. Defining the Sections (i.e. Intersect the Planes with the Model)
![[Pasted image 20240425232555.png]]
Each resulting section curve is offset relative to the defined plane normal ("$z$ axis") (the "first" plane normal corresponding with the "first" point of origin of a section plane) via **[[Loops#Offset Curve component;|Offset Curve]]** component. 
	Where the (D) input is a "preset distance" [[#^interval-between-sections|equal to the thickness of the material to mill]].
	And each
##### *A potential issue:* Offsetting may produce [[Discontinuities|discontinuities]].
###### Why this might happen:
1. **Sharp Corners and Tight Curvatures**: When a curve has sharp turns or tight bends, offsetting these curves can result in segments that intersect or overshoot each other. This is because the offset curve attempts to maintain a constant distance from the original path all along its length. In areas where the curvature of the original curve is very tight, the radius of the offset curve can become smaller than the offset distance, causing self-intersections or cusps (pointed turns).
2. **Varying Curve Directions**: If the original curve changes direction abruptly, the offset curve might not smoothly transition through these changes. The offset process essentially creates a parallel curve, and sudden changes in direction in the original curve can lead to abrupt or disjointed segments in the offset curve.
3. **Non-uniformities in the Curve**: In cases where the original curve is not smooth (having variations in curvature or non-uniform parametrization), the offset curve may inherit or even exaggerate these imperfections. This can result in uneven distances between the original and offset curves and potential discontinuities.
4. **Curve Self-intersections**: If the original curve intersects itself or comes very close to itself, offsetting such a curve can easily lead to overlapping segments or complex self-intersections in the offset curve, which are hard to resolve and can be seen as discontinuities.
###### This issue is addressed (i.e. eliminated) by:
1. Dividing each offset curve into *N* parts.
		**Curve Refinement:** By dividing the offset curve into segments (or parts), the process refines the curve's definition. Essentially, it increases the number of points defining the curve, which allows for more detailed manipulation and adjustment in the subsequent steps. This step helps in managing complex curves that may have kinks or abrupt changes, which are typical sources of discontinuities.
1. Then rebuilding each offset curve using the **[[Nurbs Curves#NURBS Curve component|Nurbs Curves]]** component (NURBS curves are [[Continuities|continuous]]. 
		**Rebuilding with NURBS:** By rebuilding/converting the segmented curve into a NURBS curve, you essentially smooth out the points, providing a **continuous** and smooth curve that lacks the sharp corners or kinks that originally led to discontinuities.

*The blue curve is the original curve and the red curve is the rebuilt NURBS curve*
![[Pasted image 20240425234907.png]]

Lastly, each section curve is joined with its smooth offset by defining two segments that connect the curves' end points.
![[Pasted image 20240425235006.png]]
The **four** curves:
1. The offset curve as start point and section curve as end point
2. The section curve as start point and offset curve as end point 
3. The section curve
4. The offset curve
Are merged into a single Data Tree branch via **Merge** component set to **[[Data Trees|simplify mode]]**.
Then the merged branches are then joined, returning a list of closed planar curves. 
	These curves can then be oriented to a plane for milling. 

*Below image is the output of the joined curves i.e. the closed planar curves.*
![[Pasted image 20240425235045.png]]

Below image is the joined curves/closed planar curves oriented on the *xy* plane (i.e. such that all parts of every curve are **coincident** with the *Ixy* plane) via the **[[Euclidean Transformations#Orient component|Orient]]** component. 
![[Pasted image 20240425235851.png]]
Once the joined curves are oriented according to the *xy* plane, they can be transferred to a cutting or milling machine. 
#### 4. Convert NURBS curves into Arcs and Segments
Most [[Digital Fabrication#CNC Milling machines|CNC machines]] cannot read NURBS curves.
	As a result the **NURBS curves must be converted** into **arcs and segments**.  
		The conversion is based on two main strategies:
			1. Divide the curves into a large number of points and then define a polyline through the resulting points.
			2. Use Rhino's **Convert** command to convert curves into arcs or polylines with set tolerances. 

After the conversion, the resulting geometries are **nested** in order to minimize the material waste either manually, by third party software or by plug-in.
## Waffling
A **bi-directional planar section strategy**.
Waffling performs the section contouring procedure in two orthogonal directions. 
	An alternate way to build freeform objects by section planes.
![[Pasted image 20240426162922.png]]
*Below are examples of various waffling techniques, which are based on the initial shape and the direction of sectioning, to achieve a desired output.*
![[Pasted image 20240427082731.png]]
### Waffling Intersections
Waffling requires intersections on which to perform a standard set of operations.

Every possible intersection between every **rib** (or planar surface) is calculated and a list of intersection-segments are returned. 
![[Pasted image 20240427083154.png|400]]

At each intersection-segment two domain boxes(*A'* and *B'*) are created.
These boxes are subsequently subtracted using the **Solid Difference** operation: *A-A'* and *B-B'*.
![[Pasted image 20240427083325.png|400]]
A solid difference allows to create node-intersections between ribs.
![[Pasted image 20240427083453.png|500]] ![[Pasted image 20240427083509.png|400]]