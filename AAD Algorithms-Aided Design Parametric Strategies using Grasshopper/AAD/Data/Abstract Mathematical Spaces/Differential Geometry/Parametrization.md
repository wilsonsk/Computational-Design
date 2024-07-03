---
up:
  - "[[Differential Geometry]]"
related: 
date created: 2024-06-29
---
# Parametrization
A a way to describe curves using parameters.

- - -
## Parametric Function
A parametric function is a way of defining a curve by expressing the coordinates of the **[[Points|points]]** on the [[Curves|curve]] as [[Mapping|functions]] of one or more parameters. 
	Instead of describing $y$ as a function of $x$ (or vice versa) directly, parametric functions define both $x$ and $y$ (and potentially $z$ in three dimensions) in terms of an independent parameter $t$.
##### Form
For a plane curve, the parametric equations are of the form
$$\LARGE x=f(t), \quad y = g(t)$$
Where $f$ and $g$ are **parametric functions** of the parameter $t$.
These functions specify the coordinates $(x, y, z)$ of points on the curve as the parameter $t$ varies over a certain interval.

- - -
### Relationship to Different Types of Function
Parametric functions represent linear, quadratic, cubic, and other types of functions. 
	The key is that parametric equations express the coordinates of points on a curve (or surface) as functions of one or more parameters. 
#### Linear Parametric Equations
- **Example**: A straight line parametrized by $t$
$$\LARGE x(t) = at + b, \quad y(t) = ct + d$$
- **Explanation**: 
	- The functions $f(t) = at + b$ and $g(t) = ct + d$ are linear functions of $t$. 
	- These linear parametric equations describe a straight line in the plane.
- **Shape**:
	- **Line**: The combination of these linear functions produces a straight line. The slope of the line is ca\frac{c}{a}ac​, and the intercepts are determined by bbb and ddd.
#### Quadratic Parametric Equations
- **Example**: A parabola parametrized by $t$
$$\LARGE x(t) = t, \quad y(t) = at^2 + bt + c$$
- **Explanation**: 
	- The function $g(t) = at^2 + bt + c$ is a quadratic function of $t$. 
	- It means $y$ changes quadratically with respect to $t$.
### Cubic Parametric Equations
- **Example**: A cubic curve parametrized by $t$
$$\LARGE x(t) = t, \quad y(t) = at^3 + bt^2 + ct + d$$
- **Explanation**:
	- The function $x(t) = t$ is a linear function of $t$.
	- The function $y(t) = at^3 + bt^2 + ct + d$ is a cubic function of $t$.
	- **Together**: These parametric equations describe a cubic curve in the $xy$-plane. 
		- The linear term $x(t) = t$ allows $x$ to change linearly with respect to $t$, while the cubic term in $y(t)$ determines the overall cubic shape of the curve.
### Higher-Order and Trigonometric Parametric Equations
- **Ellipse Example**
$$\LARGE x(t) = a \cos(t), \quad y(t) = b \sin(t)$$
- **Explanation**: 
	- The functions $f(t) = a \cos(t)$ and $g(t) = b \sin(t)$ are trigonometric functions of $t$. 
	- **Together**: These parametric equations describe an elliptical path in the $xy$-plane. 
		- The trigonometric terms determine the periodic nature of the ellipse.
- - - 
## Parameters
A parameter is a variable, often denoted by $t$, that varies within a specified range and determines the coordinates of points on a geometric object.
	Are the variables that control the position of points on a curve or surface.