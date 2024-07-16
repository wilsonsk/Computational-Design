---
up:
  - "[[Multivariable Calculus]]"
related: 
date created: 2024-07-28
---
# Gradients
#### *Note: Context-Dependent Terminology*
*If the Gradient is of a [[Abstract Mathematical Spaces#Scalar Functions|Scalar Function]], then it is itself a [[Abstract Mathematical Spaces#Vector Function|Vector Function]].*
	*But if the Gradient is of a [[Abstract Mathematical Spaces#Scalar Fields|Scalar Field]], then it is itself a [[Abstract Mathematical Spaces#Vector Fields|Vector Field]].*

*And that context is depending on the domain of the Scalar Function/Field and Vector Function/Field.*
	*I.e. Whether or not the domain is [[Abstract Mathematical Spaces#"Space" vs. "Spatial"|"spatial"]] or not.*

*The Gradient itself only exists relative to a Scalar Function (or Scalar Field).*
	*Therefore, the Gradient as a word, is "short for", Gradient of a Scalar Function (or Scalar Field).*
### Gradient Defined
*Note: a Derivative (and Partial Derivative) **is** a vector.*
	*That vector being the [[Derivatives#4. Is the Unit Tangent Vector|Unit Tangent Vector]] to a given point.*
		Therefore the Vector of the Partial Derivatives is a Unit Tangent Vector describing the direction of the function in a single dimension.
			But the **Gradient vector** describes the direction and rate of the steepest increase in a multi-dimensional space.

A Gradient (of a Scalar Function/Field) is ***itself*** a **Vector Function/Field** (depending on context).
	Therefore, the Gradient of a Scalar Function/Field, as a Vector Function/Field, maps points (also vectors which can be represented by those points) from a given domain to vectors in a given codomain.
		A **Gradient** through its mappings, at every point in the domain, produces a [[Vectors|vector]] that encapsulates how a [[Mapping#A Function as a Subset of Mappings ($1 1$, $m 1$)|function]] changes at a given point in its [[Mapping#Domain as a Subset of the Underlying Set|domain]]. 
			It indicates both the direction and the rate of the steepest ascent of the function.
				The concept of a gradient is fundamental in multivariable calculus and has applications in various fields such as physics, engineering, and optimization.

The gradient of a scalar function $f$, denoted as $\nabla f$, is a [[Abstract Mathematical Spaces#Vector Fields|vector field]] that points in the direction of the greatest rate of increase of the function. 
	The [[Components of Motion|components]] of those produced Vectors are the [[Partial Derivatives|Partial Derivatives]] of the Scalar Function $f$ as each input variable changes (i.e. in respect to each input variable).
		Therefore, the Gradient of the Scalar Function is a set of Vectors each composed of the Partial Derivatives (as Vector components)
$$\LARGE \nabla f = \left< \frac{\partial f}{\partial x_1}, \frac{\partial f}{\partial x_2}, \ldots, \frac{\partial f}{\partial x_n} \right>$$
	$\LARGE \nabla$ is the [[#Nabla Operator ($ nabla$)|Nabla Operator]].


- The magnitude of the gradient vector ∣∇f(p)∣|\nabla f (\mathbf{p})|∣∇f(p)∣ represents the greatest rate of increase of fff at p\mathbf{p}p
##### Gradient at a Point (i.e. a Single Vector)
The Gradient of a scalar function at a specific point in the domain is a vector whose components are the partial derivatives at that point. 
	This vector points in the direction of the greatest rate of increase of the function at that point, and its magnitude represents the rate of this increase.

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
##### Gradient Over the Domain (Vector Field)
When you compute the gradient at every point in the domain of the function $f$, you get a vector field.
	This means that at each point $\mathbf{x}$ in the domain, there is a corresponding gradient vector $\nabla f(\mathbf{x})$.
##### Example
Consider the scalar function $f(x, y) = x^2 + y^2$.
Over the entire domain, the gradient is:
$$\LARGE \nabla f(x, y) = \left< 2x, 2y \right>$$
This expression represents a vector field. 
	For each point $(x, y)$ in the domain, there is a corresponding gradient vector $(2x, 2y)$.
#### Gradients and Scalar Functions 
*Again, the Gradient itself only exists relative to a Scalar Function (or Scalar Field).*
	*Therefore, the Gradient as a word, is "short for", Gradient of a Scalar Function (or Scalar Field).*
	
The gradient is specifically defined for scalar functions.
	It is a vector-valued function that represents the rate and direction of the fastest increase of the scalar function.
##### How Gradients are Connected to Scalar Functions
###### The Scalar Function, $f: R^n \to R$
Scalar Function, $f$ maps points in its domain (spatial or non spatial domain) to single Scalar Values.
###### The Gradient of *That* Scalar Function, $\nabla f: R^n \to R^n$
The Gradient of that Scalar Function, $\nabla f$, takes those ***same points*** (i.e. those same points that the Scalar Function took as input to be mapped to single Scalar Values) and ***itself* maps those points to vectors**.
	The [[Components of Motion|components]] of those produced Vectors are the [[Partial Derivatives|Partial Derivatives]] of the Scalar Function $f$ as each input variable changes (i.e. in respect to each input variable).
		Therefore, the Gradient of the Scalar Function is a set of Vectors each composed of the Partial Derivatives (as Vector components)
##### Why Gradients Apply to Scalar Functions
###### Directional Information
The gradient vector provides both the direction and magnitude of the steepest ascent of the scalar function. 
	This is useful for understanding how the function behaves locally around a point.
###### Optimization
In optimization, gradients are used to find local maxima and minima of scalar functions. 
	The gradient points in the direction of the steepest increase, and its negative points in the direction of the steepest decrease.
###### Physical Interpretations
In physics, gradients often describe how physical quantities (like temperature, pressure, etc.) change in space. 
	These quantities are scalar fields, and their gradients provide insight into their spatial variation.
##### Gradients and Non-Scalar Functions
For functions that are not scalar-valued, such as vector-valued functions $\mathbf{F}: \mathbb{R}^n \to \mathbb{R}^m$, the concept of the gradient does not directly apply. 
	Instead, other concepts are used.

Consider a function $f$ that takes multiple variables as input and produces a single value as output. 
	This function can be written as $f(x_1, x_2, \ldots, x_n)$, where $x_1, x_2, \ldots$, are the variables.

- - -
## Nabla Operator ($\nabla$)
The Nabla operator is a vector differential operator that, when applied to a scalar or vector field, produces different types of derivatives. 
	Its components are partial derivatives with respect to the spatial coordinates. 
		In three dimensions, the Nabla operator is defined as:
$$\LARGE \nabla = (\frac{\partial}{\partial x}, \frac{\partial}{\partial y}, \frac{\partial}{\partial z})$$
### Applying the Nabla Operator to a Scalar Function: Gradient
When the Nabla operator $\nabla$ is applied to a scalar function $f$, it produces the gradient of $f$.
	The gradient is a vector that contains all the first-order partial derivatives of $f$. 
		If $f$ is a function of $n$ variables, the gradient $\nabla f$ is given by:
$$\LARGE \nabla f=(\frac{\partial f}{d x_{1}},\frac{\partial f}{d x_{2}}, \ldots \frac{\partial f}{d x_{n}}​)$$
This gradient vector points in the direction of the steepest increase of the function and its magnitude represents the rate of this increase.
- - -
