# Partial Derivatives
Derivatives in 2D and 3D (and higher dimensions) are generally referred to as **partial derivatives** when dealing with functions of multiple variables. 

For a function of multiple variables, such as $f(x,y)$ or $f(x,y,z)$:
	Partial derivatives represent the rate of change of the function with respect to one of its variables, while holding the other variables constant.

$\LARGE \partial = \text{partial}$
## For a (1D) Function $f(x)$
The Partial Derivative in 1D is the **same** as the conventional Derivative in 1D.
![[Pasted image 20240623214613.png|300]] ![[Pasted image 20240623214918.png|300]]
$$\LARGE \partial_x f(x)== {\partial \over \partial x} == {d\over dx} f(x) == f'(x)$$
$$\LARGE {\partial \over \partial x} f(x) = \lim_{h \rightarrow 0} {f(x+h) - f(x) \over h}$$
## For a ([[Components of Motion#2D Components of the Velocity Vector|2D]]) Function $f(x, y)$
Its a bit different, because we have a function that depends on multiple variables, $x,y$.
	$f'(x.y)$ does not make sense or clarify meaning. 

Therefore, we need Partial Derivatives, where we only derive in respect to a single given variable. 
$$\LARGE \frac{\partial f}{\partial x} \quad \text{and} \quad \frac{\partial f}{\partial y}$$
### Partial Derivative for Single Point
The following, is the Partial Derivative of $f(x,y)$ with respect to $x$. 
	Which means, we only derive with respect to the variable, $x$. 
		Therefore, the interval value, $h$ is only added to $x$ and not $y$.
			But the rest is the same as the conventional Limit. 
				I.e. The limit of the rate of change of the output of the function, $f(x,y)$ as the $x$ changes.  
![[Pasted image 20240623221622.png|300]]
*Remember: The [[Limits#Limit at a Specific Point|Limit]] in the following form represents the rate of change at a specific point, $a$.*
$$\LARGE \partial_x f(x,y) == {\partial \over \partial x}f(x,y) = \lim_{h \rightarrow 0} {f(x+h,y) - f(x,y) \over h}$$
![[Pasted image 20240623222925.png|300]]
*Remember: The [[Limits#Limit at a Specific Point|Limit]] in the following form represents the rate of change at a specific point, $a$.*
$$\LARGE \partial_x f(x,y) == {\partial \over \partial y}f(x,y) = \lim_{h \rightarrow 0} {f(x,y+h) - f(x,y) \over h}$$
### General Function for the Partial Derivative at Any Point
![[Pasted image 20240624140108.png|500]]
To obtain a general function of the Derivative such that we are not restricted to a single point.

Consider the exponential function given in the image:
	*The exponential function is denoted by $\exp(z)$ and is equivalent to $e^z$, where $e$ is the base of the natural logarithm.*
$$\LARGE f(x, y) = \exp(-x^2 -y^4)$$
This is equivalent to: 
$$\LARGE f(x, y) = e^{-x^2 - y^4}$$
##### Partial Derivative with Respect to $x$
To find the partial derivative of $f$ with respect to $x$, denoted as $\LARGE \frac{\partial f}{\partial x}$​

###### 1. Identify the inner function: 
The inner function in this case is the exponent, $\LARGE z(x,y) -x^2 - y^4$
	The inner function is what is inside the exponential function, $z(x,y)$.
###### 2. Differentiate the outer function: 
The outer function is $\exp(z)$, and its derivative is 
$$\exp(z) \cdot \frac{dz}{dx}$$
###### 3. Apply the [[Derivatives#Chain Rule|chain rule]]
To find the partial derivatives, we differentiate the outer function with respect to the inner function and then multiply by the derivative of the inner function with respect to each variable.

- **Partial derivative of the inner function with respect to $x$**: 
	- To find the partial derivative of $z$ with respect to $x$, we treat $y$ as a [[Derivatives#Derivative of a Constant is Zero|constant]] (which is 0), and use the [[Derivatives#Power Rule|Power Rule]]
$$\LARGE \frac{\partial u}{\partial x} = \frac{\partial}{\partial x} (-x^2 - y^4) = -2x$$

$$\LARGE \frac{\partial f}{\partial x} = \frac{\partial}{\partial x} \left( \exp(-x^2 - y^4) \right) = \exp(-x^2 - y^4) \cdot \frac{\partial}{\partial x} (-x^2 - y^4)$$
###### 4. Differentiate the inner function -x^2 - y^4− with respect to $x$
$$\LARGE \frac{\partial}{\partial x} (-x^2 - y^4) = -2x$$
####### 5. Combine the results
$$\LARGE \frac{\partial f}{\partial x} = \exp(-x^2 - y^4) \cdot (-2x) = -2x \exp(-x^2 - y^4)$$

## For a ([[Components of Motion#3D Components of the Velocity Vector|3D]]) function $f(x, y, z)$
$$\LARGE \frac{\partial f}{\partial x}, \quad \frac{\partial f}{\partial y}, \quad \text{and} \quad \frac{\partial f}{\partial z}$$
The partial derivative $\frac{\partial f}{\partial x}$​ represents the rate of change of the function $f$ with respect to the variable $x$, while keeping all other variables constant.
	It does not mean the output value of ${f(x) \over x}$​, but rather how the function $f(x, y, \ldots)$ changes as $x$ changes, with all other variables held fixed.

Given a function $f(x,y)$, the partial derivative of $f$ with respect to $x$, denoted $\frac{\partial f}{\partial x}$​, is defined as:

$$\LARGE \frac{\partial f}{\partial x} = \lim_{\Delta x \to 0} \frac{f(x + \Delta x, y) - f(x, y)}{\Delta x}$$

This definition shows that the partial derivative measures how the function $f(x,y)$ changes as $x$ changes by a small amount $\Delta x$, while $y$ remains constant.
### Partial Derivative Example
Consider the function $f(x, y) = x^2 + 3xy + y^2$.
	To find the partial derivative with respect to $x$, we differentiate $f$ with respect to $x$ while treating $y$ as a constant:

$$\LARGE \frac{\partial f}{\partial x} = \frac{\partial}{\partial x} \left( x^2 + 3xy + y^2 \right)$$
#### Calculation Steps
1. **Differentiate $2x^2$ with respect to $x$**:
$$\LARGE \frac{\partial}{\partial x} \left( x^2 \right) = 2x$$
2. **Differentiate $3xy$ with respect to $x$**:

$$\LARGE \frac{\partial}{\partial x} \left( 3xy \right) = 3y$$

- Here, $y$ is treated as a constant.

3. **Differentiate $y^2$ with respect to $x$**:

$$\LARGE \frac{\partial}{\partial x} \left( y^2 \right) = 0$$
- Since $y^2$ is independent of $x$, its derivative with respect to $x$ is zero.
###### Combine the Results
Adding these partial derivatives together gives:
$$\LARGE \frac{\partial f}{\partial x} = 2x + 3y$$
### Gradient
The gradient of a scalar function $f(x, y, z)$ in 3D is a vector that points in the direction of the greatest rate of increase of the function. 
	It is composed of the partial derivatives with respect to each variable:

$$\LARGE \nabla f = \left( \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z} \right)$$
##### Scalar Functions
A scalar function $f$ is a function that takes one or more variables and returns a single scalar value. Mathematically, it can be written as, 
	*This notation represents scalar functions that take multiple inputs and return a single output, which is a scalar value.*
###### For 2 Variables
$$f(x,y)$$
###### For 3 Variables
$$f(x,y,z)$$
###### For $n$ Variables
$$f(x_1, x_2, \ldots, x_n)$$
