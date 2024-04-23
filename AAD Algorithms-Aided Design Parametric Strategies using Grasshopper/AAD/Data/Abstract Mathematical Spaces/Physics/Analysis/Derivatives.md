---
up:
  - "[[Analysis]]"
related:
  - "[[Data Operations]]"
  - "[[SubD Surface Patterns]]"
  - "[[Curves]]"
  - "[[Notion of Surface Curvature]]"
  - "[[Numbers]]"
  - "[[Points]]"
  - "[[Data Relationships]]"
date created: 2024-04-10
---
# Derivatives
## $f'(x)$
## Is a [[Proportion|Proportion]]
Proportion is fundamental to the concept of the derivative.
It [[Measurement|measures]] the output ($\Delta y$) of a function $f(x)$ is proportioned to the input ($\Delta x$) at an infinitesimally small scale.
### Is the Instantaneous Rate (i.e. Proportion) of Change of a Function
A derivative (of a function $f(x)$) at a single point $f'(x)$, is the **value** of the **limit** of the **average rate of change** (i.e. limit of $\Delta y / \Delta x$).
#### Is the [[Tangent Line#The Slope of a Tangent Line|Slope]] (i.e. a proportion/rate/ratio between $\Delta y / \Delta x$) of the [[Tangent Line|Tangent Line]]
A **derivative** of a **function** at a point **provides the slope of the [[Tangent Line|tangent]] line to the function at that specific point**.^calculus-derivatives
- The **derivative** (which only exists for a given point) is itself is a **value** that represents the **exact slope** of the **tangent vector** at that **point** it is associated with (on the curve).
	- I.e. The **derivative** ***is*** the **slope of the tangent line**.
		![[Pasted image 20240410150406.png]]
 - The **Tangent line (or vector)** at a single point, represents the **"instantaneous" rate of change** of the curve (i.e. function) at that point. ^f2b939
	- The slope of this tangent line/vector is given by the **derivative** of the curve/function at this point. ^1f0a97
	- The derivative at any point, gives the direction of the tangent vector at that point.
		- For surfaces, taking partial derivatives provides the tangent planes.
## Derivative as a name:
- First used by mathematician Lagrange in the late 18th century.
	- Derived from the Latin word "derivare", which means:
		- "To draw off" or "to take from".
			- The idea was to take the original function and draw from it a new function.
				- This new function would describe how original function changes.
- The derivative is the result of an operation that takes a function and produces another function.
	- Then new function (the derivative) provides information on the slope or rate of change of the original function at any given point. 
- It is a conceptual representation of the slope over an interval that is infinitesimally small.
	- So small that it's effectively a point. 
