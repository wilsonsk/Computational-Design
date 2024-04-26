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
## Continuity: (i.e. when curves join)
![[Pasted image 20240425140151.png]]
A curve or surface can be described as having $G_n$ continuity.
	*n* being the increasing measure of smoothness.
	
Continuity has different behavior with respect to:
### [[Parametric Space]]: *C* 
- if a curve is **connected**: it has *C0* continuity.
	- if its first derivation is continuous: the original curve has *C1* continuity.
	- if the *nth* derivation is continuous: the original curve has *Cn* continuity.
- *C* continuity does **not** mean that a curve is geometrically smooth.
### [[Geometric Space]]: *G* 
If a curve has *C0* continuity: it is *G0* continuous- it is connected and this means the same thing in both parametric and geometric space.
![[Pasted image 20240425135811.png]]
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
##### Graphical Representation
Curves will appear smooth, though reflections could have sudden changes.
![[Pasted image 20240425135301.png|300]] ![[Pasted image 20240425134151.png|200]]
#### $G_2$ Continuity (or Curvature Continuity)
##### Continuity Type
###### Curvature
![[Pasted image 20240425165440.png]]
Curvature continuity (G2 continuity) between two curves measures **position**, **direction**, and **radius** of curvature at the ends.
**If the radius of curvature is the same at the common end point, curves are curvature continuous (G2).** 
	In other words, the curves not only go the same direction when they meet, but also have the same radius at that point. 
		This condition is not easy to determine by just looking at where the points are located.
Both the first and [[Second Derivatives|second derivatives]] of the equations are equal at that point.

The curves also share a common center of curvature at the join point (curvature).
G2 continuity takes smoothness further by aligning the curvature of the sections at the joins. This ensures the sections not only align in direction but also in curvature, making the transitions appear seamless and smooth
##### Adjacency Analysis
![[Pasted image 20240425165446.png]]
##### Inheritance
$G_2 >> G_1 >> G_0$
##### Mathematical Analysis
$f''(x) = g''(x)$
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