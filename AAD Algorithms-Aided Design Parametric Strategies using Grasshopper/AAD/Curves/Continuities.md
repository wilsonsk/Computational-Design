---
up:
  - "[[Curves]]"
related:
  - "[[Discontinuities]]"
  - "[[Limits]]"
  - "[[Derivatives]]"
  - "[[Parametric Space]]"
  - "[[Geometric Space]]"
date created: 2024-04-25
---
# Continuities
*See reference [video](https://www.youtube.com/watch?v=Cks7nA296v8&t=192s&ab_channel=CMUPDET)*
## Curvature
Is the geometric measure of how fast a curve is changing direction at a point. 
	It qualifies the deviation of the curve from being a straight line. 
		The curvature $k$ of a curve at a point gives an idea of the circle's radius (i.e. the **osculating circle**) that best approximates the curve at that point. 
			The smaller the curve, the greater the curvature.
### [[Notion of Surface Curvature#In order to **define the curvature** of a surface, the **osculating circle** needs to be defined.|Osculating]] Circle
A circle at a point on a curve is the circle that best approximates the curve near that point.
It "kisses" (i.e. is tangent to) the curve at the point.
	Therefore, it has the **same tangent line as the curve at that point**.
	Has a **radius** ($r$) that is the **reciprocal of the curvature** at that point ($r=1/κ$).
## Continuity: (i.e. when curves join)
![[Pasted image 20240425140151.png]]
A curve or surface can be described as having $G_n$ continuity.
	*n* being the increasing measure of smoothness.
	
Continuity has different behavior with respect to:
### [[Parametric Space]]: Differential Continuity, *C* 
- if a curve is **connected**: it has *C0* continuity.
	- if its first derivation is continuous: the original curve has *C1* continuity.
	- if the *nth* derivation is continuous: the original curve has *Cn* continuity.
- *C* continuity does **not** mean that a curve is geometrically smooth.
### [[Geometric Space]]: Geometric Continuity, *G* 
If a curve has *C0* continuity: it is *G0* continuous- it is connected and this means the same thing in both parametric and geometric space.
#### Derivatives and Continuity
###### G Continuity Adjacency Analysis in Terms of [[Derivatives|Derivatives]]
$G$ continuity describes how smoothly two surfaces or curves join together at a boundary. 
	The levels of $G$ continuity—$G0$, $G1$, and G2$—indicate increasingly stringent conditions on the matching of [[Derivatives|derivatives]] at the connection point.
##### Matching Derivatives
Refers to the process of ensuring that the derivatives of two functions are equal at a given point. 

This concept is fundamental in calculus and is used to ensure smooth transitions between functions, surfaces, or curves. 
	Matching derivatives at a point ensures that the functions share certain properties (such as [[Components of Motion#Position|position]], [[Slope|slope]], and [[Notion of Surface Curvature|curvature]]) at that point.
###### Levels of Matching Derivatives
1. **Matching Function Values ([[#$G_0$ Continuity (i.e. Position Continuity)|Positional Continuity]], $G0$)**:
    - **Definition**: The functions have the same value at a particular point.
    - **Mathematical Expression**:
        $$\LARGE f_1(c) = f_2(c)$$
    - **Meaning**: The two functions intersect at the point $\LARGE x=c$, ensuring that the positions match.
2. **Matching First Derivatives ([[#$G_1$ Continuity (i.e. Tangency Continuity)|Tangential Continuity]], $G1$)**:
    - **Definition**: The functions have the same first derivative (slope) at a particular point.
    - **Mathematical Expression**:
        $$\LARGE f_1'(c) = f_2'(c)$$
    - **Meaning**: The slopes of the tangent lines to the curves represented by the functions are equal at $\LARGE x=c$, ensuring that the direction of the curve is continuous.
3. **Matching Second Derivatives ([[#$G_2$ Continuity (or Curvature Continuity)|Curvature Continuity]], $G2$)**:
    - **Definition**: The functions have the same second derivative (curvature) at a particular point.
    - **Mathematical Expression**:
        $$\LARGE f_1''(c) = f_2''(c)$$
    - **Meaning**: The curvature of the curves is the same at $\LARGE x=c$, ensuring that not only the direction but also the rate of change of the direction is continuous.

![[Pasted image 20240425135811.png]]
![[Pasted image 20240429141001.png]]
#### $G_0$ Continuity (i.e. Position Continuity)
##### Continuity Type
##### Position
![[Pasted image 20240425164702.png]]
Position (G0 continuity) measures location only. 
If the end points of each curve are in the same location in space, the curves are position continuous (G0) at the ends. 
	I.e. The two curves in question touch each other at their end points.
The curves touch at the join point (position).
The simplest form of continuity, G0, signifies that the sections meet but may not be smooth or aligned. 
If a curve is *G0* continuous and its tangent direction varies continuously: the curve is *G1* continuous.
There is no gap between them, but there might be a visible or palpable "step" or angle change at the joints.
##### Adjacency Analysis
![[Pasted image 20240425164741.png]]
##### Inheritance
$G_0$
##### Mathematical Analysis
$f(x) = g(x)$
Where $x$ is the point on the curves where they join or are continuous. 
##### Graphical Representation
Curves are continuous, but will probably have obvious "crease".
![[Pasted image 20240425135046.png|300]] ![[Pasted image 20240425134134.png|200]]
#### $G_1$ Continuity (i.e. Tangency Continuity)
##### Continuity Type
###### Tangency (i.e. Position Variation)
![[Pasted image 20240425165135.png]]
Tangency (G1 continuity) measures position and curve direction at the ends. 
	I.e. The two curves not only touch, but they go the same direction at the point where they touch.
The direction is determined by the first and second point on each curve. 
If these two points fall on a line, the two curves are tangent at the ends.

The first [[Derivatives|derivative]] of the two curves is equal at the point where they touch.
The curves also share a common [[Tangent Line|tangent]] direction at the join point (tangent).
This involves not only touching (G0) but also aligning tangents at the joints to ensure that the curve or surface does not have a sharp kink. 
G1 continuity means that the direction of the surface or curve is continuous across the boundary.
##### Adjacency Analysis
![[Pasted image 20240425165145.png]]
##### Inheritance
$G_1 >> G_0$
##### Mathematical Analysis
$f'(x) = g'(x)$
The derivatives are equal at x.
The both curves at point $x$ have the **same slope of their tangent lines**.  
##### Graphical Representation
Curves will appear smooth, though reflections could have sudden changes.
![[Pasted image 20240425135301.png|300]] ![[Pasted image 20240425134151.png|200]]
#### $G_2$ Continuity (or Curvature Continuity)
##### Continuity Type
###### Curvature
![[Pasted image 20240425165440.png]]
Curvature continuity (G2 continuity) between two curves measures **position**, **direction**, and **radius** of **curvature** at the ends.
**If the radius of curvature (i.e. of the osculating circles of each curve at that point) is the same at the common end point, curves are curvature continuous (G2).** 
	In other words, the curves not only go the same direction when they meet, but also have the same radius at that point. 
		This condition is not easy to determine by just looking at where the points are located.

The curves also share a common center of curvature at the join point (curvature).
G2 continuity takes smoothness further by aligning the curvature of the sections at the joins. This ensures the sections not only align in direction but also in curvature, making the transitions appear seamless and smooth
##### Adjacency Analysis
![[Pasted image 20240425165446.png]]
##### Inheritance
$G_2 >> G_1 >> G_0$
Both the first and [[Second Derivatives|second derivatives]] of the equations are equal at that point.
##### Mathematical Analysis
$f''(x) = g''(x)$
The [[Second Derivatives|second derivatives]] of the curves at $x$ are equal. 
	The second derivatives represent the rate of change of the slope of the [[Tangent Line|tangent line]].

The joining point $x$ of both curves means the curves will have the same (i.e. equal) [[#Notion of Surface Curvature In order to **define the curvature** of a surface, the **osculating circle** needs to be defined. Osculating Circle|osculating circle]].
	- Specifically, the radius of the osculating circles will be identical/equal.
		- So $k_1 = k_2$ and $r_1 = r_2$ at $x$.
			- The radius of the osculating circle at any point on a curve is inversely proportional to the curvature at that point. 
				- Mathematically, if the curvature $κ$ at a point on the curve is given, the radius $r$ of the osculating circle is $r=1/k$​.
##### Graphical Representation
Curves and reflections will appear smooth.
Ambient shadows will be gradual.
![[Pasted image 20240425135430.png|300]] ![[Pasted image 20240425134207.png|200]]
#### $G_3$ Continuity (i.e. Planar Continuity)
##### Continuity Type
###### Planar Acceleration
G3 continuity adds a third requirement: planar acceleration. 
Curves that are G3 continuous touch, go the same direction, have the same radius, and that radius is accelerating at the same rate at a certain point.
G3 continuous curves have equal third derivatives.
![[Pasted image 20240425135634.png|300]] ![[Pasted image 20240425134232.png|200]]
#### $G_n$ Continuity (i.e. variation)
##### Continuity Type
![[Pasted image 20240425165737.png]]
###### Variation
##### Inheritance
$G_n >> G_{n-1} >> G_{n-2} >> ...$
##### Adjacency Analysis
![[Pasted image 20240425170318.png]]
##### Mathematical Analysis
$f^n(x) = g^n(x)$