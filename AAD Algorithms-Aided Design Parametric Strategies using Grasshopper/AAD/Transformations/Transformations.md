---
up:
  - "[[Data Relationships]]"
related:
  - "[[Points]]"
  - "[[Numbers]]"
  - "[[Parameters]]"
  - "[[Surfaces]]"
  - "[[Curves]]"
date created: 2024-03-27
---
# Transformations
## I.e. Change
### Measures the change between two points *P(x,y)* and *P'(x',y')*:
 - For example:
	 - To **translate** a **point** to a different **position**, a specific **quantity** is required to be added or subtracted from its original coordinates.
		 - That quantity being: the **change** in the **x coordinate** and the **y coordinate**. 
	- An entire object can be translated performing the pervious transformation to all its points or, more simply, to its vertices.
		- Therefore, a point reaches a new position by **moving** a **specific distance**, **in** or according to a **specific direction** and **sense**. 

	- #### Therefore, a translation is defined by a **starting point** P and a **translation vector** *v*. 
		- *See* [[Vectors]]
			![[Pasted image 20240327225122.png|500]]
## Types of Geometric Transformations:

### [[Euclidean Transformations]]
Preserve lengths or angle measures.
- Include translations, rotations and reflections.
### [[Affine Transformations]]
Do **not** preserve lengths or angle measures. 
- Include scaling, shearing and projections.
### Other Transformation
More complex transformations can be performed by combining transformations or by specific components such as the **Morph** component.

| Transformation | Maintain                  | Does NOT maintain      |
| -------------- | ------------------------- | ---------------------- |
| Euclidean      | shape, size               | position               |
| Affine         | parallelism               | shape, size, position  |
| Similiarity    | shape                     | size, position         |
| Morph          | topological relationships | geometrical properties |
![[Pasted image 20240327140235.png]]

1. Original geometry
2. 2. Euclidean transformation: rotation
3. Affine: Scale
4. Similarity: Scale and Rotation
5. Morph


## Proportions of the Numbers that Determine a Transformation Are Important
Just like the **proportions** of the **compositional elements** of a geometry, the proportions of the **sequences of numbers** that represent scaling factors, move distances, twist and relative angles, etc. are **critical**. 