---
up:
  - "[[Data]]"
related:
  - "[[Data Trees]]"
  - "[[Data Control]]"
  - "[[Data Relationships]]"
  - "[[Numbers]]"
  - "[[Elemental Building Blocks]]"
date created: 2024-03-18
---
# Data Operations
## Generating Numbers : ([[Data Trees#Lists|Lists]])
### Series component: 
###### Often used with the transformation components (i.e. move) - creates "[[Vectors]] sequences": 
- Generates numerical sequences according to:
	- (S): first number in series
	- (N): "step/increment" size between each subsequent number
	- (C): the number of steps (between numbers) in the series
### Random component:
###### Generates a list of (N) numbers within a defined numeric domain (R):
- (S) input specifies the seed value of the component. 
	- if the seed values is changed while holding all other inputs the same, a new list of values will be generated.
### Construct Domain component: 
###### Used to define a numeric set (a [[number-system]]) existing within two numeric extremes (a min and a max value).
- (A): min value of domain
- (B): max value of domain
- to change domain space from integer, or real number: edit the component values via right click
### Range component: 
###### Defines a range of numbers within:
- (D): numeric domain
- (N): equal subdivisions ("steps") between the min and max of the domain
- **Outputs**: A list
## Selecting Data: 
### List Item component:
Retrieve a (one) specific item from a list.
- Inputs:
	- (L): Base List.
	- (i): Item index to be selected.
	- (W): Wrap index to list bounds.
- Outputs:
	- (i): Item at (i) input.

### Merge component:
Mergers multiple data streams (lists and Data Trees).
	**Inputs**:
	- (D1): Data Stream 1.
	- (D2): Data Stream 2.
	**Outputs**:
		(R): Result of merge.
###### Selects two or more items
## Filters: 

### Cull-Index component:
###### Performs reverse function of the **List Item** component.
- It deletes the specified index items from a list.
### Cull Pattern:
###### Filters *lists* according to a repeating pattern of Boolean values.
Removes elements in a list using a repeating bit mask.
- Inputs:
	- (L):  List to cull.
	- (P): Culling pattern.
- Outputs:
	- (L): Culled list.

### Shift List component:
###### Shifting items in a list.

### Split List component:
###### Modifying list length at specific index.

### List Length component:
###### Get list length.

### Reverse List component:
###### Reversing order of list.

### Repeat Data component:
###### Extends a numeric sequence to a specified length by repeating the input data (looping).
- The output of the Repeat Data component can be used to define sequential geometry.
## Data/Input Matching: ^data-matching
###### A set of consistent **rules for how components "lace" or match** the data/inputs across multiple inputs to a component.
- For [[Data Trees]] aka **Lists of Lists**:
	- ==*Remember*: a **Branch** is a **List** of the **initial** list or tree.==
		- ==I.e. The **first level** of a **Data Tree** is an **initial** list of **branches** (i.e. **elements** of the initial list that are themselves **also lists**).==
		- ==General **behavior**:==
			- ==Matches **Branches** into pairs.==
				- ==Matches **items** (of branches) into pairs.==

#### M : 1
- ##### *M* list elements : 1 list element - (i.e. Non Data Trees) 
	- A **single step** process.
	- The **1 length list item** is matched with **each** of the ***M* items** (from the "M" length list).
		- Generating a **new list** of ***M*** paired **items**.
			![[Pasted image 20240326133712.png|400]]
- ##### *M* Data Tree Branches : *1* Data Tree Branch
	- A **multi step** process:
	1. The **single branch** (of the "1"data tree) is matched with **each** of the ***M* branches**.
		- Generating ***M* new paired branches**.
		![[Pasted image 20240326134259.png|400]]
	2. Next, **each ith List Elements** from each of the ***M*** **paired branches** are **matched**.
		- Generating a **new Data Tree of *M* branches**.
		![[Pasted image 20240326135242.png|400]]
#### N : N
- ##### N list elements : N list elements - (i.e. Non Data Trees) 
	- Each ***ith* indexed item** (i.e. element) of the **first list** is paired/matched/laced with **corresponding *ith* indexed element** of the **second list**.
		- Generating a **new list** of *N* **paired items**.
			![[Pasted image 20240326133744.png|400]]
- ##### N Data Tree Branches : N Data Tree Branches 
	- A **multi step** process:
	1. The **ith indexed BRANCH** of the first Data Tree is paired with the **corresponding ith indexed BRANCH** of the second Data Tree.
		- Generating a ***M* new paired branches**.
			![[Pasted image 20240326140052.png|400]]
	1. Next, the **each ith Branch (i.e. list) element (i.e. item)** is paired with the **corresponding  ith Branch (i.e. list) element (i.e. item)**.
		-  Generating a **new Data Tree with N paired branches of paired elements**.
			![[Pasted image 20240326150240.png|400]]

#### N (items) : M (items) - **NOT a Good Operating Procedure**
- ##### Shortest List: 
	- Matches each item of 1st list with the corresponding item of 2nd list. Then slices the longer list to the same length as the shorter list.
- ##### Longest List (default): 
	- Matches each item of 1st list with corresponding item of 2nd list. 
	- Then the last item of the shorter list will be matched repeatedly with each remaining item of the longer list.
- ##### Cross Reference: 
	- Matches each item of the 1st list with each and every item of the 2nd list. 
	![[Pasted image 20240326133239.png|500]]

