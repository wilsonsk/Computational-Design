---
up:
  - "[[Multivariable Calculus]]"
related: 
date created: 2024-07-28
---
# Directional Derivatives
![[Pasted image 20240705152625.png|400]]

A directional derivative measures the rate of change of the function $f(x, y)$ in a specific direction given by a vector $\mathbf{v} = (a, b)$.
	This direction can be any arbitrary direction in the $xy$-plane, not just along the $x$ or $y$ axes.

The **directional derivative** of a function $f(x, y)$ at a point $(x_0, y_0)$ in the direction of a vector $\mathbf{v} = (a, b)$ measures how $f$ changes as you move from $(x_0, y_0)$ in the direction of $\mathbf{v}$.
	It generalizes the concept of a [[Partial Derivatives|partial derivative]] to any direction, not just along the coordinate axes.

A directional derivative represents a rate of change of a function in any given direction.

$D_{u}​f(p)$ gives the rate of change of the function $fff$ at the point $\mathbf{p}$ in the direction of the unit vector $\mathbf{u}$.

- - -
## Calculation of Directional Derivatives
![[Pasted image 20240708134159.png]]
*Finding the directional derivative at a point on the graph of $\LARGE z = f(x,y)$.
	The slope of the blue arrow on the graph indicates the value of the directional derivative at that point*.

> [!note] 
> The directional derivative of a function $f(x, y, z)$ in the direction of a unit vector $\LARGE \mathbf{u} = \langle u_x, u_y, u_z \rangle$ measures the rate of change of the function in that specific direction.
> 	- The direction vector $\mathbf{u}$ makes angles $\alpha, \beta, \gammaα$ with the $x, y, z$ axes respectively, its components are: $$\LARGE u_x = \cos(\alpha), \quad u_y = \cos(\beta), \quad u_z = \cos(\gamma)$$
> **Calculation**: The directional derivative of $f$ in the direction of $\mathbf{u}$ is given by the **dot product** of the **gradient** of $f$ at $\mathbf{p}$ and the **unit vector** $\mathbf{u}$:
> $$\LARGE D_{\mathbf{u}} f = \nabla f \cdot \mathbf{u} = \frac{\partial f}{\partial x} \cos(\alpha) + \frac{\partial f}{\partial y} \cos(\beta) + \frac{\partial f}{\partial z} \cos(\gamma)$$


> [!note]
> ### Deriving
> We start with the graph of a surface defined by the equation $\LARGE z = f(x,y)$.
> 
> Given a point $\LARGE (a,b)$ in the domain of $f$, we choose a direction to travel from that point. 
> We measure the direction using the angle $\LARGE \theta$, which is measured counterclockwise in the $xy$-plane, starting at $zero$ from the positive $x$-axis.
> ###### $\LARGE h$ (i.e. and interval): The distance traveled.
> ###### [[Static Equilibrium#Unit Vector|Unit Vector]], $\LARGE \vec{u} = (\cos\theta)\hat{i} + (\sin\theta)\hat{j}$: The direction of travel.
> Trigonometric functions help break down a vector into orthogonal components along the coordinate axes.
> - This isolation allows for the analysis of the vector's effect along each axis independently, simplifying complex vector problems.
> 	- $cos$ and $⁡\sin$ ensure that the magnitude of the original vector is preserved when summing its components.
> 
> Using the combination of these $\cos\theta$ and $\sin\theta$ components for direction of $\vec{u}$, can isolate or extract the change or magnitude along specific axes or directions.
> - $\LARGE \cos\theta$ gives the projection of the unit vector on the $x$-axis.
> 	- If $\theta = 0$, $\cos 0 = 1$, and we move entirely in the $x$-direction.
> - $\LARGE \sin \theta$ gives the projection of the unit vector on the $y$-axis.
> 	- If $\LARGE \theta = \frac{\pi}{2}$​, $\LARGE \sin \frac{\pi}{2} = 1s$, and we move entirely in the $y$-direction.
>
> Therefore, the $z$-coordinate of the second point on the graph is given by: 
> $\LARGE z = f(a+\cos\theta, b+h\sin\theta)$.
> ###### Slope of the Secant Line
> $$\LARGE m_{secant} = \frac{f(a+h\cos\theta,\space b+h\sin\theta) - f(a,b)}{h}$$
To find the slope of the tangent line in the same direction, we take the limit as $\LARGE h$ approaches zero.
### 1. [[Statics Analysis#Static Equilibrium Norm of a Vector Magnitude|Normalize]] the Direction Vector
Ensure the direction vector $\mathbf{v}$ is a unit vector. 
	If $\mathbf{v} = (a, b)$, normalize it by dividing by its magnitude:
