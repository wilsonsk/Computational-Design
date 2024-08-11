# Straight Line Through a Point
## Standard Form of a Line
The general equation of a straight line in two dimensions can be written as:
$$\LARGE y = mx + b$$
   where:
   - $y$ is the dependent variable,
   - $x$ is the independent variable,
   - $m$ is the slope of the line (the rate at which $y$ changes with respect to $x$),
   - $b$ is the y-intercept (the value of $y$ when $x = 0$).
## The Standard Equation of a Line with Slope $m$ Passing Through a Point $(x_1, y_1)$
The equation $y - y_1 = m(x - x_1)$ is known as the point-slope form of a line. 
	It is derived by starting from the general form of a line and using the condition that the line passes through a specific point $(x_1, y_1)$. 
		This form is particularly useful because it directly relates the slope of the line $m$ and the coordinates of a point on the line.
##### Finding the Equation with a Specific Point
Suppose we know the slope $m$ of the line and we want the line to pass through a specific point $(x_1, y_1)$.
	We can start with the general form of the line and use the point $(x_1, y_1)$ to find $b$, the y-intercept.

1. **Using the Point to Find the Y-Intercept**:
   Substitute $x_1$ for $x$ and $y_1$ for $y$ in the general equation $y = mx + b$:
$$\LARGE y_1 = mx_1 + b$$
   To solve for $b$, rearrange this equation:
$$\LARGE b = y_1 - mx_1$$
4. **Substitute Back to Get the Point-Slope Form**:
   Now, substitute $b = y_1 - mx_1$ back into the general equation $y = mx + b$:
$$\LARGE y = mx + (y_1 - mx_1)$$
   This can be rearranged as:
$$\LARGE y - y_1 = m(x - x_1)$$
*How to calculate the [[Data/Abstract Mathematical Spaces/Physics/Analysis/Tangent Line#The Tangent Line Through a Point|tangent line through a point]]*
![[Pasted image 20240811062503.png]]
## Parametric Equation
A point $(x,y,z)$ and the origin point $(x_0,y_0,z_0)$, added to a scaling ($t$) of the directional vector ($\vec{v}$).
$$\LARGE \begin{Bmatrix} x = x_0 + v_1t \\ y = y_0 + v_2t \\ z = z_0 + v_3t\end{Bmatrix}$$
## Standard Equation for a Line Through a Point
A point $\LARGE x_0 = (x_0, y_0, z_0)$ and with a [[Data/Abstract Mathematical Spaces/Physics/Analysis/Multivariable Calculus/Partial Derivatives#Direction Vector in the Plane $y = b$|direction vector]] $\LARGE \vec{v} = (v_1, v_2, v_3)$ with all non-zero coordinates.
	Eliminate the $t$ parameter:
$$\LARGE \begin{Bmatrix} x = x_0 + v_1t \\ y = y_0 + v_2t \\ z = z_0 + v_3t\end{Bmatrix} =  \frac{x - x_0}{v_1} = \frac{y - y_0}{v_2} = \frac{z - z_0}{v_3}$$

If *for example* $\LARGE v_2 = 0$ (and $v_1, v_3 \neq 0$), produces the following equation:
$$\LARGE \frac{x-x_0}{v_1} = \frac{z-z_0}{v_3}, y = y_0$$
Here, the $y$-coordinate is **constant** for all the points on the line, which means that the line lies in the **plane** $\LARGE y = y_0$ which is **parallel** to the $\LARGE xz$-plane.

