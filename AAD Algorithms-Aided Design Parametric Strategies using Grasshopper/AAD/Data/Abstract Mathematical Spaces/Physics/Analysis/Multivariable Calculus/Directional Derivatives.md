---
up:
  - "[[Multivariable Calculus]]"
related: 
date created: 2024-07-28
---
# Directional Derivatives
*Note: a Derivative (and Partial Derivative) **is** a vector.*
	*That vector being the [[Derivatives#4. Is the Unit Tangent Vector|Unit Tangent Vector]] to a given point.*
		Therefore the Vector of the Partial Derivatives is a Unit Tangent Vector describing the direction of the function in a single dimension.
			But the **Gradient vector** describes the direction and rate of the steepest increase in a multi-dimensional space.

The main difference between the gradient and the directional derivative is how the direction is specified.
	In essence, the directional derivative is a projection of the gradient vector onto the direction given by $\mathbf{u}$. 
		It tells you how much the function changes in that specific direction, while the gradient tells you the direction and rate of the steepest change.
- **Direction**:
    - The gradient vector inherently provides the direction of the steepest ascent.
    - The directional derivative calculates the rate of change in a specified direction given by the unit vector $\mathbf{u}$.
- **Magnitude and Direction**:
    - The magnitude of the gradient vector gives the maximum rate of change at that point.
    - The directional derivative gives the rate of change in a particular direction, which depends on both the magnitude of the gradient and the cosine of the angle between the gradient and the unit vector $\mathbf{u}$.
- **Unit Vector**:
    - The directional derivative requires an arbitrary unit vector $\mathbf{u}$ to specify the direction.
    - The gradient vector itself determines its own direction.
![[Pasted image 20240705152625.png|400]]

A directional derivative measures the rate of change of the function $f(x, y)$ in a specific direction given by a vector $\mathbf{v} = (a, b)$.
	This direction can be any arbitrary direction in the $xy$-plane, not just along the $x$ or $y$ axes.

The **directional derivative** of a function $f(x, y)$ at a point $(x_0, y_0)$ in the direction of a vector $\mathbf{v} = (a, b)$ measures how $f$ changes as you move from $(x_0, y_0)$ in the direction of $\mathbf{v}$.
	It generalizes the concept of a [[Partial Derivatives|partial derivative]] to any direction, not just along the coordinate axes.

A directional derivative represents a rate of change of a function in any given direction.

$D_{u}​f(p)$ gives the rate of change of the function $f$ at the point $\mathbf{p}$ in the direction of the unit vector $\mathbf{u}$.
- - -
## The Vector Components of a Directional Derivative
### Unit Vector (i.e. Directional Vector)

The directional derivative of a function $f(x, y, z)$ in the direction of a unit vector $\LARGE \mathbf{u} = \langle u_{\cos(\alpha)}, u_{\cos(\beta)}, u_{\cos(\gamma)} \rangle$ measures the rate of change of the function in that specific direction.

The direction vector $\mathbf{u}$ makes angles $\alpha, \beta, \gammaα$ with the $x, y, z$ axes respectively, its components are:
$$\LARGE \mathbf{u} = \langle u_x, u_y, u_z \rangle = \LARGE \mathbf{u} = \langle u_{\cos(\alpha)}, u_{\cos(\beta)}, u_{\cos(\gamma)} \rangle$$
$$\LARGE u_x = \cos(\alpha), \quad u_y = \cos(\beta), \quad u_z = \cos(\gamma)$$
#### The Direction of the Unit Vector
The direction of the tangent vector is determined by the orientation you choose for measuring the rate of change or movement along the surface. 
	When you compute the directional derivative, you are essentially projecting the gradient onto the chosen direction vector.
		The unit vector $\mathbf{u}$ can be oriented in any direction, not just along the $x$-axis or the $x$-axis.
			 It is chosen based on the direction in which you want to measure the rate of change of the function.
				 For a unit vector to represent a tangent direction, it must be perpendicular to the gradient vector at the point of interest, ensuring it lies in the tangent plane.

A unit vector $\mathbf{u}$ can be oriented in any direction in 3D space. It is defined as: 
$$\mathbf{u} = \langle u_x, u_y, u_z \rangle $$
- The components $u_x, u_y$ and $u_z$​ are such that $\mathbf{u}$ has a magnitude of 1: 
$$u_x^2 + u_y^2 + u_z^2 = 1$$
**Perpendicular to the Gradient**
To find a tangent vector at a point on a surface f$f(x, y, z) = c$, the unit vector $\mathbf{u}$ must be perpendicular to the gradient vector $\nabla f$.
	This ensures that $\mathbf{u}$ lies in the tangent plane to the surface at that point.
##### Example of Choosing the Unit Vector
Consider a surface defined by $f(x, y, z) = x^2 + y^2 + z^2 - 1$ (a sphere of radius 1 centered at the origin).
###### Steps to Find a Tangent Vector at a Point
1. **Compute the Gradient**:
    $\nabla f = \left( 2x, 2y, 2z \right)$
2. **Evaluate the Gradient at a Point**:
    - At the point $(1, 0, 0)$: $\nabla f(1, 0, 0) = (2, 0, 0)$
3. **Choose a Unit Vector Perpendicular to the Gradient**:
	- To find a tangent vector, choose a unit vector $\mathbf{u}$ that is perpendicular to $(2, 0, 0)$. 
		- Any vector in the $y$-$z$ plane is perpendicular to $(2, 0, 0)$.
- For example, $\mathbf{u} = (0, 1, 0)$ or $\mathbf{u} = (0, 0, 1)$.
- - -
## Calculation of Directional Derivatives
When we talk about the directional derivative of a scalar function in the direction of a unit vector $\mathbf{u}$, we project the gradient vector $\nabla f∇$ onto $\mathbf{u}$ to determine how much of the gradient’s magnitude is in the direction of $\mathbf{u}$.

This projection is given by the dot product:

$$\LARGE D_{\mathbf{u}} f = \nabla f \cdot \mathbf{u}$$
Here, $\nabla f \cdot \mathbf{u}$ gives a scalar that tells us the rate of change of $f$ in the direction of $\mathbf{u}$.

![[Pasted image 20240708134159.png]]
*Finding the directional derivative at a point on the graph of $\LARGE z = f(x,y)$.
	The slope of the blue arrow on the graph indicates the value of the directional derivative at that point*.

The directional derivative of a function $f$ in the direction of a unit vector $\LARGE \mathbf{u} = \langle u_{\cos(\alpha)}, u_{\cos(\beta)}, u_{\cos(\gamma)} \rangle$ is a measure of the rate at which $f$ changes in that direction. 
The gradient allows us to calculate the directional derivative as follows:
$$\LARGE D_{\mathbf{u}} f = \nabla f \cdot \mathbf{u} = \frac{\partial f}{\partial x} u_{\cos(\alpha)} + \frac{\partial f}{\partial y} u_{\cos(\beta)} + \frac{\partial f}{\partial z}  u_{\cos(\gamma)}$$
- The gradient $\LARGE \nabla f$ gives the vector of partial derivatives of $f$.
- The dot product $\LARGE \nabla f \cdot \mathbf{u}$ projects the gradient vector onto the direction vector $\mathbf{u}$, yielding the rate of change of $f$ in that direction.
### Deriving
> [!note]
> We start with the graph of a surface defined by the equation $\LARGE z = f(x,y)$.
> 
> Given a point $\LARGE (a,b)$ in the domain of $f$, we ***[[#Example of Choosing the Unit Vector|choose]]*** a direction to travel from that point. 
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
>###### The Limit of the Slope of the Secant Line (i.e. The Tangent Line/Directional Derivative)
> $$\LARGE \mathbf{D}_{\vec{u}}\mathbf{f}(\mathbf{a},\mathbf{b}) = \lim \limits_{h \to 0} = \frac{f(a+h\cos\theta,\space b+h\sin\theta) - f(a,b)}{h}$$
### 1. [[Normalizing a Vector|Normalize]] the Direction Vector
Ensure the direction vector $\mathbf{v}$ is a unit vector. 
	If $\mathbf{v} = (a, b)$, normalize it by dividing by its magnitude:
$$\LARGE \mathbf{u} = \left( \frac{a}{\sqrt{a^2 + b^2}}, \frac{b}{\sqrt{a^2 + b^2}} \right)$$
### 2. Compute the [[Gradients|Gradient]]
The set of partial derivatives of a scalar function $f$ with respect to each spatial variable forms the components of the gradient vector. 
	The gradient vector $\nabla f$ is a vector field that represents the rate and direction of the fastest increase of the scalar function at every point in the domain.

Find the gradient of $f$ at the point $(x_0, y_0)$. 
	The gradient is a vector of partial derivatives:
$$\LARGE \nabla f(x_0, y_0) = \left( \frac{\partial f}{\partial x}(x_0, y_0), \frac{\partial f}{\partial y}(x_0, y_0) \right)$$
### 3. [[Statics Analysis#Dot Product (i.e. Scalar Product)|Dot **Product**]]
The Dot Product [[projects|projects]] the Gradient Vector onto the Unit Vector, which gives the component of the Gradient in the direction of the Unit Vector. 

The directional derivative is **the dot product of the gradient vector and the unit vector**, reflecting how much of the gradient’s magnitude is in the direction of $\mathbf{u}$.

The directional derivative $D_{\mathbf{u}}f$ is obtained by taking the dot product of the gradient $\nabla f$ and the unit vector $\mathbf{u}$. 
	This operation projects the gradient vector onto the direction specified by $\mathbf{u}$, giving the rate of change of the scalar function $f$ in that direction.
		This projection tells us how fast the function $f$ is increasing in that specific direction.

The partial derivatives $\frac{\partial f}{\partial x_i}$ represent changes along the coordinate axes, not in the direction of $\mathbf{u}$. 
	The unit vector $\mathbf{u}$ might point in a completely different direction.
		 The directional derivative projects the gradient (which consists of these partial derivatives) onto the direction of $\mathbf{u}$ to find the rate of change in that specific direction.
			When $\mathbf{u}$ is in the same direction as $\nabla f$ ($\theta = 0$), the dot product is maximized.

$$\LARGE \text{The Dot Product between two vectors a and b:}$$
$$\LARGE a \cdot b = \|a\| \|b\| \cos \theta$$
$$\text{Where } \theta \text{ is the angle between the two vectors.}$$
$$\LARGE \text{For the gradient }\nabla f \text{ and the unit vector }\mathbf{u}:$$
$$\LARGE \nabla f \cdot \mathbf{u} = \|\nabla f\| \|\mathbf{u}\| \cos \theta = \|\nabla f\| \cos \theta$$
$$\LARGE \text{since }\|\mathbf{u}\| = 1$$
Take the dot product of the gradient vector and the normalized direction vector:
$$\LARGE D_{\mathbf{u}} f(x_0, y_0) = \nabla f(x_0, y_0) \cdot \mathbf{u}$$
### Result
$$\LARGE D_{\mathbf{u}} f(x_0, y_0) = \frac{\partial f}{\partial x}(x_0, y_0) \cdot \frac{a}{\sqrt{a^2 + b^2}} + \frac{\partial f}{\partial y}(x_0, y_0) \cdot \frac{b}{\sqrt{a^2 + b^2}}$$
#### The Reasoning Behind Utilizing the [[Dot Product|Dot Product]]
As a means to compute the Directional Derivative.

The reasoning behind using the dot product to compute the directional derivative is rooted in the geometric interpretation of vectors and [[Projection|projections]]. 
	The gradient vector $\nabla f$ represents the direction and rate of the steepest increase, while the unit vector $\mathbf{u}$ specifies the desired direction of change. 
		The dot product projects the gradient onto this direction, yielding the rate at which the function $f$ changes as we move in the direction of $\mathbf{u}$.
			 This method leverages the inherent properties of the dot product to capture the directional aspect of the rate of change effectively.

When it comes to directional derivatives, the concept of projection via the dot product becomes very useful. The directional derivative of a scalar field $f$ in the direction of a unit vector $u$ is given by the dot product of the gradient of $f$ and the unit vector $u$:

$$D_{u} f = \nabla f \cdot u$$
Here’s why this works:
##### Computing the Directional Derivative
The directional derivative of $f$ in the direction of $\mathbf{u}$ measures the rate at which $f$ changes as we move in the direction specified by $\mathbf{u}$.
	This can be visualized as how much the scalar function $f$ is increasing in the direction of $\mathbf{u}$.
###### Gradient Vector $\nabla f$
- The gradient vector $\nabla f$ points in the direction of the steepest increase of the function $f$.
- Its magnitude represents the rate of increase in that direction.
##### Computing the [[Static Equilibrium#Unit Vector|Unit Vector]]
A unit vector $\mathbf{u}$ specifies a particular direction in space and has a magnitude of 1. 
	The unit vector is used to indicate the direction in which we want to measure the rate of change of the function. $u$
		A unit vector $u$ has a magnitude of 1 and indicates the direction in which we want to find the derivative.
##### Utilizing the Dot Product 
By taking the dot product of the gradient $\nabla f$ with the unit vector $\mathbf{u}$, we effectively [[Projection#Vector Projection|project]] the gradient vector onto $\mathbf{u}$. 
	This projection tells us how much of the gradient's magnitude is in the direction of $\mathbf{u}$, which is precisely the rate of change of $f$ in that direction.
		The dot product $\nabla f \cdot u$ measures how much of the gradient vector $\nabla f$ lies in the direction of $u$.
			This gives us the rate of change of $f$ in the direction of $u$.
### Example Calculation
Suppose $f(x, y) = x^2 + y^2$ and we want to find the directional derivative at $(1, 1)$ in the direction of the vector, $\vec{v}$ $(1, 2)$.
1. **[[Static Equilibrium#Normalizing Vectors (i.e. unit vectors)|Normalize]] the Direction Vector**:
$$\LARGE \mathbf{v} = (1, 2) \implies \|\mathbf{v}\| = \sqrt{1^2 + 2^2} = \sqrt{5}$$
$$\LARGE \left( \frac{1}{\sqrt{1^2 + 2^2}}\right),\left(\frac{2}{\sqrt{1^2+2^2}}\right)$$
$$\LARGE \mathbf{u} = \left( \frac{1}{\sqrt{5}}, \frac{2}{\sqrt{5}} \right)$$

2. **Compute the Gradient**:

$$\LARGE \nabla f(x, y) = \left( \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y} \right) = (2x, 2y)$$

##### A. At the Point $(1, 1)$:
$$\LARGE D_{\mathbf{u}} f(x, y) = \nabla f(x, y) \cdot \mathbf{u}$$
1. **Substituting the $x,y$ points for $\nabla f(x, y)$ and $\mathbf{u}$**
$$\LARGE \nabla f(1, 1) = (2 \cdot 1, 2 \cdot 1) = (2, 2)$$

2. **Compute the Dot Product**:
$$\LARGE D_{\mathbf{u}} f(1, 1) = \nabla f(1, 1) \cdot \mathbf{u} = (2, 2) \cdot \left( \frac{1}{\sqrt{5}}, \frac{2}{\sqrt{5}} \right)$$

3. **Result**:
$$\LARGE D_{\mathbf{u}} f(1, 1) = 2 \cdot \frac{1}{\sqrt{5}} + 2 \cdot \frac{2}{\sqrt{5}} = \frac{2}{\sqrt{5}} + \frac{4}{\sqrt{5}} = \frac{6}{\sqrt{5}}$$
##### B. As a Vector-Valued Function
To find the directional derivative as a vector function rather than evaluating it at a single point, you need to express the directional derivative in terms of the general coordinates $(x, y)$. 
$$\LARGE D_{\mathbf{u}} f(x, y) = \nabla f(x, y) \cdot \mathbf{u}$$
1. **Substituting the expressions for $\nabla f(x, y)$ and $\mathbf{u}$**
$$\LARGE D_{\mathbf{u}} f(x, y) = (2x, 2y) \cdot \left( \frac{1}{\sqrt{5}}, \frac{2}{\sqrt{5}} \right)$$
2. **Compute the Dot Product**:
   The dot product of the gradient and the unit vector is:
$$\LARGE D_{\mathbf{u}} f(x, y) = 2x \cdot \frac{1}{\sqrt{5}} + 2y \cdot \frac{2}{\sqrt{5}}$$
$$\LARGE D_{\mathbf{u}} f(x, y) = \frac{2x}{\sqrt{5}} + \frac{4y}{\sqrt{5}}$$
3. **Simplify the Expression**:
   Combining the terms, the directional derivative as a vector function is:
$$\LARGE D_{\mathbf{u}} f(x, y) = \frac{2x + 4y}{\sqrt{5}}$$

Therefore, the directional derivative of $f(x, y) = x^2 + y^2$ in the direction of the vector $\mathbf{v} = (1, 2)$, expressed as a function of $(x, y)$, is:
$$\LARGE D_{\mathbf{u}} f(x, y) = \frac{2x + 4y}{\sqrt{5}}$$
And, the vector form of the directional derivative of $f(x, y) = x^2 + y^2$ in the direction of the vector $\mathbf{v} = (1, 2)$, expressed as a function of $(x, y)$, is: $$\LARGE \mathbf{D}_{\mathbf{u}} f(x, y) = \left< \frac{2x}{\sqrt{5}}, \frac{4y}{\sqrt{5}} \right> = \begin{pmatrix}\frac{2x}{\sqrt{5}} \\ \frac{4y}{\sqrt{5}} \end{pmatrix}$$
### Special Cases
1. When $\mathbf{v}$ is aligned with the $x$-axis ($\mathbf{v} = (1, 0)$), the directional derivative simplifies to the partial derivative with respect to $x$:
$$\LARGE D_{\mathbf{v}} f = \frac{\partial f}{\partial x}$$ 

2. When $\mathbf{v}$ is aligned with the $y$-axis ($\mathbf{v} = (0, 1)$), the directional derivative simplifies to the partial derivative with respect to $y$:
$$\LARGE D_{\mathbf{v}} f = \frac{\partial f}{\partial y}$$
- - -
## How the Gradient Uses Partial Derivatives to Calculate the Directional Derivative
> [!note]
> ##### 1. Directional Derivative
> The directional derivative of a function $f$ in the direction of a unit vector $\LARGE \mathbf{e} = \langle e_x, e_y, e_z \rangle$ is a measure of the rate at which $f$ changes in that direction. 
> The gradient allows us to calculate the directional derivative as follows:
> $$\LARGE D_{\mathbf{e}} f = \nabla f \cdot \mathbf{e} = \frac{\partial f}{\partial x} e_x + \frac{\partial f}{\partial y} e_y + \frac{\partial f}{\partial z} e_z$$
> Where:
> $\LARGE D_{e}f$ gives the rate at which the function $f$ changes as you move from a point in the direction of $\mathbf{e}$.​
> 
> Here’s how this works:
> - The gradient of scalar field $\LARGE \nabla f$ gives the vector field containing partial derivatives of $f$.
> - The dot product $\LARGE \nabla f \cdot \mathbf{e}$ projects the gradient vector onto the direction vector $\mathbf{e}$, yielding the rate of change of $f$ in that direction.
> ##### 2. Finding Maximal Increase
> The gradient points in the direction of the steepest ascent of the scalar field $f$. 
> By knowing the gradient, one can determine how to move in space to increase the function $f$ most rapidly.

![[Pasted image 20240721131026.png]]
![[Pasted image 20240721131807.png]]
- - -
