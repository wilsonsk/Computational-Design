---
up:
  - "[[Data Management]]"
related:
  - "[[Data Operations]]"
  - "[[Data Trees]]"
  - "[[Data]]"
  - "[[Numbers]]"
  - "[[Abstract Concept]]"
date created: 2024-03-30
---
# Data Structures
Are the **underlying mechanisms** that **facilitate** [[Data Management#^c60676|data abstractions]].
- Different types of these mechanisms support specific types of requirements of the compositional data (i.e. elements). ^data-types-are-requirement-specific

## Types of Data Structures
- ###### Primitive Data Structures/Types:
	- The basic mechanisms that  **represent** and **manage/store/operate** directly on the fundamental (usually numerical) values.
		- I.e. a numerical value like the number "2" *is* in and of itself a **primitive data structure**. 
- ###### Composite (i.e. compound) Data Structures:
	- Are the structures that are **composed** of the primitive data structures/types. 
	- Consists of:
		- **Linear Data Structures**: Data elements are arranged in a linear sequence where each element has a single level of hierarchy associated with it. ^linear-data-structures
			- I.e. Set of singular elements.
				- Arrays
				- Linked Lists
				- Stacks
				- Queues
		- **Non-linear Data Structures**: Data elements are **not** arranged in a linear sequence, and they may have multiple levels of hierarchy. ^non-linear-data-structures
			- I.e. Set of sets.
				- Trees
				- Graphs
- ###### Abstract Data Types:
	- More conceptual data structures that are defined by their behavior from the point of view of a user.
		- Such as operations that can be performed on them and their properties.