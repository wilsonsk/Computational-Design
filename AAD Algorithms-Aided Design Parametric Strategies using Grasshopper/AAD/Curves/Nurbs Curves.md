---
up:
  - "[[Curves]]"
related:
  - "[[Bezier Curves]]"
date created: 2024-03-19
---
# NURBS Curves
Are [[Continuities|continuous]].

NURBS curves can exhibit different levels of [[Continuities|continuity]]:
###### C0 Continuity (i.e. Position Continuity): 
This is the basic level of continuity where the curve is continuous, but there might be a visible corner where segments meet.
###### C1 Continuity(i.e. Tangent Continuity):
At this level, not only the curve but also the first derivative (the tangent) is continuous across segments. This means there are no visible corners, and the curve appears smooth.
###### C2 Continuity (i.e. Curvature Position Continuity):
Here, the curve, its first derivative, and its second derivative (curvature) are continuous. This level of smoothness is especially important in automotive and aerospace applications where the flow of a surface needs to be extremely smooth.
## **N**on-**U**niform **R**ational **B**-**S**plines:
Are mathematical representations of 3D geometry that can accurately describe any shape from a simple 2D line, circle, arc or [[Curves]] to the most complex 3D organic free-form surface or solid.

They exist to enable curves control polygons can be **taken through perspective projection** and the **curve computed afterwards**.
- **To do this**: NURBS introduce and define **weights**.
## A **NURBS curve** is a mathematical expression represented by a curve:
**Defined** by its **degree** (a set of a weighted control points, a knots vector and an evaluation rule):
## Degree:
A positive integer number
- Example:
	- NURBS **lines**, and NURBS **polylines** are **degree 1**
		- A degree 1 curve coincides with its control polygon (i.e. a line connecting consecutive control points)
	- NURBS **circles** (and circles, parabolas, hyperbolas and ellipses) are **degree 2**
	- Most **free form** curves are **degree 3 or 5**
- The value equal to degree+1 is called the **order**.
## Control Points:
A NURBS curve is constrained by the **position** and **weight** of control points.
- **Weights**: regulates the attraction between the control points and the curve.
	- a weight > 1 attracts the curve and a weight between 0-1 repels the curve.
- The **number** of control points **cannot** be smaller than order (degree+1).
## Knots: 
A list of (degree+N-1) numbers, that control the **smoothness** of a curve.
##### Evaluation Rule:
Is a formula that:
- **Inputs** degree, control points, and knots.
- **Outputs** a point location.
## NURBS Curve component
Constructs a NURBS curve from control points
Inputs:
- (V): Curve control points - i.e. vertices.
- (D): Curve Degree.
- (P): Periodic Curve (Boolean).
Outputs:
- (C): Resulting NURBS Curve.
- (L): NURBS Curve Length
- (D): NURBS Curve Domain.
## Parametric Representation of a NURBS Curve:
### World Coordinate System (WCS):
In Rhino 3D, the environment is based on a WCS.
- Points on a NURBS curve are defined b (x, y, z).

If *z=0* then the curve is a **planar** curve and is defined by the coordinates (x, y).
![[world coordinate system.png|400]]

![[planar curve 1.png|400]]

**Another way** to find points on a curve is based on the **Parametric representation.**
### Local Coordinate System: 
A **system** set **on** the curve itself. 

The **advantages** as it requires just **one parameter** to **identify** a point, which is still **defined** in the **World Coordinate System**.
- The coordinates of an arbitrary point *P* are expressed as a function of a variable *t* that ranges between 0 and 1. 
	- *t* is a **scalar**.
	- When a curve's end points are represented by 0 and 1 respectively, this is unitization or reparameterization as detailed in [[Numbers]].
	- I.e. the curve is said to be "parametrized" between 0 and 1 or alternatively, that is **domain** is *[0,1]*.
	![[lcs.png]]
- **Important:** *t* does **NOT measure distances**.
	- *t* represents **time** that a particle takes to move from t=0 to the position marked by *p(t)*. 
	- This **time** is affected by the **position** of **control-points**, and specifically the **motion** of the the *particle* **slows** down when it passes though a **concentration** of control points.
		- For this reason *t=0.5* is not the parameter that specifies the curve's **midpoint**. 
			![[Pasted image 20240323002953.png]]
			- Even if the curve is **rebuilt** with uniform redistribution of control points, the mid point is not coincident with the point corresponding to *t=0.5*. ^65f47a
## Analysis of Curves in Grasshopper:
Components, logics, and strategies to control NURBS curves using Parametric Representation. 
#### Finding points on a curve: 
- **Evaluate Curve** component
	- **Inputs**:
		- **(C):** a curve to be evaluated.
		- **(t):** a parameter **on the curve domain** to evaluate.
	- Parametric Representation **assumes** that a **curve** is **parametrized** between 0 and 1.
		- But curves in Rhino typically do have different domains.
		- The domain of a curve can be **set** to a domain of [0,1] via **reparametrizing** the curve. 
	- **Outputs**:
		- **(P):** points *location* in the World Coordinate System
		- **(T):** the **tangent** vector at *t.*
			- It is a **unit vector**.
			- Can use **Display Vector** component to visualize the tangent vector and can be scaled using the *multiplication* component.
