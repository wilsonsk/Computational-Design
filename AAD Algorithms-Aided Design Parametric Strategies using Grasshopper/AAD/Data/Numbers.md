---
up:
  - "[[Data]]"
related:
  - "[[Data Control]]"
  - "[[Data Operations]]"
  - "[[Data Relationships]]"
  - "[[Elemental Building Blocks]]"
  - "[[Points]]"
  - "[[Parameters]]"
  - "[[Data Trees]]"
  - "[[Number Systems]]"
date created: 2024-03-18
---
# Numbers
## Numbers are **abstract mathematical objects**.

Numbers are **fundamental data elements** as they **serve** as the primary means through which **[[Data]]** **is** **quantified** ([[Parameters]]), **[[Data Operations]] are performed** and **[[Data Relationships]] are defined**.

Numbers represent a **language** (via **MAPPING**) through which aspects (of a design or object) can be described, analyzed, and realized. And thus, are the **FOUNDATIONAL** elemental building block through which higher level blocks are composed and interacted with (i.e. handled). 

We **apply** numbers to aspects of experience that we want to interact with at some level. That is, measure, control or manipulate.

## **Domain**:
^domain
#### The area or **bounds** of a range of data.

Is simply, the **set**, or **defined min and max values** between which other values of that domain are contained. 

##### **Quantification of Properties:** **Mapping** via units
1. Numbers **facilitate** the **measuring** of physical **properties** and design parameters such as dimensions, angles, distances and material properties via a **mapping of units to the geometrical aspects of an object**
2. **Understanding how [[Number Systems]] MAP to Geometrical Systems**
	1. **Unified Scaling** ([[unitization]]):
		1. **Normalization**: reparameterization of scale
			1. This is where we map a domain ([[number-system]]) of numbers to 0-1, which unifies its scale with any other element that is also mapped to 0-1
				1. this means that 50% of one element still means 50% when applied to another element. 
					1. before mapping to 0-1 a **curve** of say length *588* has a half way point represented by *294*, not represented by *0.5*
					2. *see* [[Curves#^linear-interpolation]] *for a more in depth understanding (why this effects curves and not lines, etc.)*
##### **Data Representation**: [[Data Trees#Data Structures|Data Structures]]
1. **SETS** of [[Elemental Building Blocks]] are constructed in Grasshopper via [[Data Trees#Lists|Lists]] and [[Data Trees#Data Structures|Data Structures]]. And as follows, the composition of sets of these data structures represent or compose design elements, aspects or components of an object. 
	1. For example a point in space is **represented** by (i.e.. mapped to) a set of **numbers** (coordinates)
	2. **Numbers** enable to **storage**, **retrieval** and **manipulation** of this **data** within **computational** **systems**.
##### **Defining Constraints**: i.e. defining [[Data Relationships]]
1. Mathematical equations are used to **constrain** relationships between numbers (correlations). 
##### **Algorithmic Operations**: [[Data Operations]]
1. algorithms are used to generate, modify and analyze designs (i.e. the relationships between components)