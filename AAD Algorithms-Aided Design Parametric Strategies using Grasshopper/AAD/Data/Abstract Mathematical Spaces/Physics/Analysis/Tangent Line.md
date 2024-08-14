---
up:
  - "[[Dynamics Analysis]]"
related:
  - "[[Derivatives]]"
  - "[[Secant Line]]"
  - "[[Limits]]"
  - "[[Proportion]]"
date created: 2024-04-22
---
# Tangent Line
Touches the **curve of a function** **exactly once**.
![[Pasted image 20240422200942.png]]
![[Pasted image 20240422200754.png|500]]
The [[Secant Line|Secant Line]] touches a curve of a function at least twice. 
	The tangent touches just one of those points (of secant line) at exactly on point on the tangent line.
## Represents a [[Proportion#Visually Represented by the Hypotenuse of a Right Triangle|Proportion]]
### As the [[Proportion#Visually it is the Hypotenuse of a Right Triangle|Hypotenuse]] of the Triangle Representing the [[Derivatives#Is a Proportion Proportion|Derivative]] 
It represents $\Delta y / \Delta x$ where $\Delta y$ and $\Delta x$ are the **adjacent** and **opposite** sides of that connect to the tangent line and to each other.
Therefore, creating a triangle where the tangent is the **hypotenuse**. 
	And again, this "hypotenuse" i.e. tangent line **only touches the curve of a function exactly once**.
		I.e. Only a **single point** on the **tangent line** **touches a curve of a function in exactly one point**.
![[Pasted image 20240422150825.png]]![[Pasted image 20240422150856.png]]
## The Slope of a Secant Line 
The Secant Line connects two points on a curve.

The Slope of the Secant Line gives an average rate of change between those two points.

As the two points get closer to each other, the secant line approaches the tangent line at a single point on the curve.

Mathematically, if you have a function $f(x)$ and two points on the curve, $(x1,f(x1))$ and $(x2,f(x2))$:
	Then the slope of the secant line is given by:
		$\LARGE m_{sec} = \frac{f(x_2) - f(x_1)}{x_2 - x_1}$

When $x_2$​ approaches $x_1$​, this slope approaches the derivative of $f$ at $x_1$, which is the slope of the tangent line at that point.
	In the limit as $x_2$ approaches $x_1$​, the secant line becomes the tangent line. 
		This is represented as:
			$\LARGE \lim_{x_2 \to x_1} \frac{f(x_2) - f(x_1)}{x_2 - x_1} = f'(x_1)$

Therefore, as the two points defining the secant line get infinitesimally close, the slope of the secant line approximates the slope of the tangent line.
## The Tangent Line Through a Point (on a Curve)
The equation of the tangent line through a point $(a, f(a))$ is derived from the limit of the slope of the secant line as it approaches the point $(a, f(a))$. 
	The equation $y = f(a) + f'(a)(x - a)$ is derived by finding the slope of the tangent line as the limit of the slopes of secant lines and then using the point-slope form of the equation of a line. 
		This process ensures that the tangent line touches the curve $y = f(x)$ at exactly one point $(a, f(a))$ and has a slope equal to the derivative $f'(a)$ at that point.

The **tangent line** through a point on a curve is derived using the derivative to find [[Straight Lines#The Standard Equation of a Line with Slope $m$ Passing Through a Point $(x_1, y_1)$|the slope at that point]].

1. **Secant Line Slope**:
   The slope of the secant line between the points $(a, f(a))$ and $(x, f(x))$ on the curve $y = f(x)$ is given by:
   $$\LARGE
   m_{\text{sec}} = \frac{f(x) - f(a)}{x - a}
   $$

2. **Tangent Line Slope**:
   The slope of the tangent line at the point $(a, f(a))$ is the limit of the secant slope as $x$ approaches $a$:
   $$\LARGE
   m_{\text{tan}} = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}
   $$

   This limit, if it exists, is the derivative of $f(x)$ at $x = a$, which we denote as $f'(a)$:
   $$\LARGE
   m_{\text{tan}} = f'(a)
   $$

3. **Equation of the Tangent Line**:
   The equation of a line with slope $m$ passing through a point $(x_1, y_1)$ is:
   $$\LARGE
   y - y_1 = m(x - x_1)
   $$

   In our case, the slope $m$ is $f'(a)$ and the point $(x_1, y_1)$ is $(a, f(a))$. 
	   Plugging in these values:
   $$\LARGE
   y - f(a) = f'(a)(x - a)
   $$

4. **Rearranging to the Standard Form**:
   We can rearrange this equation to the more familiar form of the tangent line:

   $$\LARGE
   y = f(a) + f'(a)(x - a)
   $$
## The [[Derivatives#Is the Tangent Line The Slope of a Tangent Line Slope (i.e. a proportion/rate/ratio between $ Delta y / Delta x$) of the Tangent Line Tangent Line|Slope]] of a Tangent Line
Is the [[Derivatives|derivative]] of that single point along the curve of a function.
$$\LARGE m_{tan} =  \lim_{x \to a} \frac{f(x) - f(a)}{x - a}$$ 