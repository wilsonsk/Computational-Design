# Partial Derivatives
![[Pasted image 20240630153708.png]]
Derivatives in 2D and 3D (and higher dimensions) are generally referred to as **partial derivatives** when dealing with functions of multiple variables. 

For a function of multiple variables, such as $f(x,y)$ or $f(x,y,z)$:
	Partial derivatives represent the rate of change of the function with respect to one of its variables, while holding the other variables constant.

The idea to keep in mind when calculating partial derivatives is to treat all independent variables, other than the variable with respect to which we are differentiating, as constants. 
	Then proceed to differentiate as with a function of a single variable. T

$\LARGE \partial = \text{partial}$
##### Key Concepts
1. A partial derivative is a derivative involving a function of more than one independent variable. 
	1. **partial derivative**: A derivative of a function of more than one independent variable in which all the variables but one are held constant.
	2. **Partial Differential Equation**: An equation that involves an unknown function of more than one independent variable and one or more of its partial derivatives.
2. To calculate a partial derivative with respect to a given variable, treat all the other variables as constants and use the usual differentiation rules. 
3. Higher-order partial derivatives can be calculated in the same way as higher-order derivatives.
	1. **Higher-Order Partial Derivatives**: Second-order or higher partial derivatives, regardless of whether they are mixed partial derivatives.
	2. **Mixed Partial Derivatives**: Second-order or higher partial derivatives, in which at least two of the differentiations are with respect to different variables.
## For a (1D) Function $f(x)$
The Partial Derivative in 1D is the **same** as the conventional Derivative in 1D.
	That is because there is only one variable to begin with.
![[Pasted image 20240623214613.png|300]] ![[Pasted image 20240623214918.png|300]]
$$\LARGE \partial_x f(x)== {\partial \over \partial x} == {d\over dx} f(x) == f'(x)$$
$$\LARGE {\partial \over \partial x} f(x) = \lim_{h \rightarrow 0} {f(x+h) - f(x) \over h}$$

- - -
## For a ([[Components of Motion#2D Components of the Velocity Vector|2D]]) Function $f(x, y)$
Its a bit different, because we have a function that depends on multiple variables, $x,y$.
	$f'(x.y)$ does not make sense or clarify meaning. 

Therefore, we need Partial Derivatives, where we only derive in respect to a single given variable. 
$$\LARGE \frac{\partial f}{\partial x} \quad \text{and} \quad \frac{\partial f}{\partial y}$$
###### Notation
$$\LARGE \frac{\partial f}{\partial x}$$
​This is the standard notation for the partial derivative of $f$ with respect to $x$.
$$\LARGE \partial_x f(x,y)$$
This notation emphasizes that the partial derivative is with respect to $x$ and can be seen as a more compact form.
$$\LARGE \frac{\partial}{\partial x} f(x,y)$$
This notation explicitly shows the operation of taking the partial derivative with respect to $x$.
### Partial Derivative Means the Differential of the Function in Respect to a Single Variable
The following, is the Partial Derivative of $f(x,y)$ with respect to $x$. 
	Which means, we only derive with respect to the variable, $x$ (i.e derive $f(x,y)$ as $x$ changes). 
		Therefore, the interval value, $h$ is only added to $x$ and not $y$.
			But the rest is the same as the conventional Limit. 
				I.e. The limit of the rate of change of the output of the function, $f(x,y)$ as the $x$ changes.  

