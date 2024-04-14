---
up:
  - "[[Data Operations]]"
related:
  - "[[Data Trees]]"
  - "[[Numbers]]"
  - "[[Number Systems]]"
  - "[[Elemental Building Blocks]]"
  - "[[Data]]"
  - "[[Data Control]]"
  - "[[Surface Creation]]"
  - "[[Surface Strategies]]"
  - "[[Surface Decomposition]]"
  - "[[Surface Analysis]]"
  - "[[Surfaces]]"
  - "[[Parameters]]"
date created: 2024-03-30
---
# Data Management
###### "Complexity that works is built up out of modules that work perfectly, layered one over the other" - Kevin Kelly

###### Relationships compose structure.
- *See [[Data#^1cd6a4|composition]]*.
## Abstractions (i.e. a set)
^data-abstractions
Are "singular" **representations** or **encapsulations** of compositional elements (i.e. data). ^c60676
- I.e. A representation of **complex data** (i.e. relational, multi-dimensional data) in simplified form (i.e. as a singular, representational structure).
	- That singular, representational structure *is* the **Abstraction**.
	A "one" to/of "many" **[[Data Structures|data structure]]**. 
	- Where the *one* "**hides**" or "encapsulates" the *many* (i.e. the details/complexity) of the structure. 
- Can be a **set of sets** or a **set of singular items**.

They can be thought of as a "**list of lists**" that **enables complex relationships** among its **compositional elements** and **facilitates** easier **management** (access, manipulate and control) the **internal data**. 

## Geometries are layers (i.e. skins) of abstractions - .
I.e. **Sets** **of** compositional **sets**.
- Nested Abstractions:
	- Each layer is a skin/set/list of its own respective [[Elemental Building Blocks|compositional elements]]. 

## Skins (i.e. abstractions representing layers that envelop data)

^3a5b41

A skin is considered the *most* superficial **surface** (perhaps at a given moment if the one skin is removed, the next layer would then be the *skin*).

Describe the complex **layers** of **data structures** (i.e. the ways in which data is organized, accessed, manipulated, and represented).
- Describes how data layers (such as [[Data Trees]]) **encapsulate** or envelop geometry or design logic.
- At the most abstract level, they are the visual representation of a hierarchical, nesting logic.
	- I.e. multi-dimensional data structures.
	-  Refers to an architectural or design concept describing the exterior or the outermost layer of a structure or object. 
	- A surface treatment of an object, or any other outer layer that defines the visible "appearance" (i.e. texture and sometimes the functional aspects of the designs).

In general a **skin** refers to [[Surface Creation|surface generation]], or generation of a set of surfaces.

[[#Skin and Pattern Generation Methods on an Input Surfaces NURBS Surface|Skins can be generated from a grid or pattern that is generated from a surface.]]

## Tri-dimensional Data
Refers to data that spans/encompasses three spatial dimensions, which are fundamental in describing objects or environments (i.e. geometries) in a 3D space. ^tri-dimensional-data
	1. Width
	2. Height
	3. Depth ^1b2d69

## How Data Structure [[Data Structures#^data-types-are-requirement-specific|Controls Output]]
Data structure in computational design fundamentally organizes and handles the information that defines a design. 

This organization impacts how data is accessed, manipulated, and ultimately visualized in the design process.

To achieve a specific output, the data is required to be structured in a specific way.
An example: Producing a *polyline* that connects twelve vertices.
- First, an algorithm is defined that uses four triangular surfaces (referenced in Rhino).
- Each surface is **deconstructed** using the **Deconstruct Brep** component to **extract** each Brep's vertices. 
- Then, a polyline is drawn to connect the vertices. 
- However, the result differs from the intended output.
	- The logic did not create a **single polyline** through the twelve vertices. 
		- Instead, the data structure defined four polylines each connecting three vertices. 
- **Why this happened**:
	![[Pasted image 20240330095930.png|600]]
	- [[Data Trees]] (i.e. the data structures utilized in Grasshopper), implement a **[[Data Trees#^parent-child-logic|Parent-Child Logic]]**.
		- This creates a **subset** for each **parent** [[Data Trees#^branch-data-path|branch]] (i.e. data path).
			- Therefore, in this *example* a **branching subset** was generated for **each triangular parent surface**, and an **item** was created for **each child vertex**.
				- That is, **each Parent sub-surface** created their own **set or list** of **Child nodes**.
					- The Child nodes represented the individual vertices of their respective Parent nodes (i.e. the triangular sub-surfaces).
			- ***Remember***: **Geometries are layers (i.e. skins) of abstractions - i.e. sets - of component elements.**
				- The Parent nodes are **sets** of vertices that represent one sub-surface from a list of sub-surfaces that is itself represented by a parent surface.
					- For example: The vertices of triangle 0 are contained within or represented by the parent branch with a data path of {0;0}, etc.
						![[Pasted image 20240330131943.png|400]]
					- Because of the [[Data Trees#^fundamental-rules-of-data-trees|the two fundamental rules of Data Trees]]:
						- A **Polyline** component cannot create a **single** polyline through the entire set of vertices, but four **different** polylines through the vertices of each branch.
	- The hierarchy of a this data structuring (Data Tree) can be viewed graphically as a **tree-chart**.
		- Where the subsets of the initial input "[[Data Trees#^4a4a93|root]]" are defined as **branches**.
			![[Pasted image 20240330132204.png|500]]

**Manipulation of Data Trees**: 
The ability to manipulate these data trees directly affects how design elements are generated, controlled, and varied. 

By modifying the structure of the data tree (such as reordering, grouping, or pruning branches), designers can achieve different patterns, forms, and complexities in their projects.
## [[Grids#The Pattern of Pattern Creation|Skin and Pattern Generation Methods]] on an Input [[Surfaces|NURBS Surface]]
Via Data Tree manipulation.
### Data Trees and Grid-Based Pattern Generation
The structure of data trees in the context of grids and pattern generation greatly enhances the designer’s ability to control and manipulate patterns on a granular level. 

This structured approach allows for sophisticated design techniques that are both responsive to design intents and adaptive to external conditions, essential in fields like advanced architecture and product design. 

The strategic organization of data within these trees directly impacts the effectiveness and efficiency of the design process, leading to outcomes that are both innovative and precisely engineered.
#### Hierarchical Organization of Grid Data:
##### [[Grids#1. Grid Definition/Formation on NURBS Surface (i.e. the initial set of edges)|Grids Definition]]:
A grid on a surface, such as a NURBS surface in 3D modeling software, is defined by a set of points or intersections (nodes). These points are organized within a data tree, where each branch might represent a row or a column of the grid, and each leaf node represents a point within those rows or columns.
##### [[Grids#3. c549e9 Transformation of the Extracted Edges|Extracted Edge Transformation Instructions]] (i.e. Pattern Instructions):
The manipulation of these nodes (moving, scaling, rotating) is stored as a set of instructions or operations within the data tree, which can be applied to generate complex patterns.
#### Flexibility in Pattern Customization:
##### Selective Editing: 
By accessing specific branches or leaves in the data tree, designers can selectively edit parts of the grid. For instance, one can target only the edges of a grid for transformation, leaving the interior points static, which results in a pattern that morphs at the boundaries but remains uniform centrally.
##### Complex Pattern Generation:
More complex manipulations, such as creating gradients or transitions in the pattern across the grid, are facilitated by adjusting how data flows through the tree’s branches. Parameters controlling these adjustments can be tweaked to refine the pattern iteratively.
#### Control Mechanisms via Data Trees
##### Parameter Linkages:
In parametric design tools, data trees enable linking of parameters across different parts of the design. For instance, the curvature of grid lines might be linked to environmental data such as sunlight or wind patterns, allowing the grid pattern to adapt dynamically based on environmental inputs.
##### Conditional Transformations:
Data trees allow for conditional transformations where certain conditions (like proximity to a certain point or alignment with an axis) dictate specific transformations. This conditional logic can be embedded directly within the tree structure, influencing the grid manipulation process based on predefined rules.
### Rectangular Based Pattern
^55e72e
*Example*:
- Creating a **[[Grids#Tri-dimensional Pattern|tri-dimensional]]** pattern from the **rectangular subdivision** of an input surface.   
	- The final output will be a set of **deformed pyramidal frustums**. 
	- The tri-dimensional pattern is created by **joining three different surfaces**:
		- Surface A: **Frame** the *pyramidal frustums*.
		- Surface B Form the **lateral faces** of the *pyramidal frustums*.
		- Surface C: Are the *pyramidal frustums'* **caps**.
			![[Pasted image 20240331004726.png]]
			- Curve set 1: The **extracted edges** of the sub-surfaces. 
			- Curve set 2: The **joined, offset polylines** of Curve set 1.
			- Curve set 3: The **exploded, offset polylines** of Curve set 2. 
			- Curve set 4: The **transformed (scaled and translated) polylines** of Curve set 3.
##### Surfaces A 
The [[Grids#1. Grid Definition/Formation on NURBS Surface (i.e. the initial set of edges)]] aka **frame** of the *pyramidal frustums*.
1. Set reference to a surface from Rhino, and then reparametrize the **Surface** "container" component
2. Feed the surface into an **[[Surface Analysis#^isotrim-subsrf-operation|Isotrim-SubSrf operation]]** (i.e. a **Divide Domain$^2$** component fed into a **SubSrf** component).
3. Feed the Isotrim-SubSrf operation output into a **Deconstruct Brep** component.
	1. (F): Are the sub-surfaces (i.e. the faces of the Brep).
	2. (E): The curves of the divided domain (i.e. the edges or "frames" of the Brep).
		![[Pasted image 20240402100523.png|400]]
4. The four edges of each sub-surface are joined, forming a polyline.
	1. The polyline is **offset** coincident to the set/referenced surface via the **Offset on Sfr** component.
		- The sub-surfaces generated by the **Deconstruct Brep** component are the input surfaces to be offset. 
		- The edges generated by the **Deconstruct Brep** component are the input curves to be offset. 
			- ###### Offset on Surface component:
				- Offsets a curve on a surface with a specified distance.
					- Inputs:
						- (C): Curve to offset.
						- (D): Offset distance.
						- (S): Surface for offset operation.
					- Outputs:
					- (C): Resulting offsets (curves).
			![[Pasted image 20240331012417.png]]
			![[Pasted image 20240331012433.png|400]]
5. The **offset joined polylines** must be **exploded** to define a **loft** operation between corresponding curves.  
	- The (S) output of the **Explode** component - that is the offset polylines, are then merged with the original edges of the Brep (from step 3.2).
		- The (D1) and (D2) inputs of the **Merge** component are required to be **[[Data Trees#^615489|grafted]]*** in order to correlate the data within the two corresponding sets. 
			- Meaning, the initial "flat" list containing two elements, the two "exploded" offset polylines, was grafted, creating a new Data Tree where each element/offset polyline is its own branch. 
				- This is also the case for the list of original edges of the Brep.
				- Therefore, when the two exploded, offset polylines and the original edges (Data Trees) are lofted, the offset polylines and the corresponding edges would be lofted together. 
					![[Pasted image 20240402000426.png]]

##### Surfaces B
The **lateral faces** of the *pyramidal frustums*.
- I.e. The lateral faces are defined by the exploded, offset polylines (Curve set 3 - relative to the original edges of each sub-surface), and a new set of curves that are defined by **scaling** and **moving** those offset curves. 
	- To define this new set of curves:
		- The midpoint of each sub-surface is calculated using the **Evaluate Surface** component, remembering to **reparametrize** the (S) surface input, and the *uv* input set via bi-dimensional slider at (0.5,0.5).
			- The (P) output of **Evaluate Surface** component calculates a set of points at the *uv* coordinates on the input (S) surface.
				- Therefore, it is a set of points approximately center (via bi-dimensional slider) of each of the sub-surfaces.
		- A **Scale** component is then utilized, with inputs:
			- (G) The geometry as the set of the exploded, offset polylines .
			- (C) Each [[Affine Transformations^center-of-scaling-point|center of scaling point]] of scaling is set to each extracted center point of each sub-surface. 
				![[Pasted image 20240402002158.png]]
- Next, the Curve set 3 are [[Euclidean Transformations#^a338b9|translated]] (i.e. moved) according to the **surface normals**, which are defined by the output (N) of the **Evaluate Surface** component.
	- The move/translation is defined and implemented via a scaling the surface normals by a negative scalar.
		- Then inputting that value into a **Move** component's (T) input.
			- The set of now scaled curves (Curve set 3 - the exploded, offset polylines) is the (G) input of this **Move** component. 
			- Because the surface normals were scaled negatively, the move is in the opposite direction of the surface normals. 
				- Finally, the output translated geometry is input as the (D2) input of a **Merge** component.
					- The (D1) input is the set of  exploded, offset polylines.
						- Creating a new Data Tree of paired exploded, offset polylines with a scaled and translated offset polyline.
							- Finally, the new Data Tree items of each branch, are lofted together.
								![[Pasted image 20240402003131.png]]
								![[Pasted image 20240402100351.png]]
##### Surfaces C
The **caps** of the *pyramidal frustums*. 
- I.e. The surfaces between the lateral faces.
	- They are defined by the Curve set 4 (the transformed Curve set 3). 
	- The four defining edges of a branch of Curve set are extracted via the **List Item** component. 
		- *Specifically, by "zooming in" on the **List Item** component and "adding" four output parameters.*
	- Then the extracted edges (Curve set 4) are input into an **Edge Surface** component.
		- **Edge Surface** component: Creates a surface from two, three or four edged curves.
			- Outputs:
				- (S) Surface Brep representing the edge-surface of the input curves/edges.
				![[Pasted image 20240402101631.png|400]]

##### Input Parameters
Are arbitrarily set defined manually or alternatively dependent on other parameters.
- *In this example, the parameters are the transformations (offset distance, the scale factor, the translation factor) and even the initial referenced curve and its sub divisions and frame size.*
- For example, an **[[Data Relationships#Attractor|attractor point]]** can be used to vary the offset distance that defines the frame's width. 
	- To create an attractor:
		- A point can be referenced from Rhino and extracted into a **Point** component.
		- The Distance is measured between the centers of the sub-surfaces (found via **Evaluate Surface** component using the (0.5,0.5) approx *uv* center coordinates), and the newly referenced attractor point. 
			- Because the calculated distances will be greater than the frame's width:
				- The numbers representing the distance between the attractor point and a centroid of a sub-surface (and therefore, the offset distance of the Curve set 2) need to be remapped such that the range of the numbers is within the defined domain of the frames.
					- I.e. remapped to the bounds of the width and height of the frames. 
						- In this example case, between 0.2 and 1.2. ^example-target-domain
				- A **Bounds** component can be used to output a (S) source domain input for a **[[Data Relationships#Remap Numbers component|Remap Numbers]]** component. 
					- ###### Bounds component: 
						- Creates a numeric domain which encompasses a list of numbers.
						- Inputs:
							- (N): Numbers to include in Bounds.
						- Outputs:
							- (I): Numeric Domain between the lowest and highest numbers in {N}.
					- The (T) target domain input is the set via [[#^example-target-domain|number sliders]] in this example. 
				- The output of the **Remap Numbers** component is the (D) distance input of a **Offsets on Surface** component.
					- This input from the **Remap Numbers** component was originally a numbers sliders.
					- The (C) curves to offset input is the Curve set 1. 
						![[Pasted image 20240402112444.png]]
		- Therefore, the **attractor point** influences the offset distance of the Curve set 2 and thus the frame itself.
			- The greater the distance between a centroid and the attractor point, the greater the offset distance of the edges of that sub-surface. 
			![[Pasted image 20240402113258.png|400]]


### Hexagonal based pattern

^ecb0e6

Creates a tri-dimensional pattern on a surface by means of a hexagonal subdivision.
![[Pasted image 20240409134212.png|400]]

### Responsive Façade Pattern


### Weaving Pattern




## Sorting Strategies Using the Data Tree
Sorting points is a step involved in generating a smooth surface from scattered points.

To achieve an intended output, the data needs to be structured in such a way that facilitates that outcome. 

Data Tree management components are used to implement this specified structuring.

*For example*: Generating a surface from a random distribution of points within a grid.
- Using the **Surface from Points** component.
- If the points are not organized in rows or columns, the resulting surface will generate unintended results, with possible twists, etc.
	![[Pasted image 20240402130330.png|300]]
- ###### A strategy to organize points into rows/columns:
	- Define the sequence based on each points coordinates.
		1. Sort the points according to the x-axis.
			- Producing 4 different columns of points.
		2. Sort the points inside every column according to the y-axis.
- ###### How to Sort Scattered Points:
	- ###### According to the x-axis:
		- I.e. The **Sort List** component sorts a list (in this case, of points), according to the keys (in this case, the x coordinates). 
		1. Points are distributed "randomly" within a 2D grid, i.e. in a scatter plot.
		2. Sort by x axis/x values: 
			1. Sort values along a "row" of values containing the same y coordinate. 
				- I.e. Sorting from "left" to "right" along the x-axis, a "horizontal" line. 
			1. "Draw" "vertical lines" passing through points of the same x values, but variable y values.
				- Each "vertical line" represents a column.
	- ###### According to the y-axis:
		- I.e. The **Sort List** component sorts a list (in this case, of points), according to the keys (in this case, the y coordinates). 
		1. Points are distributed "randomly" within a 1D column, i.e. in a scatter plot.
		2. Sort by y axis/y values: 
			1. Sort the values of the points along their respective "columns", which contain the same x coordinate.
				- I.e. Sorting from "bottom" to "top" along the y-axis, a "vertical" line. 

	2. Sorting points according to the x-axis:
		- ###### Sort List component:
			- Sorts a list of numeric keys.
			- Inputs:
				- (K): List of sortable keys.
				- (A): Optional list of values to sort synchronously. 
			- Outputs:
				- (K): Sorted keys.
				- (A): Synchronous values in A.
		- In this example it is used to sort a list of points according to each points position on the x-axis. 
			- The (A) input takes the list of points to rearrange.
			- The (K) input is defined by using the **Deconstruct** point component.
				- It Deconstructs a point into its separate x, y, z coordinates.
				- The x output is the data used to sort.
		- The result is:
			- A sorted left to right "row" of points that contain the same y coordinate.
			- A second sorted left to right "row" of points that contain the same y coordinate (different from previous row).
			- etc...
				![[Pasted image 20240402130430.png|300]]
		- The (A) output of **Sort List** component is a flat list of points.
		- Using the **Allocate N** component
			- Splits a flattened list into N elements per branches, computing the correct number of branches according to a specified N elements. 
			- Inputs:
				- (D): Data to be restructured.
				- (N): The number of index items per branch.
			- The data is then restructured into 4 branches, with 6 index elements per branch.
				![[Pasted image 20240402125200.png|500]]
				![[Pasted image 20240402125232.png|200]]
	2. Sort the points inside every column according to the y-axis:
		- The output of the **Allocate N** component is structured into four branches (i.e. columns), each containing six elements (i.e. points).
		- This output Data Tree is then input into another **Deconstruct** point component.
		- Finally, the y output of the **Deconstruct** point component is then input into the (K) keys input of another **Sort List** component. 
			- I.e. The Data Tree is then sorted according to the y-axis.
				![[Pasted image 20240402130231.png|400]]
				![[Pasted image 20240402130158.png|200]]
	- The points organized sequentially with respect to the x and y coordinates can be used to define a surface by means of the component, **Surface from Points**.
	- **Surface from Points**:
		- Inputs:
			- (P): Grid of points.
			- (U): Number of points in the *u* direction.
			- (I): Interpolate samples.
		- Outputs:
			- (S): Resulting surface.
		![[Pasted image 20240402130949.png]]
		![[Pasted image 20240402131002.png|400]]
