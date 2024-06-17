---
up:
  - "[[Dynamics Analysis]]"
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

#### Differentiation
Refers to the process of finding the derivative of a function.

The term "differential" comes from the concept of differences.
	Differentiation refers to the changes or differences in output values of a function as the input changes. 
		The differentiation of function values is represented/expressed in the fact that the derivative is defined as the **limit of the difference quotient**. 
			This quotient is a [[Division#Ratio|ratio]] - i.e. a rate of change.
				This ratio is called the **derivative**.
					The derivative (i.e. the ratio of the change in output values to the change in the input values) represents how a small change in the input (independent variable) results in a change in the output (dependent variable).
##### Difference Quotient
The ratio of the change in output values to the change in the input values) 
#### $\LARGE {f(x+h)−f(x)​ \over h}$
###### Difference
The numerator $f(x+h)−f(x)$ represents the [[Kinematics Analysis#Displacement (Δx,Δy,Δz)|displacement]] or the change in the function's value as the input changes from $x$ to $x+h$.
###### Quotient
Dividing by $h$ scales this change by the size of the increment $h$, giving the average rate of change over the interval from $x$ to $x+h$.
###### Geometric Interpretation
Geometrically, the difference quotient $\LARGE {f(x+h)−f(x)​ \over h}$ represents the slope of the secant line that passes through the points $(x,f(x))$ and $(x+h,f(x+h))$ on the graph of the function.
	As $h$ approaches zero, this secant line approaches the tangent line to the curve at the point $(x,f(x))$.
		The slope of this tangent line is the derivative $\LARGE f′(x)$.

## Derivative Is a [[Division#Ratio|Ratio]]
Ratios are a fundamental to the concept of the derivative.
It [[Data/Abstract Mathematical Spaces/Abstract Mathematical Objects/Measurement|measures]] the output ($\Delta y$) of a function $f(x)$ is proportioned to the input ($\Delta x$) at an infinitesimally small scale.

The derivative is the ratio of the change in the output to the change in the input as the change in the input approaches zero.
### Is the Instantaneous Rate (i.e. [[Division#Ratio|Ratio]]) of Change of a Function
A derivative (of a function $f(x)$) at a single point $f'(x)$, is itself a function that maps that single point (as an input) to the **value** of the **limit** of the **average rate of change** (i.e. limit of $\Delta y / \Delta x$) of that input.
#### Is the [[Tangent Line#The Slope of a Tangent Line|Slope]] (i.e. a rate/ratio between $\Delta y / \Delta x$) of the [[Tangent Line|Tangent Line]]
A **derivative** of a **function** at a point **provides the slope of the [[Tangent Line|tangent]] line to the function at that specific point**.^calculus-derivatives
- The **derivative** (which only exists for a given point) is itself is a **value** that represents the **exact slope** of the **tangent vector** at that **point** it is associated with (on the curve).
	- I.e. The **derivative** ***is*** the **slope of the tangent line**.
		![[Pasted image 20240410150406.png]]
 - The **Tangent line (or vector)** at a single point, represents the **"instantaneous" rate of change** of the curve (i.e. function) at that point. ^f2b939
	- The slope of this tangent line/vector is given by the **derivative** of the curve/function at this point. ^1f0a97
	- The derivative at any point, gives the direction of the tangent vector at that point.
		- For surfaces, taking partial derivatives provides the tangent planes.
## Derivative as a Name:
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
![[Pasted image 20240422232308.png]]
![[Pasted image 20240422233019.png]]
As the **interval or distance** over which the change is measured (between point $a$ and another determined point), **approaches zero**. ^c2858f
-  If this limit exists, then the function is **[[#Differentiability|differentiable]]** at that point, and the slope of the tangent line at this point is precisely the value of this limit itself - which is the derivative of that point.
**The equation to determine the derivative is:**
- The limit of the average rate of change as the interval (between two points) approaches zero.
	- Where the **average rate of change** over an interval of distance between two points is:
		- The **slope** of the **secant line** that connects those two points. 
The **[[Limits|limit]]** is the **means** of **transitioning** between the **average rate of change** to the **instantaneous rate of change**. ^limit-as-a-transition
![[Pasted image 20240410153825.png|400]] ^d8b06d
###### Inflection Points:
- Indicate the **change** from **concave** to **convex** or vice versa.
	- If you imagine this triangle "traveling" the length of the curve:
		- The way the **orientation** of $T_2$ changes relative to $T_1$ can indicate the **concavity** of the curve.
	- An [[Curves#Inflection Point|Inflection]] point is suggested if $T_2$ **rotates** from one side of $T_1$ to the other as $P_1$ and $P_2$ "travel" along the curve.
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
## Calculating the Derivative 
### Rules of Differentiation
###### *Important*: You only ever apply the Differentiating Rules to the terms associated with the independent variable.
#### Rate of Change of $t$ with Respect to Itself
Is always 1.
	I.e. The derivative of $t$ is simply 1. 
![[Pasted image 20240604144939.png]]
![[Pasted image 20240604144946.png]]
![[Pasted image 20240604144953.png]]
![[Pasted image 20240604145001.png]]
![[Pasted image 20240604145006.png]]
#### Power Rule
If $f(x) = x^n$, where $n$ is a constant, then the derivative of $f$ with respect to $x$ is given by:
	Basically just decrease the exponent by 1, then place the original value of the exponent as a coefficient in front of the term. 
#### $\LARGE \frac{d}{dx} x^n = n x^{n-1}$ 

###### Example
$\LARGE \frac{d}{dx} x^5 = 5x^4$ 
#### [[#Derivative of a Constant is Zero]]
If $f(x) = c$, where $c$ is a constant, then the derivative of $f$ with respect to $x$ is zero:
#### $\LARGE \frac{d}{dx} c = 0$
#### Constant Multiple Rule
If $f(x) = c \cdot g(x)$, where $c$ is a constant and $g(x)$ is a differentiable function, then the derivative of $f$ with respect to $x$ is:
#### $\LARGE \frac{d}{dx} \left( c \cdot g(x) \right) = c \cdot \frac{d}{dx} g(x)$
###### Example
#### $\LARGE \frac{d}{dx} (3x^3) = 3 \cdot \frac{d}{dx} (x^3) = 3 \cdot 3x^2 = 9x^2$

#### Sum Rule
If $f(x) = g(x) + h(x)$, where $g(x)$ and $h(x)$ are differentiable functions, then the derivative of $f$ with respect to $x$ is:
$\LARGE \frac{d}{dx} \left( g(x) + h(x) \right) = \frac{d}{dx} g(x) + \frac{d}{dx} h(x)$
###### Example
#### $\LARGE \frac{d}{dx} (x^2 + x^3) = \frac{d}{dx} (x^2) + \frac{d}{dx} (x^3) = 2x + 3x^2$

#### Difference Rule
If $f(x) = g(x) - h(x)$, where $g(x)$ and $h(x)$ are differentiable functions, then the derivative of $f$ with respect to $x$ is:
#### $\LARGE \frac{d}{dx} \left( g(x) - h(x) \right) = \frac{d}{dx} g(x) - \frac{d}{dx} h(x)$

#### Product Rule
If $f(x) = g(x) \cdot h(x)$, where $g(x)$ and $h(x)$ are differentiable functions, then the derivative of $f$ with respect to $x$ is:
#### $\LARGE \frac{d}{dx} \left( g(x) \cdot h(x) \right) = g(x) \cdot \frac{d}{dx} h(x) + h(x) \cdot \frac{d}{dx} g(x)$

###### Example
#### $\LARGE \frac{d}{dx} (x^2 \cdot \sin(x)) = x^2 \cdot \cos(x) + \sin(x) \cdot 2x = x^2 \cos(x) + 2x \sin(x)$
#### Quotient Rule
If $f(x) = \frac{g(x)}{h(x)}$, where $g(x)$ and $h(x)$ are differentiable functions and $h(x) \neq 0$, then the derivative of $f$ with respect to $x$ is:
#### $\LARGE \frac{d}{dx} \left( \frac{g(x)}{h(x)} \right) = \frac{h(x) \cdot \frac{d}{dx} g(x) - g(x) \cdot \frac{d}{dx} h(x)}{(h(x))^2}$
###### Example
#### $\LARGE \frac{d}{dx} \left( \frac{x^2}{\sin(x)} \right) = \frac{\sin(x) \cdot 2x - x^2 \cdot \cos(x)}{(\sin(x))^2}$

#### Chain Rule
If $f(x) = g(h(x))$, where $g$ is a differentiable function of $h(x)$ and $h(x)$ is a differentiable function of $x$, then the derivative of $f$ with respect to $x$ is:
#### $\LARGE \frac{d}{dx} g(h(x)) = g'(h(x)) \cdot h'(x)$

###### Example
#### $\LARGE \frac{d}{dx} \sin(x^2) = \cos(x^2) \cdot 2x = 2x \cos(x^2)$

### Example: Finding the Derivative

#### Given Position Function:

![[Pasted image 20240602234115.png]]
#### Find the Derivative:

To find the derivative x′(t), we'll differentiate x(t) with respect to t.

1. **Write the position function:** 
	![[Pasted image 20240602234124.png]]
2. **Differentiate each term:**
	Differentiating each term in the function $x(t) = t^2 + 3t +2$ involves applying basic [[#Rules of Differentiation|rules of differentiation]]. 
![[Pasted image 20240604144556.png]]

![[Pasted image 20240602234407.png]]
 ![[Pasted image 20240602234152.png]]
3. **Combine the results:** 
	![[Pasted image 20240602234201.png]]
### Interpretation
![[Pasted image 20240602234215.png]]
### Why Use Derivatives?

- **Instantaneous Information**: Unlike average velocity, which gives a single value over an interval, the derivative provides detailed information about how the position changes at every instant.
- **Dynamic Analysis**: It helps analyze motion dynamically. For example, if you want to know the acceleration (how velocity changes over time), you would take the derivative of the velocity function, 𝑥′′(𝑡)x′′(t).
### Summary
Finding the derivative x′(t) of a position function x(t) produces a new function that describes the instantaneous velocity at any given time t.
	This new function captures the dynamic nature of the motion and allows for deeper analysis of how the object's position changes over time.
## Derivatives of a Constant
When you differentiate a function, any constant term disappears because the derivative of a constant is zero. 
	This is a fundamental rule in calculus. Here's why:
### Derivative of a Constant is Zero
1. **Definition of the Derivative**:
    - The derivative of a function measures how the function's value changes as its input changes.
    - Mathematically, the derivative of a function $f(x)$ at a point $x$ is defined as: 
	    $\LARGE f′(x)=\lim\limits_{​\triangle x \rightarrow 0} {f(x+\triangle x) - f(x) \over \triangle x}​$
1. **Constant Function**:
    - A constant function $\LARGE f(x)=c$ means that the function's value does not change no matter what the input x is.
    - For example, $f(x)=5$ means the function always outputs 5, regardless of the value of x.
2. **Rate of Change of a Constant Function**:
    - Since the value of a constant function does not change, the rate of change (or the slope) is zero.
    - Using the definition of the derivative: 
	    $\LARGE f′(x)=\lim\limits_{​\triangle x \rightarrow 0} {f(x+\triangle x) - f(x) \over \triangle x}​$
    - For a constant function $f(x)=c$: 
		$\LARGE f'(x) = \lim\limits_{\triangle x \rightarrow 0} {c -c\over \triangle x} = \lim\limits_{\triangle x \rightarrow 0} {0\over \triangle x} = 0$
#### Visualizing the Derivative of a Constant
Imagine a flat horizontal line on a graph, like 𝑦=5y=5. This line has no slope; it does not rise or fall as you move along the 𝑥x-axis. The rate of change of this line is zero everywhere because it is perfectly flat.

When you differentiate a function that includes a constant, the constant term "disappears" in the sense that its derivative is zero, which is why the constant does not affect the derivative of the rest of the function.
## Critical Points
**Critical points** of a function are points in the domain of the function **where the first derivative is either zero or undefined**.
	These points are significant because they are potential locations where the function has local maxima, local minima, or points of inflection.
### Formal Definition
A point $x=c$ is called a **critical point** of a function $f(x)$ if one of the following conditions holds:
1. $\LARGE f'(c) = 0$
2. $\LARGE f′(c)$ does not exist
### Importance of Critical Points
#### Local Maxima and Minima
Critical points are candidates for local extrema (maxima and minima).
	By evaluating the first and second derivatives at these points, we can determine whether they are local maxima, local minima, or neither.

**Local maxima** and **local minima** are points on a function where the function reaches its highest or lowest value, respectively, within a small neighborhood around these points.
	They are important for understanding the behavior of functions and optimizing real-world problems.
##### Local Maximum
A function $f(x)$ has a **local maximum** at $x=c$ if there exists an interval $(a, b)$ containing $c$ such that:
$$\LARGE f(c) \geq f(x) \quad \text{for all} \quad x \in (a, b)$$
In other words, $f(c)$ is greater than or equal to the function values at nearby points.
##### Local Minimum
A function $f(x)$ has a **local minimum** at $x=c$ if there exists an interval $(a, b)$ containing $c$ such that:
$$\LARGE f(c) \leq f(x) \quad \text{for all} \quad x \in (a, b)$$
##### Finding Local Maxima and Minima
###### Identify Critical Points
Find the points where the first derivative $f′(x)$ is zero or undefined.
###### Second Derivative Test
Use the second derivative $f''(x)$ to determine the nature of the critical points.
    - If $f''(c) > 0$, the function has a local minimum at $x=c$.
    - If $f''(c) < 0$,, the function has a local maximum at $x=c$.
    - If $f''(c) = 0$, the test is inconclusive.
##### [[#Inflection Points|Inflection Points]] (*also see* [[Curves#Inflection Point|Inflection Points]] in Curves)
**Inflection points** are points on a function where the concavity changes.
	These points are not necessarily where the first derivative is zero but are significant in understanding the behavior and shape of the function.

***Important***: Although not all inflection points are critical points, analyzing the behavior of the function around critical points can sometimes help identify points where the concavity of the function changes.

A function $f(x)$ has an **inflection point** at $x=c$ if the concavity of the function changes at that point.
	This means the function changes from being concave up (convex) to concave down (concave) or vice versa.
###### Identifying Inflection Points
To find inflection points of a function $f(x)$:
1. **Find the second derivative** $\LARGE f′′(x)$.
2. **Set the second derivative equal to $0$ and solve for $x$**:
    $$\LARGE f''(x) = 0$$
3. **Determine if the concavity changes around those points**:
    - If $\LARGE f′′(x)$ changes sign as $x$ passes through $c$, then $x=c$ is an inflection point.
### Identifying Critical Points
#### Steps to Determine the Nature of Critical Points:
##### First Derivative Test:
- **Find the first derivative** of the function $f'(x)$.
- **Set the first derivative to zero** to find the critical points: $f'(x) = 0$.
- Solve for $x$ to find the critical points.
##### Second Derivative Test (if applicable):
- **Find the second derivative** of the function $f''(x)$.
- **Evaluate the second derivative at the critical points**:
	- If $f''(x) > 0$ at a critical point, the function has a **local minimum** at that point.
	- If $f''(x) < 0$ at a critical point, the function has a **local maximum** at that point.
	- If $f''(x) = 0$, the second derivative test is inconclusive; further analysis is needed.
##### Alternative Analysis (if the second derivative test is inconclusive):
- **Analyze the sign of the first derivative** on intervals around the critical points to determine whether the function is increasing or decreasing.
- **Consider higher-order derivatives** or other methods, such as the first derivative test, to determine the behavior of the function.
### Example:
Let's illustrate with a simple example:
Given the function $$\LARGE f(x) = x^3 - 3x^2 + 2$$
1. **Find the first derivative**:
    $$\LARGE f'(x) = 3x^2 - 6x$$
2. **Set the first derivative to zero and solve for $x$**:
    $$\LARGE 3x^2 - 6x = 0$$
    
    $$\LARGE 3x(x - 2) = 0$$
    
    $$\LARGE x = 0 \quad \text{or} \quad x = 2$$
    
    The critical points are $x = 0$ and $x = 2$.
    
3. **Find the second derivative**:
    $$\LARGE f''(x) = 6x - 6$$
4. **Evaluate the second derivative at the critical points**:
    - At $x = 0$:
        $$\LARGE f''(0) = 6(0) - 6 = -6 \quad (\text{negative, so } x = 0 \text{ is a local maximum})$$
    - At $x = 2$:
		$$\LARGE f''(2) = 6(2) - 6 = 6 \quad (\text{positive, so } x = 2 \text{ is a local minimum})$$