- Refers to a seemingly "instantaneous" rate of change. 
## Formally, the derivative at a point $a$, is **defined** as the [[Limits|limit]] of the slope of the [[Secant Line|secant line]] (i.e. **average rate of change**)
- As the **interval or distance** over which the change is measured (between point $a$ and another determined point), **approaches zero**. ^c2858f
	-  If this limit exists, then the function is **[[#Differentiability|differentiable]]** at that point, and the slope of the tangent line at this point is precisely the value of this limit itself - which is the derivative of that point.
- **I.e. The equation to determine the derivative is:**
	- The limit of the average rate of change as the interval (between two points) approaches zero.
		- Where the **average rate of change** over an interval of distance between two points is:
			- The **slope** of the **secant line** that connects those two points. 
- The **[[Limits|limit]]** is the **means** of **transitioning** between the **average rate of change** to the **instantaneous rate of change**. ^limit-as-a-transition
	![[Pasted image 20240410153825.png|400]] ^d8b06d
###### Inflection Points:
- Indicate the **change** from **concave** to **convex** or vice versa.
	- If you imagine this triangle "traveling" the length of the curve:
		- The way the **orientation** of $T_2$ changes relative to $T_1$ can indicate the **concavity** of the curve.
	- An inflection point is suggested if $T_2$ **rotates** from one side of $T_1$ to the other as $P_1$ and $P_2$ "travel" along the curve.
- An inflection point is typically a smooth, continuous transition or change in the curvature of a function.
	![[Pasted image 20240410143446.png|500]]
	- Take some $P_1 =C(s_1)$ on a curve $C$.
		- $T_1$ = the **unit tangent vector** at this point $P_1$.
	- $P_2$ is a point on $C$ that represents "a small movement" relative to $P_1$.
		- $T_2$ = the **unit tangent vector** at this point $P_2$.
	- Vector $V =T_2 - T_1$
		- Notice that they combine to "make" a **triangle**.
			- It represents the **rate of change** between the two points on the curve (in the function) $T_1$ and $T_2$.
				- That is the approximation of the curve between $P_1$ and $P_2$.
					- As the distances between $P_1$ and $P_2$ decrease, the **secant line** becomes a better approximation of the **tangent** $T_1$ at point $P_1$.
			- The triangle visually describes the "smoothness" or **continuity** of a function.
				- If the curve is smooth and function is differentiable at the measured points, then the tangent vectors will change gradually and not "jump".
	- If $P_1$ and $P_2$ are very "close" together distance wise:
		- $T_1$ and $T_2$ will be almost equal.
			- Therefore, $V$ will be almost **perpendicular** (i.e. normal, orthogonal) to both $T_1$ and $T_2$.
## Differentiability:
**In calculus**, it refers a **curve** that has, at a **point** in a **function**, a **derivative** **existing**. 
- **As Differentiability relates to [[Limits#Limits Define Continuity or Discontinuities Discontinuity|Continuity]]:**
	- **For a function to be differentiable at a point**, it **must** be **continuous at that point**, and the **derivative** at that point must also exist.
		- Solutions to differential equations are often smooth and continuous (i.e. differentiable).
			- This is because most physical process **behave** as though they are continuous (i.e. smooth) over time and space.
				- Making differentiable functions suitable models for such processes.
	- For a curve (i.e. function) to be differentiable **everywhere** it must be smooth without any [[Discontinuities|discontinuities]] for the entirety of its length. 
		- And would therefore, have tangent vectors for every point on its curve.
- **In computational geometry**, it refers to the curve being smooth enough at a point that you can define a tangent line at every point along the curve. 
	- **I.e. A curve is differentiable if it has a derivative at every point along the curve.**
		- In which case it would be smooth enough that a tangent vector could be defined at every point along the curve.
	- A curve that is not differentiable at a point might have a discontinuity (like a cusp) there instead.
## Why [[Discontinuities|Discontinuities]] (i.e. disruptions in smoothness) Prevent the Existence of a Derivative
Discontinuities prevent the existence of derivatives because the derivative is defined as the limit of the slope of secant lines as the points used to create them get infinitely close. 
- This definition **presupposes** that the **function is continuous** at the point where the derivative is being calculated.
- **Impact on Derivatives**: ^discontinuities-prevent-limits-which-prevent-deriviatives
	- Also, in actuality it is that [[Limits#Why Discontinuities Discontinuities (i.e. disruptions in smoothness) Prevent the Existence of a Limits|Discontinuities can prevent the existence of limits, which in turn means that derivatives at those points cannot be defined.]] 
		- Without a limit, there is no way to talk about the slope of the function at the point of discontinuity. 
			- You cannot have an instantaneous rate of change (derivative) where there is no consistent value for the function at that point.

When a function is discontinuous at a point, there's a break in the curve at that point. 
- Since the **derivative is the slope of the tangent line** to the curve **at a point**;
	- And a **tangent line requires a smooth passage through the point**;
		- A discontinuity creates a situation where there's no single, well-defined tangent line.

**Cusps**:
- A sudden change in direction (i.e. a sharp corner) of the curve $f(x)$ at point $a$.
	- Even though this function might be continuous:
		- The slopes of the **secant lines** from the **left and right** differ.
			- Thus the limits from the left and right are not equal.
				- Thus no unique slope (i.e. derivative) of the tangent at point $a$ exists.
- Since the [[#^c2858f|derivative is defined in terms of the limit]]:
			- If the limit does not exist for a given point, then the [[#^277add|derivative also does not exist]] for that same given point.
- If $f(x)$ is continuous without discontinuities like cusps:
	- The limits from left and right at any point, are equal.
		- Thus a derivative exists for that point, having a well defined tangent line with a slope. 
- **[[#Discontinuities|Discontinuity]]**:
	- Discontinuities in a curve are positions where the curve "jumps" from one value to another without any connecting points in between.
		- Without a continuous path:
			- There is not "approaching" the point from either side in a meaningful way.
				- Which means there's no slope of the secant to speak of.	
- **How This Affects Tangent Vector Direction:**
	- **Indeterminacy at Sharp Points**: 
		- At points where the curve has a sharp change in direction (non-differentiable points), the concept of a single, well-defined tangent line breaks down. 
			- If you tried to draw a tangent, you would find an infinite number of lines that could arguably be tangents, depending on the approach angle. 
				- This indeterminacy means there's no unique tangent vector direction at such points.
	- **Visualization with Secant Lines**: 
		- Imagine drawing secant lines (lines connecting two nearby points on the curve) and then moving these points closer together towards the point of interest. 
			- For smooth parts of the curve, as the points get infinitely close, the secant line approaches a unique position — the tangent line. 
				- However, at a sharp corner or discontinuity, the limit of the secant line's position oscillates or becomes undefined as the points get closer, indicating the absence of a well-defined tangent line and thus a tangent vector.
## Second Derivative
The second derivative of a function $f(x)$ is denoted as $f^"(x)$ or $d^2y/dx^2$.
It is obtained by **differentiating** the **first derivative** $f'(x)$
### Calculating the Second Derivative
###### 1. Compute the First Derivative:
Find $f'(x)$ of the function $f(x)$.
	The first derivative represents the **rate of change** of the function i.e. the **slope of the tangent line** at any point $x$.