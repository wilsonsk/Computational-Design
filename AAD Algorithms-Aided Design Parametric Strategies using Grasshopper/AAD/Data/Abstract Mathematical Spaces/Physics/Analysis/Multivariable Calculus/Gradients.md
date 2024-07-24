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
An **increase** or **decrease** in the **magnitude** of a **property**, relative to some variable (time, position, etc.).

*Note: a Derivative (and Partial Derivative) **is** a vector.*
	*That vector being the [[Derivatives#4. Is the Unit Tangent Vector|Unit Tangent Vector]] to a given point.*
		Therefore the Vector of the Partial Derivatives is a Unit Tangent Vector describing the direction of the function in a single dimension.
			But the **Gradient vector** describes the direction and rate of the steepest increase in a multi-dimensional space.

The gradient of a scalar field is a vector field that points in the direction of the greatest rate of increase of the scalar field and whose magnitude is the rate of increase in that direction.
	==**The gradient $\nabla f$ is a vector field that points radially outward from the origin and whose magnitude increases with distance from the origin.==**
		The phrase "the gradient of a scalar field" specifically refers to the vector field that is derived from a scalar field by taking its partial derivatives. 
			This gradient vector field indicates the direction and rate of the greatest increase of the scalar field at each point in space.
### What "Greatest Increase of $f$" Means
The directional derivative is maximized when $\mathbf{u}$ is in the same direction as $\nabla f$. 
	Thus, the gradient vector $\nabla f$ points in the direction where $f$ increases most rapidly.
		The magnitude of the gradient vector $|\nabla f|$ represents the rate of change of $f$ in the direction of the gradient.
			A larger magnitude means a steeper ascent.
### Therefore, the Gradient Vector $\nabla f$ at a point on a level curve (or level surface) is **Perpendicular** to the [[Partial Derivatives#Tangent Plane and Tangent Vector|unit tangent vector]] of that point
==This perpendicularity of the gradient vector to the tangent vector of the level curve (or surface) at a point is what causes the gradient vector to point in the direction of the greatest increase in the scalar function $f$.==

Remember the Derivative is the Differential Ratio
$$\LARGE \LARGE f'(x) = \frac{df}{dx}$$
And rearranged it is:
$$\LARGE \LARGE df=f′(x) dx = \frac{df}{dx}dx$$
Remember that the Derivative as a Unit Tangent Vector is just a Vector Function that contains the Differentials as components.
$$\LARGE \mathbf{T}(\Delta x) = \begin{pmatrix} \Delta x \\ \Delta y \end{pmatrix} = \begin{pmatrix} \Delta x \\ f'(x) \Delta x \end{pmatrix}$$
$$\text{Where } \Delta y = f'(x)\Delta x $$
The Unit Tangent Vector for a Partial Derivative
$$\LARGE \mathbf{T}(\Delta x, \Delta y) = \begin{pmatrix} \Delta x \\ \Delta y \\ \Delta z \end{pmatrix} = \begin{pmatrix} \Delta x \\ \Delta y \\ \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y \end{pmatrix}$$
$$\text{Where } \Delta z = \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y   $$
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
