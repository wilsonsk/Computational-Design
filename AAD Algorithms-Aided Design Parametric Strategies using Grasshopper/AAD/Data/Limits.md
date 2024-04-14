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
# Limits
## Limit i.e. *limes*
Meaning the boundary or threshold.
- The mathematical concept that describes the behavior of a function (i.e. a curve) as its independent variable approaches some boundary value.
	- I.e. as one value (or point) gets closer to another point. 

A Limit refers to the **value** of a **function's output** as that **function's input** (i.e. a point on the function curve) approaches or gets infinitely close to some point.
	![[Pasted image 20240410151035.png]]
	- *$f(x)$ is a function that maps every $x$ (i.e. point) to an $F(x)$ on a 2D graph.*
	- *$f'(a)$ is the **derivative** at a point where $x=a$.*
	- *$h$ (i.e. the independent variable) represents the **increment or distance** from the point $a$ along the $x-axis$.*
		- *It is used to measure how far away a point on the curve is from point $a$ when calculating the slope of the secant line.*
			- *As $h$ approaches zero (i.e. zero distance between a point and point $a$), the secant line approaches the tangent line $T_a$ for point $a$*.
## The limit as a means of [[Derivatives^limits-as-a-transitions|transition]]:
Between the **average rate of change** to the **instantaneous rate of change**. 
- Mathematically, the [[Derivatives^limits-as-a-transitions|derivative]] at a point is defined as the **limit** of the **difference quotient** (the slope of the secant line) as the interval (distance between two values/points) **approaches zero**.
	- Therefore, if this limit exists at this point, then the function is **differentiable** at that point.
		- And the slope of the tangent line at this point is precisely the value of this limit itself - which is the derivative of that point.
## Limits Define Continuity or [[Discontinuities|Discontinuity]]
### [[Curves#Continuity (i.e. when curves join)|Continuity]]
Continuity at a point means that there is **no** interruption in the curve (i.e. function) at that point. 
- For a function to be continuous at a point $a$, three conditions must be met:
	1. **The function $f(x)$ is defined at point $a$.**
		- I.e. There exists an output value $f(a)$.
	2. **The limit exists at point $a$.**
		![[Pasted image 20240410233411.png]]
		- I.e. The left-hand limit (as $x$ approaches $a$ from the left) and the right-hand limit (as $x$ approaches $a$ from the right) both exist and are equal.
			- Here, $h$ (i.e. the independent variable representing distance or interval between $x$ and $a$) can approach zero from negative values (left-hand limit) or from the positive values (right-hand limit).
				- This means that as you get closer to $a$ from either side, the function's output values approach the same number.
	1. **The function's output value at $a$ equals the limit at $a$**.
		- I.e. The **value** $f(a)$ is **equal** to the **limit** of $f(x)$ as **$x$ approaches $a$**.

