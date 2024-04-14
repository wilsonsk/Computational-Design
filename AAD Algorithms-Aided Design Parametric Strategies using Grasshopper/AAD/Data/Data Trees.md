---
up:
  - "[[Data Management]]"
related:
  - "[[Data Control]]"
  - "[[Data Relationships]]"
  - "[[Numbers]]"
  - "[[Data Operations]]"
date created: 0202-03-27
---
# Data Trees
In Grasshopper, data is managed according to the hierarchical structure of the Data Tree.

A **Data Tree** is a hierarchical, nested (i.e. multi-dimensional) [[Data Structures#^non-linear-data-structures|non-linear data structure]] used to **organize** and **manage** (i.e. control, access and manipulate) and **represent** **data**.

It can be thought of as a "**list of lists**" that **enables complex relationships** among its **compositional elements** and **facilitates** easier **management** (access, manipulate and control) the **internal data**. 

**It consists of**:
- ###### Nodes (i.e. vertex): Represent the data - that is the elements, or items stored within the Data Tree.
	- This data include geometry information encoded as **numerical values**.
- ###### Edges: Represent the relationships or connections between nodes.
	- They represent the **structure** of the Data Tree thereby **defining** the **Parent-Child logic**.
- ###### Parent-Child Logic: A flow of dependency between nodes. ^parent-child-logic
	- **Child node**: Is node-dependent on its associated Parent node.
		- The child in some way relies on the relationship with its parent node for information.
	- **Parent Node**: Is either node-dependent on its Parent Node or node-independent and is therefore a root.

**Implementational Structure**:
0. **Root**: The **starting point** of the Data Tree, therefore has no parent node.  ^4a4a93
1. **Branch**: A "watertight" subset of the root. ^branch-data-path
	- *Watertight* meaning **connections** between **data** within **different branches** cannot be established. 
	- A **branch** represents a **dimensional element** that is a **list** (i.e. data path) and **not** a simple **numerical** **value**. 
	- I.e. A branching subset.
1. **Leaf**: A terminal node, therefore has no children nodes.
	1. It represents a **single element** that is a simple numerical value.  
![[Pasted image 20240330101946.png|]]

## Two Fundamental Rules of Data Trees ^fundamental-rules-of-data-trees
1. Branches are watertight sets.
	- Any **operation** performed on a Data Tree will **affect** the **data** stored in **every branch**.
		- I.e. Branch level operations
			- For example:
				- A **Polyline** component cannot create a **single** polyline through the entire set of vertices, but four **different** polylines through the vertices of each branch.
1. Data Trees can be **manipulated** to generate **specific results**.
	- For example: 
		- To create a polyline through a set of twelve points, the Data Tree must be manipulated via a set of specific components. 
## Data Tree Operations/Manipulations
*See [[Data Operations#^data-matching|Data Matching/Lacing]]*

### Flatten Tree component/operation
("Many to 1")
Simplifies a Data Tree by **removing all branching information** and storing all the data inside the **root**. 
- I.e. **Eliminates each branch** and reorganizes each element of each branch into a **single** node-independent branch (i.e. the root).
- Should resist being utilized unless absolutely necessary as it destroys the original branching structure.
	- *A dashed wire indicates "structured" flow of data, while continuous line indicates a "flattened" flow of data.*
	![[Pasted image 20240330193242.png|400]]
	- The **Unflatten Tree** component can convert a flattened list (T) into a Data Tree according to a *guide* Data Tree from which it references its branching structure.
		- The **Unflatten Tree** component only operates *if* the flattened list has the same *data* as the guide list (i.e. data type like points, curves, etc.).
### Graft Tree component/operation 
("1 to many") ^graft-data
Creates a branch for every item within an arbitrary list.  ^615489
- So a flat list with *N* items that is **grafted** returns a **new list** with *N* branches, that is one branch for each list item.
- The **Graft Tree** component can be used to match disconnected sets of corresponding objects. 
	- For example: Lofting surfaces from 
		- Two surfaces (referenced from Rhino) are connected to two **Deconstruct Brep** components to access each surfaces' edges. 
			- The two outputted lists of edges are then individually **grafted** to produce two new Data Trees with branches for each edge of the original lists. 
			- The **Merge** component is then used to combine the two new Data Trees into one Data Tree.
				- Via **N to N** [[Data Operations#^data-matching|data matching]].
					- This results in a *pairing* of ith branches into one branch containing elements of each of the ith branches. 
			- The **Loft** component can now loft surfaces from the *paired* edges of the new branches. 
				![[Pasted image 20240330211810.png|500]]
				- If **not** grafted, the Lofting will be applied to the entire flat list of edges in the sequence of:
					- Each edge of the first Brep (a, b, c, d, ...) then each edge of the second Brep (a', b', c', d', ...).
						![[Pasted image 20240330212145.png]]
### Shift Paths / Trim Tree
"Shifts" paths **"safely"**.
- Does this by **flattening** or **trimming** **only** a given index (i.e. offset) of each branch.
	- I.e. adjusts the branch indices of each branch in the Data Tree.
		- The amount of shift is determined by the input (A).
			- A positive amount shifts the paths "upwards", thus increasing their indices.
			- A negative amount shifts the paths "downwards", thus decreasing their indices.
- Effect on List items of *shifted branches*:
	- The affected items are not changed value wise or moved in terms of their content order/sequence.
	- What changes is their branch path or address that represents their position within the Data Tree. 
- The Data Tree is reorganized, but the integrity and sequence of the list items within each branch remains intact.
### Flip Matrix component
Swaps **rows** and **columns** in the **matrix-like** Data Tree.
- I.e. Swaps **items with branches** and **branches with items**.
	- *For example*:
		- Three circles input into a **Divide Curve** component (dividing each curve 10 times).
			- Generating a Data Tree of three branches representing the three circles.
				- Each branch containing 10 points corresponding to the **Divide Curve** component.
		- The **Flip Matrix** component takes that Data Tree and produces:
			- A Data Tree containing 10 branches.
				- Each branch contains three points. 
					![[Pasted image 20240331000234.png|500]]