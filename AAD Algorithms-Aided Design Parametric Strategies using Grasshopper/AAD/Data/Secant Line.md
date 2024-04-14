---
up:
  - "[[Data Relationships]]"
related:
  - "[[Curves]]"
  - "[[Data Operations]]"
  - "[[Notion of Surface Curvature]]"
  - "[[Numbers]]"
  - "[[Points]]"
  - "[[SubD Surface Patterns]]"
date created: 2024-04-10
---
# Secant Line

![[Pasted image 20240410153825.png|400]]
Is a **straight line** that **intersects a curve at two points**.
## Secant lines and Tangent lines
As another point gets closer and closer to a point $a$ on either side:
- The slopes of the **secant lines** (i.e. lines connection the two points) will approach the **slope of the tangent line at point $a$**.
	- The **slope of a secant line** is the the **average rate of change** over an **interval of distance** between two points.
		![[Pasted image 20240410225437.png]] = ![[Pasted image 20240410225456.png]] = ![[Pasted image 20240411000804.png]]
		- Also called the **difference quotient**.
			- The slope of a secant line is calculated between two points on the curve, say $(x,f(x))$ and $(x+h,f(x+h))$, where $h$ is a non-zero distance between the two points along the x-axis.
			- The slope is given by $(f(x+h)−f(x))/h$​, which is the average rate of change of $f$ over the interval from $x$ to $x+h$.
				- **As $h$ gets smaller, that is as the distance between the two points decreases, the secant line starts to resemble a tangent line at the first point.**
		- And the **[[Limits|limit]]** of the **slope of the secant** line ***IS*** the [[Derivatives|derivative]] of point $a$.
	- The [[Derivatives#^f2b939|slope of the tangent line]] is the instantaneous rate of change of the function at a single point. 
		- And this **slope of the tangent** line ***IS*** the **derivative**.
	- **As the distance between these two points decreases, the secant line approximates the [[#^f2b939|tangent line]] at a point $a$.**
- The slope of a secant line is like a "preview" of the tangent slope. 
	- As the second point used to create the secant line moves closer to the first, the secant line becomes a better and better approximation of the tangent line. 
- The process of taking the limit effectively "zooms in" on the curve at point $a$​ until the secant line and the tangent line are indistinguishable.
	- [[Derivatives#^d8b06d|And the average rate of change becomes the instantaneous rate of change]].
		- That being the slope of the tangent line ($T_a$) at point $a$​.

## Secant Lines and [[Derivatives#Differentiability|Differentiability]] 
##### How [[Derivatives#Differentiability|differentiability]] relates to the rate of change:
- **Average Rate of Change (i.e. slope of the [[Secant Line|secant line]]): 
	- **If we look at the slopes of secant lines near a point of interest on the curve, the average rate of change is represented by these slopes.** 
		- **If the slopes of the secant lines from either side of the point do not converge to the same value as they get infinitely close to the point (i.e. as $h$ gets smaller, this suggests that the derivative (instantaneous rate of change) at the point does not exist**.		
- I.e. If the limit doesn't exist for a point, it means:
	- The function's (i.e. curve's) behavior is **too erratic** at that point to be **captured by a single number** (i.e. the slope of the tangent- the derivative).
		- Therefore, the function is not [[Derivatives#Differentiability|differentiable]] at that point.
			- Meaning no well defined instantaneous rate of change at that point.