$$\LARGE \mathbf{u} = \left( \frac{a}{\sqrt{a^2 + b^2}}, \frac{b}{\sqrt{a^2 + b^2}} \right)$$
### 2. Compute the [[Gradients|Gradient]]
Find the gradient of $f$ at the point $(x_0, y_0)$. 
	The gradient is a vector of partial derivatives:
$$\LARGE \nabla f(x_0, y_0) = \left( \frac{\partial f}{\partial x}(x_0, y_0), \frac{\partial f}{\partial y}(x_0, y_0) \right)$$
### 3. [[Statics Analysis#Dot Product (i.e. Scalar Product)|Dot Product]]
The directional derivative is the dot product of the gradient vector and the unit vector, reflecting how much of the gradient’s magnitude is in the direction of $\mathbf{u}$.

Take the dot product of the gradient vector and the normalized direction vector:
$$\LARGE D_{\mathbf{u}} f(x_0, y_0) = \nabla f(x_0, y_0) \cdot \mathbf{u}$$
### Result
$$\LARGE D_{\mathbf{u}} f(x_0, y_0) = \frac{\partial f}{\partial x}(x_0, y_0) \cdot \frac{a}{\sqrt{a^2 + b^2}} + \frac{\partial f}{\partial y}(x_0, y_0) \cdot \frac{b}{\sqrt{a^2 + b^2}}$$
### Example Calculation
Suppose $f(x, y) = x^2 + y^2$ and we want to find the directional derivative at $(1, 1)$ in the direction of the vector $(1, 2)$.
1. **Normalize the Direction Vector**:
$$\LARGE \mathbf{v} = (1, 2) \implies \|\mathbf{v}\| = \sqrt{1^2 + 2^2} = \sqrt{5}$$

$$\LARGE \mathbf{u} = \left( \frac{1}{\sqrt{5}}, \frac{2}{\sqrt{5}} \right)$$

2. **Compute the Gradient**:

$$\LARGE \nabla f(x, y) = \left( \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y} \right) = (2x, 2y)$$

At the point $(1, 1)$:

$$\LARGE \nabla f(1, 1) = (2 \cdot 1, 2 \cdot 1) = (2, 2)$$

3. **Dot Product**:
$$\LARGE D_{\mathbf{u}} f(1, 1) = \nabla f(1, 1) \cdot \mathbf{u} = (2, 2) \cdot \left( \frac{1}{\sqrt{5}}, \frac{2}{\sqrt{5}} \right)$$


$$\LARGE D_{\mathbf{u}} f(1, 1) = 2 \cdot \frac{1}{\sqrt{5}} + 2 \cdot \frac{2}{\sqrt{5}} = \frac{2}{\sqrt{5}} + \frac{4}{\sqrt{5}} = \frac{6}{\sqrt{5}}$$
### Relationship Between Directional and Partial Derivatives
The directional derivative can be expressed in terms of the partial derivatives. 
	Specifically, if you have a function $f(x, y)$ and a direction vector $\mathbf{v} = (a, b)$, the directional derivative $D_{\mathbf{v}} f$ in the direction of $\mathbf{v}$ is given by:
$$\LARGE D_{\mathbf{v}} f(x_0, y_0) = \nabla f(x_0, y_0) \cdot \mathbf{u}$$

where $\mathbf{u} = \left( \frac{a}{\sqrt{a^2 + b^2}}, \frac{b}{\sqrt{a^2 + b^2}} \right)$ is the unit vector in the direction of $\mathbf{v}$, and $\nabla f(x_0, y_0)$ is the gradient of $f$ at the point $(x_0, y_0)$, which consists of the partial derivatives:

$$\LARGE \nabla f(x_0, y_0) = \left( \frac{\partial f}{\partial x}(x_0, y_0), \frac{\partial f}{\partial y}(x_0, y_0) \right)$$

Therefore, the directional derivative can be written as:

$$\LARGE D_{\mathbf{v}} f(x_0, y_0) = \frac{\partial f}{\partial x}(x_0, y_0) \cdot \frac{a}{\sqrt{a^2 + b^2}} + \frac{\partial f}{\partial y}(x_0, y_0) \cdot \frac{b}{\sqrt{a^2 + b^2}}$$

### Special Cases

- When $\mathbf{v}$ is aligned with the $x$-axis ($\mathbf{v} = (1, 0)$), the directional derivative simplifies to the partial derivative with respect to $x$:
\[
D_{\mathbf{v}} f = \frac{\partial f}{\partial x}
\]

- When $\mathbf{v}$ is aligned with the $y$-axis ($\mathbf{v} = (0, 1)$), the directional derivative simplifies to the partial derivative with respect to $y$:
\[
D_{\mathbf{v}} f = \frac{\partial f}{\partial y}
\]

Directional derivatives measure the rate of change of a function in any given direction and generalize the concept of partial derivatives to arbitrary directions.
