---
up:
  - "[[Curves]]"
related:
  - "[[Data Relationships]]"
  - "[[Derivatives]]"
  - "[[Limits]]"
  - "[[Abstract Concept]]"
  - "[[Secant Line]]"
  - "[[SubD Surface Patterns]]"
date created: 2024-04-10
---
# Discontinuities
## [[Discontinuities|Discontinuity]] (i.e. Disjoint)
### Continuity Type
Disjoint
![[Pasted image 20240425163949.png]]
### Adjacency Analysis
Nothing
![[Pasted image 20240425164152.png]]
### Inheritance
N/A
### Math Analysis
$f(x) != g(x)$
Domains are not adjacent.
Where $x$ is the point
### Graphical Representation
End Points not coincident, would need to be moved to join.
## Definition
Refers to **points or regions** on the **curve** where there is a **sudden change in direction**, an **interruption in the smoothness**, or a **break** in the curve itself. 
- Ways discontinuities manifest:
	- **Cusps**: Points where the curve suddenly **changes direction**, creating a sharp point.  ^2b891a
		- Characterized by an infinite curvature at the point of change. 
	- **Breaks or Gaps**: Points where the curve is not continuous.
		- There is a literal break or gap in the curve, meaning the curve does not have a defined value at those points or jumps from one point to another without a connecting path.
	- **Tangential Discontinuities**: Places where the direction of the curve changes abruptly, but the curve itself remains connected. 
		- This can occur in piecewise functions where segments of the curve meet. 
	- **Cornerness**: Similar to cusps, but may not be as sharp.
		- Refers to points where the smoothness ([[Derivatives#Differentiability|differentiability]]) of the curve is interrupted, but the curve does not necessarily have an infinite curvature.
	- **Vertical Tangents**: Points where the slope of the curve becomes undefined, typically occurring in steep parts of the curve that approach a vertical orientation. 
- Identifying and Addressing discontinuities is crucial for algorithms that rely on the smoothness of curves.
	- Such as those for curve fitting, smoothing, or for the calculation of derivatives and integrals in mathematical analysis. 

## Some ways a discontinuity can occur:
###### Jump Discontinuity: 
- The left-hand limit and the right-hand limit exist but are not equal to each other. 
	- The function "jumps" from one value to another at the point of discontinuity.
###### Infinite Discontinuity: 
- The function goes to infinity in at least one direction as it approaches the point.
###### Removable Discontinuity: 
- The function has a hole at a point where the limit exists, but the function is not defined at that point or is defined but has a different value.

## ### Non-[[Derivatives#Differentiability|Differentiability]] Without Discontinuity

A function can be continuous but not differentiable at a point. 
- This happens when the function's graph has a sharp turn or cusp at that point. 
	- Even though the function does not break or jump, the direction of the graph changes so abruptly that there is no single tangent line that can be drawn at that point.
- I.e. If the [[Limits]] doesn't exist for a point, it means:
	- The function's (i.e. curve's) behavior is **too erratic** at that point to be **captured by a single number** (i.e. the slope of the tangent- the derivative).
		- Therefore, the function is not [[Derivatives#Differentiability|differentiable]] at that point.
			- Meaning no well defined instantaneous rate of change at that point.