- - -
### 2D Partial Derivative of $f$ with Respect to $x$
$$\LARGE \frac{\partial f}{\partial x} == \partial_x f(x,y) == {\partial \over \partial x}f(x,y) = \lim_{h \rightarrow 0} {f(x+h,y) - f(x,y) \over h}$$
*Remember: The [[Limits#Limit at a Specific Point|Limit]] in the following form represents the rate of change at a specific point, $a$.*
##### Function, $\LARGE f(x,y)$
![[Pasted image 20240623221622.png|300]]
##### Differential of $f(x,y)$, $\LARGE \frac{\partial}{\partial x}f(x,y)$
![[Pasted image 20240705151637.png|400]]
When we first approach this very, very steep slope here where this derivative has a large peak.
	Then when you approach the top, this slope gets less steep.
		Then at the plateau, the slope is zero.
			This is why you get here a very large flat region in between the convex and concave regions, where the derivative is basically zero.

- - -
### 2D Partial Derivative of $f$ with Respect to $y$
$$\LARGE \frac{\partial f}{\partial y} == \partial_x f(x,y) == {\partial \over \partial y}f(x,y) = \lim_{h \rightarrow 0} {f(x,y+h) - f(x,y) \over h}$$
*Remember: The [[Limits#Limit at a Specific Point|Limit]] in the following form represents the rate of change at a specific point, $a$.*
##### Function, $\LARGE f(x,y)$
![[Pasted image 20240623222925.png|300]]
##### Differential of $f(x,y)$, $\LARGE \frac{\partial}{\partial y}f(x,y)$
![[Pasted image 20240705151727.png|400]]
When we first approach this very, very steep slope here where this derivative has a large peak.
	Then when you approach the top, this slope gets less steep.
		Then at the plateau, the slope is zero.
			This is why you get here a very large flat region in between the convex and concave regions, where the derivative is basically zero.

- - -
## Interpreting Partial Derivatives
Recall that the graph of a function of two variables is a surface in R^3.

If we remove the limit from the definition of partial derivative with respect to $x$, $\LARGE \lim\limits_{h \to 0} \frac{f(x+h, y) - f(x,y)}{h}$, then the Difference Quotient remains.
$$\LARGE \frac{f(x+h, y) - f(x,y)}{h}$$
This resembles the difference quotient for the derivative of a function of one variable, except for the presence of the variable.
![[Pasted image 20240630154205.png]]
If $h$ is positive, and we graph $f(x,y)$ and $f(x+h,y)$ for an arbitrary point $(x,y)$ then the slope of the secant line passing through these two points is given by this Difference Quotient.
	This line is parallel to the $x$-axis.
		Therefore, the slope of the secant line represents an average rate of change of the function $f(x,y)$ as we travel parallel to the $x$-axis.
			 As $h$ approaches zero, the slope of the secant line approaches the slope of the tangent line.

If we choose to change $y$ instead of $x$ by the same incremental value $h$, then the secant line is parallel to the $y$-axis and so is the tangent line.
	Therefore, $\LARGE \frac{\partial f}{\partial x}$ represents the slope of the tangent line passing through the point $(x,y, f(x,y))$ parallel to the $x$-axis.
		And $\LARGE \frac{\partial f}{\partial y}$ represents the slope of the tangent line passing through the point $(x,y,f(x,y))$ parallel to the $y$-axis. 

If we wish **to find the slope of a tangent line passing through the same point** in any other direction, then we need what are called **directional derivatives**.

- - - 
### Calculating Partial Derivative by Using the Limit
Use the definition of the partial derivative as a limit to calculate $\frac{\partial f}{\partial x}$ and $\frac{\partial f}{\partial y}$ for the function
$$\LARGE f(x, y) = x^2 - 3xy + 2y^2 - 4x + 5y - 12$$
##### Solution
###### 1. Calculate $f(x + h, y)$
$$\LARGE f(x + h, y) = (x + h)^2 - 3(x + h)y + 2y^2 - 4(x + h) + 5y - 12$$
$$\LARGE = x^2 + 2xh + h^2 - 3xy - 3hy + 2y^2 - 4x - 4h + 5y - 12$$
###### 2. Substitute This Into the Initial Equation and Simplify
$$\LARGE \frac{\partial f}{\partial x} = \lim_{h \to 0} \frac{f(x + h, y) - f(x, y)}{h}$$
$$ = \lim_{h \to 0} \frac{(x^2 + 2xh + h^2 - 3xy - 3hy + 2y^2 - 4x - 4h + 5y - 12) - (x^2 - 3xy + 2y^2 - 4x + 5y - 12)}{h}$$
$$ = \lim_{h \to 0} \frac{x^2 + 2xh + h^2 - 3xy - 3hy + 2y^2 - 4x - 4h + 5y - 12 - x^2 + 3xy - 2y^2 + 4x - 5y + 12}{h}$$
$$\LARGE = \lim_{h \to 0} \frac{2xh + h^2 - 3hy - 4h}{h}$$
$$\LARGE = \lim_{h \to 0} \frac{h(2x + h - 3y - 4)}{h}$$
$$\LARGE = \lim_{h \to 0} (2x + h - 3y - 4)$$
$$\LARGE \frac{\partial f}{\partial x} = 2x - 3y - 4$$
###### 3. Calculate $\frac{\partial f}{\partial y}$, first calculate $f(x, y + h)$
$$\LARGE f(x, y + h) = x^2 - 3x(y + h) + 2(y + h)^2 - 4x + 5(y + h) - 12$$
$$\LARGE = x^2 - 3xy - 3xh + 2y^2 + 4yh + 2h^2 - 4x + 5y + 5h - 12$$
###### 4. Substitute This Into the Equation and Simplify
$$\LARGE \frac{\partial f}{\partial y} = \lim_{h \to 0} \frac{f(x, y + h) - f(x, y)}{h}$$
$$= \lim_{h \to 0} \frac{(x^2 - 3xy - 3xh + 2y^2 + 4yh + 2h^2 - 4x + 5y + 5h - 12) - (x^2 - 3xy + 2y^2 - 4x + 5y - 12)}{h}$$
$$ = \lim_{h \to 0} \frac{x^2 - 3xy - 3xh + 2y^2 + 4yh + 2h^2 - 4x + 5y + 5h - 12 - x^2 + 3xy - 2y^2 + 4x - 5y + 12}{h}$$
$$\LARGE = \lim_{h \to 0} \frac{-3xh + 4yh + 2h^2 + 5h}{h}$$
$$\LARGE = \lim_{h \to 0} \frac{h(-3x + 4y + 2h + 5)}{h}$$
$$\LARGE \frac{\partial f}{\partial x} = \lim_{h \to 0} (-3x + 4y + 2h + 5)$$
$$\LARGE = -3x + 4y + 5$$

- - -
### Calculating Partial Derivative by Rules Of Differentiation
$$\LARGE \frac{\partial f}{\partial x} = \frac{\partial}{\partial x} [x^2 - 3xy + 2y^2 - 4x + 5y - 12]$$
$$\LARGE = \frac{\partial}{\partial x} [x^2] - \frac{\partial}{\partial x} [3xy] + \frac{\partial}{\partial x}[2y^2] - \frac{\partial}{\partial x}[4x] + \frac{\partial}{\partial x}[5y] - 12]$$
##### Solution
##### 1st Term, $\LARGE x^2$
[[Derivatives#Power Rule|Power Rule]] is applied.
$$\LARGE [x^2] = 2x $$
##### 2nd Term, $\LARGE -3xy$
Utilizes the [[Derivatives#Constant Scalar Rule, ($ LARGE af(x)$)|Constant Scalar Rule]] to discretize $-3xy$.
$$\LARGE -3y \text{ is treated as a constant scalar of x.}$$
Then applies the [[Derivatives#Derivative of a Linear Term, ($ LARGE ax$) aka Differentiating $x$ with Respect to Itself "*Directly*"|Derivative of a Linear Term Rule]] for $\LARGE -3y \cdot x = -3y$
$$\LARGE = -3y \cdot x = -3y \cdot 1(x^{1-1}) = -3y \cdot 1 = -3y$$
##### 3rd Term, $\LARGE 2y^2$
$\LARGE 2y^2$ contains no  x at all, so $\LARGE y$  is treated as a constant.
	And therefore, the [[Derivatives#Constant Scalar Rule, ($ LARGE af(x)$)|Constant Scalar Rule]] is applied.
$$\LARGE \text{The derivative of a constant is 0, } [2y^2] = 0 $$
##### 4th Term, $\LARGE-4x$
Utilize the [[Derivatives#Derivative of a Linear Term, ($ LARGE ax$)| Derivative of a Linear Term Rule]]
$$\LARGE [4x] = 4 \cdot (1)x^{1-1}= 4 \cdot 1= 4$$
##### 5th Term, $\LARGE 5y$
$\LARGE 5y$ contains no  x at all, so $\LARGE y$  is treated as a constant.
	And therefore, the [[Derivatives#Constant Scalar Rule, ($ LARGE af(x)$)|Constant Scalar Rule]] is applied.
$$\LARGE \text{The derivative of a constant is 0, }= [5y] = 0 $$
##### 6th Term, $\LARGE -12$
$\LARGE -12$ contains no  x at all, so $\LARGE y$  is treated as a constant.
	And therefore, the [[Derivatives#Constant Scalar Rule, ($ LARGE af(x)$)|Constant Scalar Rule]] is applied.
$$\LARGE \text{The derivative of a constant is 0, }= [-12] = 0 $$
- - -
## For a ([[Components of Motion#3D Components of the Velocity Vector|3D]]) function $f(x, y, z)$
$$\LARGE \frac{\partial f}{\partial x}, \quad \frac{\partial f}{\partial y}, \quad \text{and} \quad \frac{\partial f}{\partial z}$$
The partial derivative $\frac{\partial f}{\partial x}$​ represents the rate of change of the function $f$ with respect to the variable $x$, while keeping all other variables constant.
	It does not mean the output value of ${f(x) \over x}$​, but rather how the function $f(x, y, \ldots)$ changes as $x$ changes, with all other variables held fixed.

Given a function $f(x,y)$, the partial derivative of $f$ with respect to $x$, denoted $\frac{\partial f}{\partial x}$​, is defined as:

$$\LARGE \frac{\partial f}{\partial x} = \lim_{\Delta x \to 0} \frac{f(x + \Delta x, y) - f(x, y)}{\Delta x}$$

This definition shows that the partial derivative measures how the function $f(x,y)$ changes as $x$ changes by a small amount $\Delta x$, while $y$ remains constant.

- - -
## [[Directional Derivatives|Directional Derivatives]]
![[Pasted image 20240705152625.png|400]]

- - -


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
