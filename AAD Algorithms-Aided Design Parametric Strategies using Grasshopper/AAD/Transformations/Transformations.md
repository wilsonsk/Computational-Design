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
## [[Secant Line|Measures the change]] between two [[Points|points]] *P(x,y)* and *P'(x',y')*:
 - For example:
	 - To [[Euclidean Transformations#Generative Point Transformations|translate a point]] to a different **position**, a specific **quantity** is required to be added or subtracted from its original coordinates.
		 - That quantity being: the **change** in the **x coordinate** and the **y coordinate**. 
### Point to Curve: 
A point in a parametric setting could be seen as the simplest form of a parameter—essentially, a position in space defined by coordinates.

This is kinematics - that is calculus.
[[Components of Motion]]
[[Uniform Motion]]
[[Linear Motion]]
[[Non-Linear Motion]]
[[Kinematics Analysis]]
#### 2D Transformation of a Point:
In a 2D space, transforming a single point involves manipulating it across the plane to create a series of new points. 

When these points are connected, they form a curve or a line. 

This transformation can be governed by mathematical functions or parametric equations where the point's new position is a function of variables like time or another parameter.
	If a point moves along a path defined by the equation $y=f(x)$, where $f$ is any function (linear, polynomial, sinusoidal, etc.), the trail of the point forms a curve which can be graphically represented.
#### 3D Transformation of a Set of Points (i.e. a Line or Curve):
A line or a curve—a set of points ordered in one dimension—can be transformed to populate a surface. 

 Consider a curve in 3D defined parametrically as $(x(t),y(t),z(t))$. 
	 By applying another parametric function that modifies these coordinates, say $x(t)→x(t)+u,y(t)→y(t)+v,z(t)→z(t)+w$ where $u,v,w$ are functions of another parameter $s$, you generate a surface. 
		 This surface can be visualized as a set of these transformed curves, each representing a 'snapshot' of the curve at a different state.

An entire object can be translated performing the pervious transformation to all its points or, more simply, to its vertices.
- Therefore, a point reaches a new position by **moving** a **specific distance**, **in** or according to a **specific direction** and **sense**. 
#### Therefore, a translation is defined by a **starting point** P and a **translation vector** *v*. 
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