#### Inverting the curve direction: 
Swapping start and end points. 
- Via **Flip Curve** component.
	- **Inputs**:
		- **(C):** curve to be flipped.
		- **(G):** a reference curve used to unify the direction of the set of curves.
#### World to Local Conversion:
- In Rhino set points are expressed in the **WCS**.
- **Curve CP** component: 
	- Is use to convert a point expressed in the **WCS** to the **LCS** - that is, to the local *t* the **local parameter**. 
		- **(t) output:** is the parameter on the curve's domain expressed in the **Local Coordinate System.**
	- It also enables users to find the **closest** point *p* on a curve given an **external** point *P*. (I.e. secondary functionality)
		- **Inputs:**
			- **(P):** an **external** point relative to the curve. 
			- **(C):** a curve containing a point to be found. 
		- **Outputs:**
			- **(D):** the displacement distance between points *p* and *P*. 
		- When Curve CP is used to convert from WCS to LCS: *p* = *P* and *D = 0*.
- **Point on Curve** component:
	- Can be used to find points at specific locations of a curve (*start, quarter, mid, etc.*)
	- The specific locations are based on the curve's **length** not on the curve's domain. 
	- Does not require the input curve to be reparametrized.
- **Evaluate Length** component:
	- Finds a point *P*, a distance measured as an arc length **(L)** from the start point *t=0*.
	- **(L):** is a number between 0 and the curve's length - which can be calculated using he component **Curve Length**.
	- **(P):** This component outputs coordinates in the **WCS**.
	- **(t):** This component also outputs coordinates in the **LCS**.
- **Divide a curve**:
	- **Divide Length** component:
		- Divides a curve into segments specified by the arc length **(L)**.
		- If the curve's length is not a multiple of **(L)**, a "left-over-arc" with a different length from (L) will result. 
	- **Divide Distance**:
		- Divides a curve into segments by calculating sequential intersections of circles and the curve. (i.e. radii)
		- Depending on the value of the radial distance (**D**) a "left-over" arc will result having a distance PE different from (D).
	- **Contour** component:
		- Creates a set of curve contours given a curve (**C**), a start point (**P**), and a distance (**D**). 
		- The resulting intersections are output as a point coordinates in the WCS (P) as well as in the LCS (t).
## Notion of Curvature for planar curves:
The curvature of a planar curve *c* measured at point *P* calculates the **deviation** from *c* from its tangent line near *P*. 
###### Planar Curve
Essentially a 2D (i.e. bi-dimensional) curve.
It lies completely within a single plane.
	This means that no matter how the curve twists or turns, every point of the curve is contained within a single plane.
###### Non-Planar Curve
A curve that does not lie entirely within a single plane.
This type of curve has a 3D (i.e. tri-dimensional) form and cannot be fully represented on a 2D surface without distortion. 

The curvature of a *generic* curve varies from point to point. In order to mathematically define the curvature there are two basic **assumptions**:
	1. The curvature of a straight line is zero at every point.
	2. The curvature of a circle is **constant**. I.e. the curvature is equal to zero when the **radius** approaches **infinity**- that is a straight line is a circle with an infinite radius. 

Therefore, the curvature *k* can be **defined** as the **reciprocal of the radius** *r*:
- **k = 1/r**
- *k* is always "positive" because the quotient always involves two positive numbers. 
- However, **signed curvature** convention denotes a positive sign if the direction of the curve is along the clockwise direction of the **osculating circle** ([[Curves#^01ae23|Osculating Circle]]), and has a negative sign if the curve's direction lies along the counter clockwise direction of the osculating circle. 
	![[Pasted image 20240323094238.png|400]]

Curvature can also be **defined** as the **vector** *k* with direction *PO* and a magnitude equal to reciprocal of the osculating circle's radius. (where *P* is a point on the curve and the circle's circumference, and *O* is that circle's center)
- *k* is the **tangent vector**. 
	![[Pasted image 20240323092558.png|500]]
- **Curvature** component:
	- Graphically displays the curvature **vector** *k* and the osculating circle t a generic point *P*.
	- It is expressed in the Local Coordinate System. 
	- The curve's curvature value can be calculated in one of two ways:
		- As the reciprocal of the radius of osculating circle (C) - which is obtained via the (R) output of the **Deconstruct Arc-DArc** component. 
		- As the magnitude of the **vector** *k* which can be calculated via the **Vector Length** component. 
###### Deconstruct Arc-DArc component
Retrieve the base plane, radius and angle domain of an arc. 
- Inputs
	- (A): Arc or Circle to deconstruct.
- Outputs
	- (B): Base plane of arc or circle.
	- (R): Radius of arc or circle.
	- (A): Angle domain (in radians) of an arc. 

**Curves on a surface**: [[Surfaces#^parametric-representation-of-a-surface|Parametric Representation of Curves on a Surface]]
## Closed NURBS Curves
A NURBS curve that **connects back to its starting point**.
	Forms a continuous loop.
	
When a NURBS curve is 'closed,' it means that its start and end points are coincident, and the segments between control points around these ends smoothly transition into each other, creating a seamless boundary. 

