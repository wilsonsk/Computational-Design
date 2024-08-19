---
up:
  - "[[Multivariable Calculus]]"
related: 
date created: 2024-07-28
---
# Gradients
##### *Note: Context-Dependent Terminology*
*If the Gradient is of a [[Abstract Mathematical Spaces#Scalar Functions|Scalar Function]], then it is itself a [[Abstract Mathematical Spaces#Vector Function|Vector Function]].*
	*But if the Gradient is of a [[Abstract Mathematical Spaces#Scalar Fields|Scalar Field]], then it is itself a [[Abstract Mathematical Spaces#Vector Fields|Vector Field]].*

*And that context is depending on the domain of the Scalar Function/Field and Vector Function/Field.*
	*I.e. Whether or not the domain is [[Abstract Mathematical Spaces#"Space" vs. "Spatial"|"spatial"]] or not.*

*The Gradient itself only exists relative to a Scalar Function (or Scalar Field).*
	*Therefore, the Gradient as a word, is "short for", Gradient of a Scalar Function (or Scalar Field).*
##### *Note: Gradients in Relation to Derivatives*
###### *Partial Derivatives*
*When learning about derivatives, you typically start with functions of a single variable. As you move to functions of multiple variables (like scalar fields), you learn about partial derivatives.*

- ***Definition**: The partial derivative of a scalar field $f(x, y, z)$ with respect to $x$ is denoted by $\frac{\partial f}{\partial x}$. It measures how $f$ changes as $x$ changes, while $y$ and $z$ are held constant.*
###### *Gradient*
*The gradient of a scalar field extends the concept of a derivative to multiple dimensions, providing a vector that points in the direction of the steepest increase of the scalar field.*
##### *Note: Nabla Operator ($\nabla$)*
*Etymology: The Harp in Greek*
*The Nabla operator is a vector differential operator that, when applied to a scalar or vector field, produces different types of derivatives.* 
	*Its a vector whose components are partial derivatives with respect to the spatial coordinates.* 
		*In three dimensions, the Nabla operator is defined as:*
*$$\LARGE \nabla = (\frac{\partial}{\partial x}, \frac{\partial}{\partial y}, \frac{\partial}{\partial z})$$*
*The Nabla Operator by itself doesn't mean anything.*
	*It must act on a function.*
###### *Applying the Nabla Operator to a Scalar Function: Gradient*
*When the Nabla operator $\nabla$ is applied to a scalar function $f$, it produces the gradient of $f$.*
	*The gradient is a vector that contains all the first-order partial derivatives of $f$.* 
		*If $f$ is a function of $n$ variables, the gradient $\nabla f$ is given by:*
*$$\LARGE \nabla f=(\frac{\partial f}{d x_{1}},\frac{\partial f}{d x_{2}}, \ldots \frac{\partial f}{d x_{n}}​)$$*
*This gradient vector points in the direction of the steepest increase of the function and its magnitude represents the rate of this increase.*

- - -
## Gradient Defined
The Gradient is the several-variable counterpart of the first derivative.
	An **increase** or **decrease** in the **magnitude** of a **property**, relative to some variable (time, position, etc.).

Let $\LARGE f: \mathbb{R}^n \to \mathbb{R}$  be a partially differentiable function of $\LARGE n$ variables.
	Then the gradient of $\LARGE f$ in the point $\LARGE \vec{x}$ is the following vector: 
$$\LARGE grad \space f(\vec{x}) = \nabla f(\vec{x}) = (\frac{\partial f}{d x_{1}}(\vec{x}),\frac{\partial f}{d x_{2}}(\vec{x}), \ldots \frac{\partial f}{d x_{n}}(\vec{x})​)$$
		Where the Gradient is a [[Abstract Mathematical Spaces#Vector Fields|Vector Field]] (a function from $\LARGE \mathbb{R}^n \to \mathbb{R}^n$).
			Where $\LARGE \vec{x}$ is a **Spatial Point** from $\LARGE \mathbb{R}^n$ with its coordinates contained in a vector form. 
				That is, a function with a domain of scalar "spatial" values that maps each spatial scalar to a vector in the codomain.

*Note: a Derivative (and Partial Derivative) **is** a vector.*
	*That vector being the [[Derivatives#4. Is the Unit Tangent Vector|Unit Tangent Vector]] to a given point.*
		That is, the vector contains the coordinates of a slope of a line that is tangent to the point. 
			Therefore the [[Partial Derivatives#Compute a Direction Vector, $ LARGE vec{v}$|Vector of the Partial Derivatives is a Unit Tangent Vector]] describing the direction of the function in a single dimension.
				But the **Gradient vector** describes the direction and rate of the steepest increase in a multi-dimensional space.

A Gradient is a special case of the [[Jacobian Matrix|Jacobian Matrix]].
## The Gradient as the Slope $\LARGE m$
The Gradient is the **Slope** of the [[Planes#Tangent Plane to the Surface $z=f(x,y)$ in the point $(a,b,f(a,b))$|Tangent Plane Equation]].

The $1\times 2$ Vector that is composed of the Partial Derivatives for a given point, is itself the [[Gradients|Gradient]] of the function $\LARGE f$ at point $(a,b)$, $\LARGE  \nabla f(a,b) = \begin{bmatrix}(\frac{\partial f}{d x}(a,b),\frac{\partial f}{d y}(a,b)\end{bmatrix}$. 
	I.e. The scalars produced from the evaluated Partial Derivatives, are coordinates of the Gradient at point $(a,b)$. 

And the Increments $(x-a)$ and (y-b), in the $\LARGE x$ and $\LARGE y$ direction, can also be coordinates in some separate column vector (i.e. a $2 \times 1$ vector), $\LARGE \begin{bmatrix} x-a \\ y-b \end{bmatrix}$. 
	Therefore, the Tangent Plane Equation can be reconfigured.
$$\LARGE \text{Tangent Plane } z = f(a,b) + [f'_x(a,b),f'_y(a,b)] \cdot \begin{bmatrix} x-a \\ y-b \end{bmatrix}$$
$$\LARGE == z = f(a,b) + \nabla f(a,b) \cdot \begin{bmatrix} x-a \\ y-b\end{bmatrix}$$
$$\text{Compared to Standard Form of a Line } y = mx +b$$
		Where the two vectors are then arranged to produce the [[Dot Product|Dot Product]] between them. 
			And the result is the that the **Gradient** itself becomes the representation of the slope $\LARGE m$, and  the new $2 \times 1$ vector is the **increment**.  
## Gradient at Each Point is Perpendicular to the Tangent Vector on [[#Level Curves|Level Curve]] at this Point
![[Pasted image 20240816222319.png]]

![[Pasted image 20240816130841.png]]
*Each vector shows the value of the gradient at a given point for a given function.*

The gradient of a scalar field is a [[Mapping#Higher-Level Functions (i.e. Composite Functions) Higher-Level Functions|vector field]] that points in the direction of the greatest rate of increase of the scalar field and whose magnitude is the rate of increase in that direction.
	==**The gradient $\nabla f$ is a vector field that points radially outward from the origin and whose magnitude increases with distance from the origin.==**
		The phrase "the gradient of a scalar field" specifically refers to the vector field that is derived from a scalar field by taking its partial derivatives. 
			This gradient vector field indicates the direction and rate of the greatest increase of the scalar field at each point in space.
### What "Greatest Increase of $f$" Means
![[Pasted image 20240724234502.png]]
The directional derivative is maximized when $\mathbf{u}$ is in the same direction as $\nabla f$. 
Each component (partial derivative) measures the rate of change of the function $f$ in one of the coordinate directions (x, y, z).
	Thus, the gradient vector $\nabla f$ points in the direction where $f$ increases most rapidly.
		The magnitude of the gradient vector $|\nabla f|$ represents the rate of change of $f$ in the direction of the gradient.
			A larger magnitude means a steeper ascent.
				The magnitude of the gradient vector $\nabla f(x_0, y_0)\|$ represents the maximum rate of increase of the function at that point.
					The gradient vector points in the direction in which the function fff increases most rapidly.
						This direction is not necessarily aligned with any single coordinate axis (i.e., not necessarily along the x, y, or z direction alone) but is a combination of all three.
#### Think of the $z$ Value aka the $f(x,y$) Output Value as the "Height"
1. **Surface and Tangent Plane**:
    - Imagine you are standing on a hill (the surface).
    - The tangent plane at your feet is a flat surface that touches the hill exactly at that point. This plane represents all possible directions you can move without changing your height (to the first order).
2. **Gradient Vector**:
    - The gradient vector at your feet points directly uphill, indicating the direction of the steepest ascent.
    - This direction is perpendicular to the flat tangent plane because moving in any direction within the tangent plane does not change your height significantly.
	- This normal direction is the direction of steepest ascent, meaning moving in this direction increases the function value ($f(,x,y)$ or $z$) most rapidly.
		- Moving in the direction of the gradient vector means moving in the direction where the function increases, i.e., moving uphill on the surface.
			- While the gradient vector points away from the tangent plane, it does so in a way that aligns with moving uphill on the surface, not away from the surface as a whole.
###### Perpendicularity and Steepest Ascent
The key point is that the gradient vector being perpendicular to the tangent plane means it is pointing out of the plane in the direction where the function increases most rapidly. Here’s why:
1. **Direction of No Change**:
    - Moving along any direction within the tangent plane results in no significant change in the function value (height of the hill). These are directions of zero instantaneous change.
2. **Direction of Maximum Change**:
    - The gradient vector points out of this plane, indicating the direction in which the function value (height) increases most rapidly. This is the direction of steepest ascent.
### Therefore, the Gradient Vector $\nabla f$ at a point on a level curve (or level surface) is **Perpendicular** to the Tangent *Plane* (not the tangent vector) of that point
I.e. The gradient vector is normal (perpendicular) to the tangent plane at a given point on a surface.
![[Pasted image 20240724232114.png|400]]
This perpendicularity of the gradient vector to the tangent plane of the level curve (or surface) at a point is what causes the gradient vector to point in the direction of the greatest increase in the scalar function $f$.
#### Tangent Plane
$$\LARGE \text{Tangent Plane to the Surface } z = f(x,y) \text{ in the Point } (a, b , f(a,b))$$
$$\LARGE z = f(a,b) + \frac{\partial f}{\partial x}(a,b) (x-a) + \frac{\partial f}{\partial y}(a,b)(y-b)$$
The tangent plane at a point $(x_0, y_0, z_0)$ on the surface $z = f(x, y)$ can be described by all vectors that lie in the plane defined by the partial derivatives at that point.
	It is spanned by two basis vectors corresponding to the partial derivatives with respect to $x$ and $y$.
		  At a point $(x_0, y_0, z_0)$ on a surface $z = f(x, y)$, the tangent plane is a plane that best approximates the surface at that point.
		    The tangent plane is defined by the partial derivatives $\frac{\partial f}{\partial x}$ and $\frac{\partial f}{\partial y}$.
##### Tangent Plane Basis Vectors

The tangent plane at a point $(x_0, y_0)$ can be spanned by the following basis vectors:

###### Basis Vector for $x$-direction:
$$
T_x = \left( 1, 0, \frac{\partial f}{\partial x} \right)
$$
###### Basis Vector for $y$-direction:
$$
T_y = \left( 0, 1, \frac{\partial f}{\partial y} \right)
$$
###### Tangent Plane Equation
Combining these basis vectors, any vector $T$ in the tangent plane can be written as:
$$
T = a T_x + b T_y = a \left( 1, 0, \frac{\partial f}{\partial x} \right) + b \left( 0, 1, \frac{\partial f}{\partial y} \right)
$$

#### Level Curves
The curves along which the function achieves the same value.
$$\LARGE \text{Where } \textcolor{red}{z} = f(x,y) = \text{ constant } c$$
	I.e. A Level Curve of $\LARGE f$ on level $\LARGE c$.
$$\LARGE \text{Let } f: D \to \mathbb{R} \text{ where } D \subset \mathbb{R}^2 \text{ and } c \in \mathbb{R}$$
$$\LARGE \textcolor{lightblue}{L_c = \begin{Bmatrix} (x,y) \in D : f(x,y) = c \end{Bmatrix}}$$
What this implies is that the velocity of a position is constant, that is, it has no change in value and thus no acceleration. 
![[Pasted image 20240816223947.png]]
![[Pasted image 20240816221307.png]]
![[Pasted image 20240816221430.png]]
![[Pasted image 20240816221459.png]]
![[Pasted image 20240816222319.png]]
![[Pasted image 20240816222501.png]]
Level curves (or contour lines) are curves along which the function f(x,y)f(x, y)f(x,y) takes on a constant value, i.e., f(x,y)=cf(x, y) = cf(x,y)=c.
	They are found by slicing the surface with horizontal planes z=cz = cz=c.
##### Relationships Between Gradient, Tangent Plane, and Level Curves
1. **Gradient Vector and Tangent Plane**:
    - The gradient vector at a point on the surface z=f(x,y)z = f(x, y)z=f(x,y) is perpendicular (normal) to the tangent plane at that point.
    - This perpendicularity means the gradient vector points directly away from the tangent plane, indicating the direction of steepest ascent on the surface.
2. **Gradient Vector and Level Curves**:
    - The gradient vector is also perpendicular to the level curves of the function f(x,y)f(x, y)f(x,y).
    - This perpendicularity means the gradient vector points in the direction of the steepest increase in f(x,y)f(x, y)f(x,y) as you move away from the level curve.
#### Calculating Perpendicularity
##### Dot Product (Gradient $\cdot$ Tangent Vector)
For the gradient vector $\nabla f$ to be perpendicular to the tangent vector $T$, their dot product must be zero:

$$
\nabla f \cdot T = \left( \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}, -1 \right) \cdot \left( \Delta x, \Delta y, \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y \right) = 0
$$

Performing the dot product calculation:

$$
\nabla f \cdot T = \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y - \left( \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y \right)
$$

Simplifying, we get:

$$
\nabla f \cdot T = \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y - \frac{\partial f}{\partial x} \Delta x - \frac{\partial f}{\partial y} \Delta y = 0
$$
Hence, the dot product is zero, confirming that $\nabla f$ is perpendicular to $T$.

Therefore, the gradient vector $\nabla f$ is a Vector Field (i.e. specific vector function) composed of the partial derivatives (differentials) of the scalar function $f$, and this is why it inherently points in the direction of the steepest ascent and is perpendicular to the level curves (or surfaces) of $f$.
	Each partial derivative is a _scalar_. It is simply a rate of change.
- The gradient vector $\nabla f$ at a point $(x_0, y_0)$ is **perpendicular** to the tangent vector of the level curve at that point.
	- And therefore, the Gradient always points along the direction of the steepest slope.

A Gradient (of a Scalar Function/Field) is ***itself*** a **[[Abstract Mathematical Spaces#Vector Fields|Vector Function/Field]]** (depending on context).
	Therefore, the Gradient of a Scalar Function/Field, as a Vector Function/Field, maps points (also vectors which can be represented by those points) from a given domain to vectors in a given codomain.
		A **Gradient** through its mappings, at every point in the domain, produces a [[Vectors|vector]] that encapsulates how a [[Mapping#A Function as a Subset of Mappings ($1 1$, $m 1$)|function]] changes at a given point in its [[Mapping#Domain as a Subset of the Underlying Set|domain]]. 
			It indicates both the direction and the rate of the steepest ascent of the function.
				The concept of a gradient is fundamental in multivariable calculus and has applications in various fields such as physics, engineering, and optimization.

[[Mapping#Derived from Scalar Functions (General Sense)|The Gradient of a Scalar Function]] $f$, denoted as $\nabla f$, is a [[Abstract Mathematical Spaces#Vector Fields|vector field]] that points in the direction of the greatest rate of increase of the function. 
	The gradient is constructed from the partial derivatives of the scalar field.
		I.e. The [[Components of Motion|components]] of those produced Vectors are the [[Partial Derivatives|Partial Derivatives]] of the Scalar Function $f$ as each input variable changes (i.e. in respect to each input variable).
			Therefore, the Gradient of the Scalar Function is a set of Vectors each composed of the Partial Derivatives (as Vector components)
$$\LARGE \nabla f = \left< \frac{\partial f}{\partial x_1}, \frac{\partial f}{\partial x_2}, \ldots, \frac{\partial f}{\partial x_n} \right> $$
$$\LARGE \nabla f(x,y,z) = \begin{pmatrix} \frac{\partial}{\partial_x}f(x,y,z)\\ \frac{\partial}{\partial_y}f(x,y,z) \\ \frac{\partial}{\partial_z}f(x,y,z)\end{pmatrix}$$
For any point in the domain of a function $f$, the gradient vector at that point is perpendicular (orthogonal) to the tangent vector at that point.

$\LARGE \nabla$ is the [[#Nabla Operator ($ nabla$)|Nabla Operator]].
	The magnitude of the gradient vector $|\nabla f (\mathbf{p})|$ represents the greatest rate of increase of $f$ at $\mathbf{p}$
- **Scalar Field as the Starting Point**:
	- We begin with a scalar field, which is a function $f$ that assigns scalar values to points in space.
- **Gradient as Derived Vector Field**: 
	- The gradient $\nabla f$ is a vector field derived from the scalar field $f$. 
	- Each component of the gradient vector is a partial derivative of the scalar field with respect to one of the coordinates.
### Gradient Over the Domain (Vector Field)
When you compute the gradient at every point in the domain of the function $f$, you get a vector field.
	This means that at each point $\mathbf{x}$ in the domain, there is a corresponding gradient vector $\nabla f(\mathbf{x})$.
		In other words, for each point $(x, y, z)$ where the scalar function $f$ is defined, the gradient $\nabla f$ provides a vector.
			The collection of these vectors over the entire domain forms a vector field.
				 Each vector in this field indicates the direction and rate of the fastest increase of the scalar function at its corresponding point.
					 These vectors collectively form a vector field, that is, these vectors at each point together form the gradient vector field.
##### Example
Consider the scalar function $f(x, y) = x^2 + y^2$.
Over the entire domain, the gradient is:
$$\LARGE \nabla f(x, y) = \left< 2x, 2y \right>$$
This expression represents a vector field. 
	For each point $(x, y)$ in the domain, there is a corresponding gradient vector $(2x, 2y)$.
### Gradient at a Point (i.e. a Single Vector)
The Gradient of a scalar function at a specific point in the domain is a vector whose components are the partial derivatives at that point. 
	This vector points in the direction of the greatest rate of increase (i.e. the steepest ascent of the function) of the function at that point, and its magnitude represents the rate of this increase of the function.

The gradient vector $\nabla f (\mathbf{p})$ points in the direction of the greatest rate of increase of the scalar function $f$ at the point $\mathbf{p}$.

The magnitude of the gradient vector $|\nabla f (\mathbf{p})∣$ represents the greatest rate of increase of $f$ at $\mathbf{p}$.

For a scalar function $f: \mathbb{R}^n \to \mathbb{R}$, the gradient at a specific point $\mathbf{x} = (x_1, x_2, \ldots, x_n)$ is a vector given by:
$$\LARGE \nabla f(\mathbf{x}) = \left< \frac{\partial f}{\partial x_1}(\mathbf{x}), \frac{\partial f}{\partial x_2}(\mathbf{x}), \ldots, \frac{\partial f}{\partial x_n}(\mathbf{x}) \right>$$

This vector points in the direction of the steepest increase of the function $f$ at the point $\mathbf{x}$.
	And this vector is perpendicular to the tangent vector of that point. 
##### Example
Consider the scalar function $f(x, y) = x^2 + y^2$.
**Gradient at a Specific Point**:
	At the point $(1, 2)$, the gradient is:
$$\LARGE \nabla f(1, 2) = \left< \frac{\partial f}{\partial x}(1, 2), \frac{\partial f}{\partial y}(\mathbf{1, 2})\right> = \left< 2 \cdot 1, 2 \cdot 2\right> = \left<2, 4\right>$$
This expression represents a vector field. 
	For each point $(x, y)$ in the domain, there is a corresponding gradient vector $(2x, 2y)$.
### Gradients and Scalar Functions 
*Again, the Gradient itself only exists relative to a Scalar Function (or Scalar Field).*
	*Therefore, the Gradient as a word, is "short for", Gradient of a Scalar Function (or Scalar Field).*
	
The gradient is specifically defined for scalar functions.
	It is a vector-valued function that represents the rate and direction of the fastest increase of the scalar function.

Remember, a Scalar Function simply means a [[Mapping#Output Types of Functions|mapping from a spatial domain to a scalar codomain.]], as a way to preserve a domain and extend a codomain.t
#### How Gradients are Connected to Scalar Functions
###### The Scalar Function, $f: R^n \to R$
Scalar Function, $f$ maps points in its domain (spatial or non spatial domain) to single Scalar Values.
###### The Gradient of *That* Scalar Function, $\nabla f: R^n \to R^n$
The Gradient of that Scalar Function, $\nabla f$, takes those ***same points*** (i.e. those same points that the Scalar Function took as input to be mapped to single Scalar Values) and ***itself* maps those points to vectors**.
	The [[Components of Motion|components]] of those produced Vectors are the [[Partial Derivatives|Partial Derivatives]] of the Scalar Function $f$ as each input variable changes (i.e. in respect to each input variable).
		Therefore, the Gradient of the Scalar Function is a set of Vectors each composed of the Partial Derivatives (as Vector components)
##### Hierarchical Connection 
###### Gradient of a Scalar Field
The gradient of a scalar field is a vector field.
	Given a scalar field $f(x, y, z)$, the gradient $\nabla f$ is a vector field that points in the direction of the steepest ascent of the scalar field and whose magnitude represents the rate of increase.
###### Divergence of a Vector Field
The divergence of a vector field is a scalar field. 
	Given a vector field $\mathbf{F} = (F_x, F_y, F_z)$, the divergence $\nabla \cdot \mathbf{F}$ is a scalar field representing the net rate of flow of the vector field out of an infinitesimal volume.
$$\LARGE \nabla \cdot \mathbf{F} = \frac{\partial F_x}{\partial x} + \frac{\partial F_y}{\partial y} + \frac{\partial F_z}{\partial z}$$
###### Curl of a Vector Field
The curl of a vector field is another vector field. 
	Given a vector field $\mathbf{F} = (F_x, F_y, F_z)$, the curl $\nabla \times \mathbf{F}$ measures the rotation of the field around a point.
$$\LARGE \nabla \times \mathbf{F} = \left( \frac{\partial F_z}{\partial y} - \frac{\partial F_y}{\partial z}, \frac{\partial F_x}{\partial z} - \frac{\partial F_z}{\partial x}, \frac{\partial F_y}{\partial x} - \frac{\partial F_x}{\partial y} \right)$$
#### Why Gradients Apply to Scalar Functions
###### Directional Information
The gradient vector provides both the direction and magnitude of the steepest ascent of the scalar function. 
	This is useful for understanding how the function behaves locally around a point.
###### Optimization
In optimization, gradients are used to find local maxima and minima of scalar functions. 
	The gradient points in the direction of the steepest increase, and its negative points in the direction of the steepest decrease.
###### Physical Interpretations
In physics, gradients often describe how physical quantities (like temperature, pressure, etc.) change in space. 
	These quantities are scalar fields, and their gradients provide insight into their spatial variation.
#### Gradients and Non-Scalar Functions
For functions that are not scalar-valued, such as vector-valued functions $\mathbf{F}: \mathbb{R}^n \to \mathbb{R}^m$, the concept of the gradient does not directly apply. 
	Instead, other concepts are used.

Consider a function $f$ that takes multiple variables as input and produces a single value as output. 
	This function can be written as $f(x_1, x_2, \ldots, x_n)$, where $x_1, x_2, \ldots$, are the variables.
- - -

- - -