#### Non-Differentiability Without Discontinuity
A function can be continuous but not [[Derivatives#Differentiability|differentiable]] at a point. 
- This happens when the function's graph has a sharp turn or cusp at that point. 
	- Even though the function does not break or jump, the direction of the graph changes so abruptly that there is no single tangent line that can be drawn at that point. 
##### How [[Derivatives#Differentiability|differentiability]] relates to the rate of change:
- **Average Rate of Change (i.e. slope of the [[Secant Line|secant line]]): 
	- **If we look at the slopes of secant lines near a point of interest on the curve, the average rate of change is represented by these slopes.** 
		- **If the slopes of the secant lines from either side of the point do not converge to the same value as they get infinitely close to the point (i.e. as $h$ gets smaller, this suggests that the derivative (instantaneous rate of change) at the point does not exist**.		
- I.e. If the limit doesn't exist for a point, it means:
	- The function's (i.e. curve's) behavior is **too erratic** at that point to be **captured by a single number** (i.e. the slope of the tangent- the derivative).
		- Therefore, the function is not [[Derivatives#Differentiability|differentiable]] at that point.
			- Meaning no well defined instantaneous rate of change at that point.
### [[Discontinuities|Discontinuity]]
Discontinuity at a point means there is a **sudden change in direction**, an **interruption in the smoothness**, or a **break** in the curve itself. 
- When the left-hand and right-hand limits are not equal, it means there's a jump in the function at point $a$ (i.e. where $x=a$.) 
	- The function is approaching different values from the left and right as you get closer to $a$.
		- So there is no single value that $f(x)$ is approaching. 
			- As a result, the overall limit at $a$ does not exist.
				- And **for a derivative to exist at point $a$, this limit must exist** for that point (and be the **same value** **irrespective of the direction** from which **$h$ approaches zero)**.

#### Why [[Discontinuities|Discontinuities]] (i.e. disruptions in smoothness) Prevent the Existence of a Limits
Discontinuities create a break in the function that disrupts the foundational requirement for limits, and since derivatives are defined in terms of limits, a discontinuity at a point means you cannot have a derivative at that point. 
- The prevention of derivatives due to discontinuities is a direct consequence of the definition of a derivative requiring a well-defined limit.

**Limits Require Consistency**: 
- For a limit to exist at a certain point, the function must approach the same value from both the left and the right of that point. 
	- This is the concept of the limit being 'well-defined'.

**Discontinuities Break Consistency**: 
- A discontinuity at a point means that there is a break in this consistency.
	- There could be a jump in the function values ([[Discontinuities#Jump Discontinuity|jump discontinuity]]), or the function could go off to infinity ([[Discontinuities#Infinite Discontinuity|infinite discontinuity]]), or the function could simply not be defined at the point ([[Discontinuities#Removable Discontinuity|removable discontinuity]]).

**Derivatives Rely on Limits**: 
- The derivative at a point is defined as the limit of the slope of the secant lines as the interval between the points on the lines approaches zero. 
	- [[Derivatives#^discontinuities-prevent-limits-which-prevent-deriviatives|If the limit doesn't exist because the function isn't approaching the same value from both sides, then the derivative cannot be defined.]]

**Impact on Derivatives**: 
- Without a limit, there is no way to talk about the slope of the function at the point of discontinuity. 
	- You cannot have an instantaneous rate of change (derivative) where there is no consistent value for the function at that point.

#### Both Non-Differentiability and Discontinuities "Break Consistency of a Limit at a Point"
But they do so in **different ways**.

##### Discontinuity:
- **Definition**: 
	- A discontinuity at a point $x=a$ occurs when a function does not have a well-defined limit at that point, or the limit exists but does not equal the function's value at $a$ (if it's defined at all).
- **Detection**:
    - **Graphical Method**: Look for breaks, jumps, or holes in the graph at $x=a$.
    - **Limit Analysis**: Check if the left-hand limit and the right-hand limit are equal. 
	    - If they are not, or if one or both do not exist, $f(x)$ is discontinuous at $a$. 
		    - Also, if the limits are equal but not equal to $f(a)$ (the actual function value at $a$, if defined), then $f(x)$ has a [[Discontinuities#Removable Discontinuity|removable discontinuity]] there.
##### Non-Differentiability:
- **Definition**: 
	- A point of non-differentiability on a curve is a point where the function is continuous (no breaks, jumps, or holes) but does not have a well-defined tangent line (and hence, no derivative) at that point. 
		- This usually happens at sharp corners or [[Discontinuities#^2b891a|cusps]].
- **Detection**:
    - **Graphical Method**: Look for sharp corners or cusps in the graph where the direction of the curve changes abruptly, but there is no break in the graph.
    - **Derivative Analysis**: If the function is continuous at $x=a$ but the limit defining the derivative, does not exist due to a change in the slope of secant lines that does not stabilize as $h$ approaches zero, the function is non-differentiable at $a$.
##### Key Distinctions:
- **Continuity First**: 
	- To be non-differentiable at a point, a function must first be continuous at that point. 
		- If it's discontinuous, questions of differentiability at that point don't apply.
- **Behavior of Limits**: 
	- For discontinuities, the issue is with the function's limit(s) not matching the function's value or not existing. 
		- For non-differentiability, the limit defining the derivative does not exist due to the slope changing abruptly, even though the function itself smoothly passes through the point.
