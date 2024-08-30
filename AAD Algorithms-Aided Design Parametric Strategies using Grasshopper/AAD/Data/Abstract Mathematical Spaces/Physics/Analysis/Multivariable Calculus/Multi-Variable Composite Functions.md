# Derivatives of Multi-Variable Composite Functions
*See [[Mapping#A Composite Function as a Subset of Functions|Composite Functions]] for more information about Composite Functions.*
	*See [[Derivatives#Multi-Variable Composite Functions Chain Rule of Single Variable Functions]|Chain Rule For Single Variable Functions]].*

*Remember: The [[Derivatives#Notation|Notation of First Order Derivatives]] (Single Variable*) = $\LARGE \frac{d}{dt}$
	$\LARGE \frac{d}{dt}$ of a function $\LARGE f(t) = t^2+1$ is equivalent to $\LARGE \frac{d}{dt}f(t) == \frac{df}{dt} == \frac{d}{dt}t^2+1$
## First Order Partial Derivatives
First-order partial derivatives measure the rate of change of a function with respect to one of its input variables, while holding the other variables constant.

For a scalar-valued function $\LARGE f(x_1, x_2, \dots, x_n)$, the first-order partial derivative with respect to $\LARGE x_i$​ is denoted by:

$$\LARGE \frac{\partial f}{\partial x_i} = \lim_{\Delta x_i \to 0} \frac{f(x_1, x_2, \dots, x_i + \Delta x_i, \dots, x_n) - f(x_1, x_2, \dots, x_n)}{\Delta x_i}$$

In the context of **composite functions**, these first-order partial derivatives arise naturally when you apply the **chain rule**. 
	When a function $f$ depends on intermediate variables (e.g., $u(x, y)$ and $v(x)$), you use the chain rule to express how $f$ changes with respect to its original variables (e.g., $x$).
###### Example
Consider a function $\LARGE f(u(x, y), v(x))$. 
	The first-order partial derivative of $f$ with respect to $x$ is:
$$\LARGE \frac{\partial f}{\partial x} = \frac{\partial f}{\partial u} \cdot \frac{\partial u}{\partial x} + \frac{\partial f}{\partial v} \cdot \frac{\partial v}{\partial x}$$

This expression shows that the **first-order derivatives** of the composite function $f$ depend on the first-order derivatives of $u$ and $v$ with respect to $x$, as well as the derivatives of $f$ with respect to its intermediate variables $u$ and $v$.
##### First Order Partial Derivatives Relationship to Composite Functions
These arise when you differentiate a composite function with respect to one of the original variables. 
	The chain rule tells you how the derivative of the composite function is distributed across the intermediate functions (e.g., $u(x,y)$ and $v(x)$.
### Notation for First-Order Partial Derivatives
##### For a function $z = f(x, y)$, where $x$ and $y$ are variables:
1. **General notation**: 
	This notation represents the **differentiation operator**.
		 It indicates that you are going to take the derivative with respect to $x$, but it does not specify the function you are differentiating.
$$\LARGE \frac{\partial}{\partial x}$$ 2. **Applied to the function $z = f(x, y)$**: 
$$\LARGE \frac{\partial z}{\partial x}$$ 3. **Equivalent notations**: 
$$\LARGE \frac{\partial}{\partial x}f(x, y) \equiv \frac{\partial f}{\partial x} \equiv \frac{\partial}{\partial x} \cdot f \equiv \frac{\partial}{\partial x}z \equiv \frac{\partial z}{\partial x}$$ 4. **Example with a specific function**: If $f(x, y) = x^2 + y$, then: 
$$\LARGE \frac{\partial}{\partial x}f(x, y) \equiv \frac{\partial f}{\partial x} \equiv \frac{\partial}{\partial x}(x^2 + y) = 2x$$
5 . **Applied to a function ($\LARGE z = f(x(s, t), y(s, t))$):**
$$\LARGE \frac{\partial z}{\partial s} = \frac{\partial f}{\partial s}$$
6 . **Chain rule application to ($\LARGE x(s, t)$):**
$$\LARGE \frac{\partial}{\partial s} f(x(s, t)) = \frac{\partial f}{\partial x} \cdot \frac{\partial x}{\partial s}$$
7 . **For a specific function ($x(s, t) = s + 2t$):**
$$\LARGE \frac{\partial}{\partial s} (s + 2t)$$
### Second Order Partial Derivatives
Are the derivatives of the first order of the derivative of the first order.
	Second-order partial derivatives measure the rate of change of the first-order partial derivatives. They provide information about the curvature of the function and are denoted as:
$$\LARGE \frac{\partial^2 f}{\partial x_i^2} = \frac{\partial}{\partial x_i} \left( \frac{\partial f}{\partial x_i} \right)$$
$$\LARGE \text{Simplified: } \quad \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x} == \frac{\partial}{\partial x} (\frac{\partial z}{\partial x}) = \frac{\partial^2 z}{\partial x} $$
	Where $\LARGE \frac{\partial}{\partial x} (\frac{\partial z}{\partial x})$ means, the "partial derivative of the partial derivative."

Second-order partial derivatives can also be mixed derivatives, where you take the derivative with respect to different variables, such as:
$$\LARGE \frac{\partial^2 f}{\partial x_i \partial x_j}$$
In the context of **composite functions**, second-order derivatives arise when you take the derivative of the first-order derivative. 
	The chain rule for second-order derivatives becomes more complex, involving not just the second-order partial derivatives of the intermediate variables, but also the product of first-order derivatives.
### Notation for Second-Order Partial Derivatives
##### For the same function $z = f(x, y)$:
1. **General notation**:    
	This notation represents the **differentiation operator**.
		 It indicates that you are going to take the derivative with respect to $x$, but it does not specify the function you are differentiating.
$$\LARGE \frac{\partial^2}{\partial x^2}$$  2. **Applied to the function $z = f(x, y)$**:
$$\LARGE \frac{\partial^2 z}{\partial x^2}$$  3. **Equivalent notations**:    
$$\LARGE \frac{\partial^2}{\partial x^2}f(x, y) \equiv \frac{\partial^2 f}{\partial x^2} \equiv \frac{\partial^2}{\partial x^2}z \equiv \frac{\partial^2 z}{\partial x^2}$$
4 . **Applied to a function ($\LARGE z = f(x(s, t), y(s, t))$):**
$$\LARGE \frac{\partial^2 z}{\partial s^2} = \frac{\partial}{\partial s} \left( \frac{\partial z}{\partial s} \right)$$
$$\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial s} \right) \text{means "take the partial derivative with respect to $s$ of the first derivative"} \frac{\partial z}{\partial x}$$
5 . **Chain rule application to the second derivative:**
$$\LARGE \frac{\partial^2}{\partial s^2} f(x(s, t)) = \frac{\partial}{\partial s} \left( \frac{\partial f}{\partial x} \cdot \frac{\partial x}{\partial s} \right)$$
##### **$\LARGE \frac{\partial^2 t}{\partial t^2}$​** is saying: "Take the derivative of $z$ with respect to $t$, and then do it again."
First, take the partial derivative of $z$ with respect to $t$, which gives $\LARGE \frac{\partial z}{\partial t}$.
	Then, take the partial derivative of $\LARGE \frac{\partial z}{\partial t}$​ with respect to $t$ again, which gives $\LARGE \frac{\partial^2 z}{\partial t^2}$.
		So, $\LARGE \frac{\partial^2 z}{\partial t^2}$ represents the **second-order partial derivative** of $z$ with respect to $t$. 
			It describes how the rate of change of $z$ with respect to $t$ changes as $t$ varies.
				 In other words, it measures the "curvature" or "acceleration" of $z$ with respect to $t$.
##### **$\LARGE \frac{\partial z^2}{\partial t^2}$​** is saying: "First square $z$, then take the derivative of the resulting expression."
This expression​ does **not** represent the second-order partial derivative of $z$ with respect to $y$.
	Instead, it suggests something different:
		The notation $\LARGE \frac{\partial z^2}{\partial t^2}$​ would imply that you are first **squaring** $z$, i.e., considering the function $z^2$, and then taking the partial derivative of this new function $z^2$ with respect to $y$.
##### Second Order Partial Derivatives Relationship to Composite Functions
These come into play when you take the derivative of the first-order derivatives.
	For composite functions, the second-order derivatives involve applying both the product rule and the chain rule, leading to more complex expressions that account for the curvature of the function in the transformed space.
## The First Order Derivatives of [[Mapping#A Composite Function as a Subset of Functions|Composite Functions]]
The derivative of a composite function in the context of multivariable calculus is dependent on the **first-order non-partial derivatives** of the inner functions.
$$\LARGE f \circ g \circ h: \mathbb{R} \xrightarrow{h}\mathbb{R} \xrightarrow{g}  \mathbb{R} \xrightarrow{f} \mathbb{R}$$
$$\LARGE \frac{d}{dx}f(g(h(x))) = \frac{d}{dg(h(x))}f(g(h(x))) \cdot \frac{d}{dh(x)}g(h(x)) \cdot \frac{d}{dx}h(x)$$
$$\LARGE ==  f'(g(h(x)) \cdot g'(h(x)) \cdot h'(x)$$

A composite function is formed when one function is applied after another. 
	Mathematically, if you have two functions $\LARGE f: \mathbb{R}^m \to \mathbb{R}^k$ and $\LARGE \Phi: \mathbb{R}^n \to \mathbb{R}^m$, their composition $\LARGE f \circ \Phi$ is defined as:
$$\LARGE (f \circ \Phi)(\mathbf{s}) = f(\Phi(\mathbf{s}))$$
		where you first apply the transformation $\Phi$ to the input $\mathbf{s}$, and then apply the function $f$ to the result.
## Transformations as Composite Functions
A **transformation** is a function that explicitly describes a mapping from one space to another. It is typically represented as $\LARGE \mathbb{R}^m \to \mathbb{R}^n$, where f maps inputs from an $m$-dimensional space ($\mathbb{R}^m$) to an $n$-dimensional space ($\LARGE \mathbb{R}^n$).

The term "transformation" is generally used when the focus is on the mapping between spaces and how that mapping changes the structure, coordinates, or geometry.
	"Composite function," on the other hand, emphasizes the process of combining functions. 
		The term "transformation" is more specific and often associated with the idea of changing or mapping spaces, while "composite function" is broader and refers to the combination of any functions, whether or not they explicitly map between spaces.

**Overlap**: $\large \textcolor{yellow}{\text{When a composite function is used to map between spaces, it is also a transformation.}}$
#### Direct Transformations
This transformation is a simple function that directly maps between spaces, and **no composition with another transformation is involved.**

If you have a transformation like 
$$\LARGE \Phi(s,t) = \begin{pmatrix} x(s,t) \\ y(s,t) \end{pmatrix}$$
This is a transformation (i.e. composite function) from $\mathbb{R}^2$ (with variables $s$ and $t$) to $\mathbb{R}^2$ (with variables $x$ and $y$). 
	This transformation by itself can be thought of as a function that directly maps between spaces.

$$\LARGE \Phi(s,t) = \begin{pmatrix} x(s,t) \\ y(s,t)  \\ z(s,t) \end{pmatrix}$$
This is a transformation (i.e. composite function) from $\mathbb{R}^2$ (with variables $s$ and $t$) to $\mathbb{R}^3$ (with variables $x$ and $y$ and $z$). 
	This transformation by itself can be thought of as a function that directly maps between spaces.
#### Composite Transformations
Refers to transformations (which are specific types of functions) that are composed of other transformations.
	I.e. Combining transformations.

A **composite transformation** occurs when two or more transformations are applied sequentially, where the output of one transformation becomes the input of the next. 
	Mathematically, if you have two transformations 
$$\LARGE \Phi: \mathbb{R}^n \to \mathbb{R}^m \text{ and } \Psi: \mathbb{R}^m \to \mathbb{R}^k$$
	Then their composition $\LARGE \Psi \circ \Phi$ is defined as: 
$$\LARGE (\Psi \circ \Phi)(\mathbf{s}) = \Psi(\Phi(\mathbf{s}))$$
This means you first apply the transformation $\LARGE \Phi$ to the input $\LARGE \mathbf{s}$ and $\LARGE \mathbf{s}$ , and then apply the transformation $\LARGE \Psi$ to the result of $\LARGE \Phi(\mathbf{s,t})$.

When you're dealing with a transformation like $\LARGE \Phi(s, t) = (x(s,t), y(s,t))$ and then apply a function $f(x,y)$ to the result, you're effectively dealing with a composite function, where the function $f$ is composed with the transformation $\Phi$.
	The partial derivatives you calculate in this context (whether you call them derivatives of composite functions or composite transformations) are derived using the chain rule, reflecting the dependence on the intermediate variables.

If you combine transformations, or if your function is expressed in terms of other functions (like coordinate transformations), this can often be modeled as a composition of functions. 
	For instance, if you have a physical quantity $f$ that depends on coordinates $(x, y)$, but you express $(x, y)$ as functions of $(s, t)$, the overall function $f$ is a composition of the transformation $\Phi(s,t)$ and the original function $f(x,y)$:
$$\LARGE \mathbb{R}^2 \xrightarrow{\Phi} \mathbb{R}^2 \xrightarrow{f} \mathbb{R}$$
$$\LARGE f(x, y) = f(x(s,t), y(s,t))$$
In this sense, the transformation is part of a composite function where the final outcome depends on the intermediate step of transforming the variables.
## [[Derivatives#Chain Rule Chain Rule of Single Variable Functions|Chain Rule for Single Variable Functions]]
The chain rule is a formula for computing the derivative of the composition (i.e. composite functions) of two or more functions.
	I.e. is a rule for computations of the [[Derivatives|derivatives]] of [[Mapping#A Composite Function as a Subset of Functions|composite functions]].
		Where the $\textcolor{yellow}{\text{derivative of a composite function}}$ is the product of the derivatives of each of the subsequent component functions. 
$$ \LARGE \textcolor{magenta}{x} \to \textcolor{orange}{x^2} \to \textcolor{green}{\sin x^2} \to \textcolor{red}{\ln(\sin x^2)} $$
$$\LARGE \textcolor{green}{\frac{d}{dx}\sin x^2 = \cos x^2}$$
$$\LARGE \textcolor{orange}{\frac{d}{dx} x^2 = 2x}$$
$$\LARGE \textcolor{magenta}{\frac{d}{dx} x = 1}$$
$$ \LARGE = \textcolor{yellow}{\frac{d}{dx}(\ln (\sin x^2))} = \textcolor{red}{\frac{1}{\sin x^2}} \cdot \textcolor{green}{\cos x^2} \cdot \textcolor{orange}{2x} \cdot \textcolor{magenta}{1}$$
In this case there are three functions which are composed with each other.
	And the chain rule gives a product of three derivatives, the most outer one, the most inner one, and all the functions in between. 
## Chain Rule for Multi-Variable Composite Functions
The chain rule in multivariable calculus tells us that when we take the derivative of a function that depends on multiple variables, we must account for how each of those variables changes.
	Specifically, when you differentiate $\LARGE \frac{\partial z}{\partial x}$​ with respect to $s$, you need to account for how $\LARGE \frac{\partial z}{\partial x}$​ changes with respect to $x$ (which itself depends on $s$) and with respect to $y$ (which also depends on $s$).

The chain rule is used to compute the derivative of the composite function with respect to the outer variables (e.g., $x$, $y$).
	The chain rule tells us that to compute the derivative of the composite function with respect to an outer variable (e.g., $x$), you need to account for all the paths through which $x$ influences the final function $f$.
		This involves:
			The **first-order partial derivatives** of the outer function $f$ with respect to the intermediate variables (e.g., $u$ and $v$).
				And the **first-order partial derivatives** of the inner functions $u$ and $v$ with respect to the outer variables (e.g., $x$).
### First-Order Partial Derivative Chain Rule
Suppose $\LARGE f(u(x,y),v(x,y))$ is a composite function. 
	The derivative of $f$ with respect to $x$ is given by: 
$$\LARGE \frac{\partial f}{\partial x} = \frac{\partial f}{\partial u} \cdot \frac{\partial u}{\partial x} + \frac{\partial f}{\partial v} \cdot \frac{\partial v}{\partial x}$$

Here, $\LARGE \frac{\partial f}{\partial u}$​ and $\LARGE \frac{\partial f}{\partial v}$​ are the **first-order partial derivatives** of the outer function $f$.
$\LARGE \frac{\partial u}{\partial x}$​ and $\LARGE \frac{\partial v}{\partial x}$​ are the **first-order partial derivatives** of the inner functions $u$ and $v$.
### Second-Order Partial Derivative Chain Rule
Suppose $\LARGE f(u(x,y),v(x,y))$ is a composite function.
The second-order partial derivative of $f$ with respect to $x$ is given by:
$$\large \frac{\partial^2 f}{\partial x^2} = \frac{\partial^2 f}{\partial u^2} \left(\frac{\partial u}{\partial x}\right)^2 + 2 \cdot \frac{\partial^2 f}{\partial u \partial v} \cdot \frac{\partial u}{\partial x} \cdot \frac{\partial v}{\partial x} + \frac{\partial^2 f}{\partial v^2} \left(\frac{\partial v}{\partial x}\right)^2 + \frac{\partial f}{\partial u} \cdot \frac{\partial^2 u}{\partial x^2} + \frac{\partial f}{\partial v} \cdot \frac{\partial^2 v}{\partial x^2}$$

Here, $\LARGE \frac{\partial^2 f}{\partial u^2}$, $\LARGE \frac{\partial^2 f}{\partial v^2}$, and $\LARGE \frac{\partial^2 f}{\partial u \partial v}$ are the **second-order partial derivatives** of the outer function $f$.
$\LARGE \frac{\partial u}{\partial x}$​, $\LARGE \frac{\partial v}{\partial x}$, and their second derivatives $\LARGE \frac{\partial^2 u}{\partial x^2}$, $\LARGE \frac{\partial^2 v}{\partial x^2}$ are the **first and second-order partial derivatives** of the inner functions $u$ and $v$.
## Notation of the Four Variants of the Chain Rule for Multi-Variable Functions
Remember there is a single derivative for Single Variable Functions.
	And there are $n$ number of partial derivatives for $n$ Variable Functions.
###### $\LARGE s$: A [[Mapping#Scalar Functions as a Subset of Functions|Real-Valued]] function (i.e. a Scalar Function) of one $\LARGE \text{\textcolor{lightblue}{real variable}}$.
$$\LARGE s'(t)$$
$$\LARGE \textcolor{lightblue}{\frac{d}{dt}}$$
###### $\LARGE f$: A [[Mapping#Scalar Functions as a Subset of Functions|Real-Valued]] function (i.e. a Scalar Function) of $\LARGE \text{\textcolor{pink}{several real variables}}$.
$$\LARGE \text{\textcolor{lightgreen}{Gradient} } \nabla f = (f'_x, f'_y, f'_z)$$
$$\LARGE \textcolor{pink}{\frac{\partial}{\partial x}}$$
Where the $\LARGE f'_x, f'_y, f'_z$ which are each themselves the partial derivative functions, are the real-valued functions from $\LARGE \mathbb{R}^3 \to \mathbb{R}$ 
###### $\LARGE \vec{v}$: A [[Mapping#Higher-Level Functions (i.e. Composite Functions) Higher-Level Functions|Vector-Valued]] function (i.e. a Vector Function) of $\LARGE \text{\textcolor{lightblue}{one real variable}}$.
I.e. A function that takes a single variable and produces a vector. 
$$\LARGE \vec{v}'(t) = (x'(t), y'(t), z'(t))$$
$$\LARGE \textcolor{lightblue}{\frac{d}{dt}}$$
Where each component of the vector is differentiated individually. 
	Each component function is a Scalar Function.
		And the Outer/Higher-level Function is a vector function that produces a vector via a single variable and several component Scalar Functions. 
###### $\LARGE \nabla f$: A Vector function of $\LARGE \text{\textcolor{pink}{several real variables}}$.
$$\LARGE \text{\textcolor{pink}{Gradient} } \nabla f(x,y,z) = (f'_x, f'_y, f'_z)$$
$$\LARGE \textcolor{}{\frac{\partial}{\partial x}}$$
###### $\LARGE \phi$: A change of variables in $\LARGE \textcolor{pink}{\mathbb{R}^2}$ or in $\LARGE \textcolor{pink}{\mathbb{R}^3}$.
[[Jacobian Matrix|Jacobian Matrix]]
$$\LARGE \textcolor{pink}{\frac{\partial}{\partial x}}$$
## Most General Variant (of the Chain Rule) for Multi-Variable Functions
Occurs when both functions are functions of several variables $\mathbb{R}^n$ and are vector-valued.
	With help of the [[Jacobian Matrix|Jacobian Matrix]].
		The Chain Rule for composite functions can be expressed with the help of **[[Matrix Multiplication|matrix multiplication]].**
$$\LARGE \vec{x}=\vec{g}(\vec{t}): \mathbb{R}^q \to \mathbb{R}^n, \quad \text{ and } \quad \vec{y} = \vec{f}(\vec{x}): \mathbb{R}^n \to \mathbb{R}^m$$
$$\LARGE \vec{f} \circ \vec{g}: \mathbb{R}^q \xrightarrow{\vec{g}} \mathbb{R}^n \xrightarrow{\vec{f}} \mathbb{R}^m$$
The Derivatives of both $g(t)$ and $f(x)$ are Jacobian Matrices composed of the gradients of their respective component (i.e. lower-level) functions.
$$\LARGE D\vec{g}(\vec{t}) = \begin{pmatrix} \frac{\partial g_1}{\partial t_1} \space \dots \space \frac{\partial g_1}{\partial t_q} \\ \vdots \quad \ddots \quad \vdots \\ \frac{\partial g_n}{\partial t_1} \space \dots \space \frac{\partial g_n}{\partial t_q} \end{pmatrix}$$
$$\LARGE D\vec{f}(\vec{x}) = \begin{pmatrix} \frac{\partial f_1}{\partial x_1} \space \dots \space \frac{\partial f_1}{\partial x_n} \\ \vdots \quad \ddots \quad \vdots \\ \frac{\partial fm}{\partial x_1} \space \dots \space \frac{\partial f_m}{\partial x_n} \end{pmatrix}$$
##### The Jacobian Matrix of the Composition of these two functions will simply be the Matrix Product (i.e. using [[Matrix Multiplication|Matrix Multiplication]]) of the Jacobian of the first/outer/higher-level function times the Jacobian of the second/inner/lower-level function. 
$$\LARGE D(\vec{f} \circ \vec{g})(\vec{t}) = D\vec{f}(\vec{g}(\vec{t}))D\vec{g}(\vec{t})$$
This is very similar to the [[Derivatives#Chain Rule Chain Rule|Chain Rule of the Single Variable Chain Rule]], where the derivatives of the higher-level and lower level functions are scalars, and are multiplied.
	But in this multi-variable variant of the Chain Rule, the Derivatives themselves are Jacobian Matrices, which are multiplied together. 

$\LARGE (\vec{f} \circ \vec{g})(\vec{t})$ is a function from $\LARGE \mathbb{R}^q \xrightarrow{\vec{g}} \mathbb{R}^n \xrightarrow{\vec{f}} \mathbb{R}^m$.
	According to the Chain Rule for a given row $\LARGE \frac{\partial}{\partial t_j} (\vec{f} \circ \vec{g})_i(\vec{t})$ 
$$\frac{\partial}{\partial t_j} (\vec{f} \circ \vec{g})_i(\vec{t}) = \sum^n_{k=1} \frac{\partial f_i(\vec{g}(\vec{t}))}{\partial x_k} \cdot \frac{\partial g_k(\vec{t})}{\partial t_j} = \frac{\partial f_i(\vec{g}(\vec{t}))}{\partial x_1} \cdot \frac{\partial g_1(\vec{t})}{\partial t_j} + \dots + \frac{\partial f_i(\vec{g}(\vec{t}))}{\partial x_n} \cdot \frac{\partial g_n(\vec{t})}{\partial t_j}$$
Which is exactly the result in the row $\LARGE i$ and the column $\LARGE j$ in the matrix multiplication above ($\LARGE i = 1, \dots, m$ and $\LARGE j =1, \dots, q$) because the product of an $\LARGE m \times n$ matrix and an $\LARGE n \times q$ matrix is an $\LARGE m \times q$ matrix. 
## Chain Rule: Variant 0
The one-dimensional Chain Rule for an Outer 1D Scalar function, composed of an inner 1D Scalar Function. 
$$\LARGE f \circ g : \mathbb{R} \xrightarrow{g}\mathbb{R} \xrightarrow{f}  \mathbb{R}$$
$$\LARGE \frac{d}{dx}f(g(x)) =  f'(g(x)) \cdot g'(x)$$
$$\LARGE \text{With the notation } u = f(v),\space v = g(x)$$
$$\LARGE \text{We can write } \frac{du}{dx} = \frac{du}{dv} \cdot \frac{dv}{dx}, \quad u:\mathbb{R} \to \mathbb{R}$$
## Chain Rule: Variant 1
For a Vector Function composed of a Scalar Function.
	The derivative of the Scalar Function (i.e. the inner/lower-level function) is essentially the scaling factor of the derivative of the Vector Function.
$$\LARGE \vec{v} \circ s: \mathbb{R} \xrightarrow{s} \mathbb{R} \xrightarrow{\vec{v}} \mathbb{R}^n$$
$$\LARGE \frac{d}{dt}(\vec{v}(s(t))) = s'(t) \cdot \vec{v}'(s(t))$$
Function $t$ is a Scalar Function from R to R which takes a scalar as input and produces a scalar output value.
	The Function $s(t)$ is a Scalar Function which takes the function $t$ as input and produces a scalar output value.
		The function $\vec{v}(s(t))$ is a Vector Function which takes $s(t)$ as input and produces a vector output value.
$$\LARGE \vec{v}(t) = (x_1(t), \dots, x_n(t)) \quad \Rightarrow \quad \vec{v}'(t) = (x'_1(t), \dots, x'_n(t))$$

Because the component functions are Scalar Functions producing a single value, then for each of the derivatives of the composite component functions we can apply the [[Derivatives#Chain Rule Chain Rule of Single Variable Functions|single variable chain rule]].
$$\LARGE \frac{d}{dt}(\vec{v}(s(t)) = \left(\frac{d}{dt}(x_1(s(t)),\dots, \frac{d}{dt}(x_n(s(t)))\right) = $$
$$\LARGE = (x'_1(s(t)) \cdot s'(t), \dots, x'_n(s'(t)) \cdot s'(t))$$
Because the same scalar is applied to each coordinate i.e. component function of a vector, then the scalar $s'(t)$ can be factored out.
$$\LARGE =\frac{d}{dt}(\vec{v}(s(t))= s'(t)\cdot\vec{v}'(s(t))$$
## Chain Rule: Variant 2
For a Scalar Function that takes a Vector as input, then that produced Scalar becomes the input for the outer function which is another Scalar Function producing a Scalar. 
	*Remember, that a [[#$ LARGE f$ A Mapping Scalar Functions as a Subset of Functions Real-Valued function (i.e. a Scalar Function) of $ LARGE text{ textcolor{pink}{several real variables}}$.|Scalar Function that takes multiple variables]] implies utilizing partial derivatives.*
		The multi-variables are differentiated individually and each derivative of the inner/lower-level function (Scalar Function) is scaled by the derivative of the outer/higher-level function (also a Scalar Function).
			I.e. Multi-variable Derivatives scaled by Single-variable Derivatives.
$$\LARGE z = s \circ f : \mathbb{R}^2 \textcolor{pink}{\xrightarrow{f}} \mathbb{R} \textcolor{lightblue}{\xrightarrow{s}} \mathbb{R}$$
$$\LARGE \frac{\partial z}{\partial x} = \textcolor{lightblue}{\frac{ds}{dt}} \cdot \textcolor{pink}{\frac{\partial f}{\partial x}}, \quad \frac{\partial z}{\partial y} = \frac{ds}{dt} \cdot \frac{\partial f}{\partial y}$$
##### Example
$$\LARGE z = \arctan \frac{y}{x}$$
$$\LARGE  \textcolor{pink}{f(x,y) = \frac{y}{x}}$$
$$\LARGE \textcolor{lightblue}{s(t) = \arctan t}$$
## Chain Rule: Variant 3
The derivative of a composition of a multi-variable scalar function (outer) that takes as input, a single variable vector function.
	The most frequently used variant in our case.
		It is essentially the [[Dot Product|dot product]] (because of the two vectors in the equation) of the gradient (i.e. the vector composed of partial derivatives) of the outer function by the derivative of the [[#$ LARGE vec{v}$ A Mapping Higher-Level Functions (i.e. Composite Functions) Higher-Level Functions Vector-Valued function (i.e. a Vector Function) of $ LARGE text{ textcolor{lightblue}{one real variable}}$.|single variable vector function]].
			$\LARGE f(x,y)$ is a [[#$ LARGE f$ A Mapping Scalar Functions as a Subset of Functions Real-Valued function (i.e. a Scalar Function) of $ LARGE text{ textcolor{pink}{several real variables}}$.|multi-variable scalar function]].
			$\LARGE \vec{v}(t) = [x(t), y(t), z(t)]$ is a [[#$ LARGE vec{v}$ A Mapping Higher-Level Functions (i.e. Composite Functions) Higher-Level Functions Vector-Valued function (i.e. a Vector Function) of $ LARGE text{ textcolor{lightblue}{one real variable}}$.|Single Variable Vector Function]].
			$\LARGE \nabla f(x,y)$ is a [[#$ LARGE nabla f$ A Vector function of $ LARGE text{ textcolor{pink}{several real variables}}$.|Multi-Variable Vector Function]].
$$\LARGE f \circ \vec{v} : \mathbb{R} \xrightarrow{\vec{v}} \mathbb{R}^2 \xrightarrow{f} \mathbb{R}$$
$$\LARGE \frac{d}{dt} [f(\vec{v}(t))] = \nabla f(\vec{v}(t)) \cdot \vec{v}'(t) $$
$$\LARGE = \nabla f(\vec{v}(t)) \cdot \vec{v}'(t) = (\frac{\partial f}{\partial x} \cdot x'(t)) + (\frac{\partial f}{\partial y} \cdot y'(t)) + (\frac{\partial f}{\partial z} \cdot z'(t))$$
![[Pasted image 20240823064235.png]]![[Pasted image 20240823064316.png]]
Where $\LARGE [\alpha , \beta]$ is the interval of the domain of the parameter $\LARGE t$ of the vector function $\LARGE \vec{v} (t)$.
	$\LARGE \vec{v}(t)$ is the green curve.
		Therefore, $\LARGE \vec{v}(t)$ is now the domain of the outer function $\LARGE f(x,y)$ (i.e. the multi-variable scalar function).
			$\LARGE f(x,y)$ is the blue curve.
				$\LARGE z$ is the produced scalar as "height" along the $z$ axis for the interval of the domain on the plane. 
###### If the Curve of $f$ is a Level, Then the Composite Function is a Constant Function
![[Pasted image 20240823064934.png]]
##### Example of Variant 3
Determine $\LARGE \frac{d}{dt}f(\vec{v}(t))$ for $\LARGE f=(f_1,f_2f_3) = f(x,y,z) = xz + \cos y$ and $\LARGE \vec{v}(t) = (\sin t, t^2, \ln (t^2+1))$ 
$$\LARGE \text{Variant 3:} \space \nabla f(\vec{v}(t)) \cdot \vec{v}'(t) = (\frac{\partial f}{\partial x} \cdot x'(t)) + (\frac{\partial f}{\partial y} \cdot y'(t)) + (\frac{\partial f}{\partial z} \cdot z'(t))$$
###### Method 1:
$$\LARGE = \frac{d}{dt}f(\vec{v}(t)) = \textcolor{red}{f'_1(\vec{v}(t))}\cdot \textcolor{violet}{x'(t)} + \textcolor{green}{f'_2(\vec{v}(t))}\cdot \textcolor{teal}{y'(t)}  + \textcolor{orange}{f'_3(\vec{v}(t))}\cdot \textcolor{gray}{z'(t)} $$
$$\LARGE \text{Where} \quad \textcolor{red}{f'_1(x,y,z) = \frac{\partial f}{\partial x}xz+\cos y  = z}$$
$$\LARGE \textcolor{gray}{z(t) = \ln(t^2+1)}$$
$$\LARGE \text{Plug } \textcolor{gray}{z(t)} \text{ into } \textcolor{red}{z \text{ of }f'_1 =\frac{\partial f}{\partial x} xz+ \cos y} = \textcolor{red}{\frac{\partial f}{\partial x}\textcolor{gray}{\ln (t^2 + 1)}z + \cos y}$$
$$\LARGE \textcolor{red}{f'_1(\vec{v}(t))_z = f'_1(\textcolor{gray}{z(t)}) = \frac{\partial f}{\partial x}xz+\cos y} = \textcolor{red}{\ln(t^2 +1)}$$
$$\LARGE \text{And } \quad \textcolor{gray}{\vec{v}'(t)_z = z'(t) = \frac{d}{dt}\ln(t^2+1) = \frac{2t}{1+t^2}}$$
$$\LARGE \text{Where }\quad\textcolor{green}{f'_2(x,y,z) = \frac{\partial f}{\partial y}xz+\cos y = -\sin y}$$
$$\LARGE \textcolor{teal}{y(t) = t^2}$$
$$\LARGE \text{Plug } \textcolor{teal}{y(t)} \text{ into } \textcolor{green}{y\text{ of }f'_2 =\frac{\partial f}{\partial y} xz+ \cos y} = \textcolor{green}{\frac{\partial f}{\partial y}xz + \cos }\textcolor{teal}{t^2}$$
$$\LARGE \textcolor{green}{f'_2(\vec{v}(t))_y = f'_2(\textcolor{teal}{y(t)}) = \frac{\partial f}{\partial y}xz+\cos y = -\sin t^2}$$
$$\LARGE \text{And} \quad \textcolor{teal}{\vec{v}'(t)_y = y'(t) = \frac{d}{dt}t^2 = 2t}$$
$$\LARGE \text{Where} \quad \textcolor{orange}{f'_3(x,y,z) = \frac{\partial f}{\partial z}xz+\cos y = x}$$
$$\LARGE \textcolor{violet}{x(t) = \sin t}$$
$$\LARGE \text{Plug } \textcolor{violet}{x(t)} \text{ into } \textcolor{orange}{z \text{ of }f'_1 =\frac{\partial f}{\partial z} xz+ \cos y} = \textcolor{orange}{\frac{\partial f}{\partial x}x\textcolor{violet}{\sin t} + \cos y }$$
$$\LARGE \textcolor{orange}{f'_3(\vec{v}(t))_x = f'_3(\textcolor{violet}{x(t)}) = \frac{\partial f}{\partial z}xz+\cos y =\textcolor{violet}{\sin t}}$$
$$\LARGE \text{And } \quad \textcolor{violet}{\vec{v}'(t)_x =x'(t) = \frac{d}{dt}\sin t  = \cos t}$$
###### Method 2:
Compute the composition $\LARGE f(\vec{v}(t))$ and differentiate it as a function of one variable (i.e. single variable derivative/differentiation).

$$\LARGE f=(\textcolor{red}{f_1},\textcolor{green}{f_2},\textcolor{orange}{f_3}) = f(\textcolor{red}{x},\textcolor{green}{y},\textcolor{orange}{z}) = \textcolor{red}{x}\textcolor{orange}{z} + \cos \textcolor{green}{y}$$
$$\LARGE \vec{v}(t) = (\textcolor{red}{x(t)}, \textcolor{green}{y(t)}, \textcolor{orange}{z(t)}) = (\textcolor{red}{\sin t}, \textcolor{green}{t^2}, \textcolor{orange}{\ln (t^2+1)})$$
$$\LARGE f(\vec{v}(t)) = \textcolor{red}{\sin t} \cdot \textcolor{orange}{\ln (t^2+1)} + \cos \textcolor{green}{t^2}$$
$$\LARGE \frac{d}{dt}f(\vec{v}(t)) = \cos t \cdot \textcolor{orange}{\ln(t^2+1)} + \textcolor{red}{\sin t} \cdot \frac{2t}{t^2+1} - 2t\sin \textcolor{green}{t^2}$$
## Proof of Variant 3
$$\LARGE z(t) = f(x(t), y(t))$$
##### 1. Replace $\LARGE z(t)$$ with $\LARGE f(x(t),y(t))$ 
##### 2. Find Limit of $\LARGE f(x(t), y(t))$
$$\LARGE z'(t) = \lim\limits_{h \to 0} \frac{z(t+h) - z(t)}{h}$$
$$\LARGE = \lim\limits_{h \to 0} \frac{f(x(t +h), y(t +h)) - f(x(t), y(t))}{h}$$
##### 3. Obtain the Partial Derivatives via Typical Trick (subtraction and addition) of $\textcolor{teal}{\text{Same Terms}}$ in Order to Eliminate Each in Either Equation
This produces two equations, where in each, one coordinate becomes constant.
	Therefore, the other coordinate is the only one to change, that is, the equation becomes a partial derivative. 
$$ = \lim\limits_{h \to 0} \frac{f(x(t +h), y(t +h)) - \textcolor{teal}{f(x(t), y(t +h))}}{h} + \lim\limits_{h \to 0} \frac{\textcolor{teal}{f(x(t +h), y(t +h))} - f(x(t), y(t))}{h}$$
$$ = \lim\limits_{h \to 0} \frac{f(\textcolor{red}{x(t +h)}, \textcolor{}{y(t +h)}) - f(\textcolor{red}{x(t)}, \textcolor{}{y(t +h)})}{h} + \lim\limits_{h \to 0} \frac{f(\textcolor{}{x(t +h)}, \textcolor{green}{y(t +h)}) - \textcolor{}{f(x(t)}, \textcolor{green}{y(t)})}{h}$$
##### 4. Apply the [[Derivatives#Chain Rule Chain Rule of Single Variable Functions|Basic Chain Rule From Single-Variable Derivatives]]
$$\LARGE = \textcolor{red}{f'_1(x(t), y(t))} \cdot \textcolor{orange}{x'(t)} + \textcolor{green}{f'_2(x(t), y(t))} \cdot \textcolor{orange}{y'(t)} = \textcolor{violet}{(\frac{\partial f}{\partial x}, \frac{\partial f}{\partial y})} \cdot \textcolor{orange}{(x'(t), y'(t))}$$
$$\LARGE = \textcolor{violet}{\nabla f(\vec{v}(t))} \cdot \textcolor{orange}{\vec{v'}(t)}$$
$$\text{Where the gradient is "dotted" (dot product) with the derivative of the vector}$$
$\LARGE \frac{\partial f}{\partial x}$​ and $\LARGE \frac{\partial f}{\partial y}$ are **first-order partial derivatives** of the scalar function $f$ with respect to its variables $x$ and $y$. 
	These partial derivatives describe how $f$ changes with respect to changes in $x$ and $yy$, assuming the other variable is held constant.
		$\LARGE \nabla f(\vec{v}(t))$ is the **gradient vector** of the function $f$ at the point $\LARGE \vec{v}(t)$.

The terms $\LARGE x′(t)$ and $\LARGE y′(t)$ represent the **first-order derivatives** of the functions $\LARGE x(t)$ and $\LARGE y(t)$ with respect to the parameter $t$. 
	These derivatives describe how the variables $x$ and $y$ change with respect to the parameter $t$.
		$\LARGE \vec{v'}(t)$ is the vector of the **first-order derivatives** $\LARGE x′(t)$ and $\LARGE y'(t)$.
## Chain Rule: Variant 4
The Derivative of $\LARGE z$ which is the scalar product of a composition of a multi-variable scalar function, which has as input variable changing functions.
##### $\LARGE z =f(x, y) = f(x(s,t), y(s,t))$
$$\LARGE f \circ \Phi: \mathbb{R}^2 \xrightarrow{\Phi} \mathbb{R}^2 \xrightarrow{f} \mathbb{R}$$
Where $\LARGE \Phi$, a [[#$ LARGE phi$ A change of variables in $ LARGE textcolor{pink}{ mathbb{R} 2}$ or in $ LARGE textcolor{pink}{ mathbb{R} 3}$.|change of variables]] in $\LARGE \mathbb{R}^2$, is defined as: $\LARGE \textcolor{orange}{x} = \textcolor{orange}{x}(\textcolor{red}{s},\textcolor{green}{t}),\quad \textcolor{violet}{y} = \textcolor{violet}{y}(\textcolor{red}{s},\textcolor{green}{t})$.
	Where $\LARGE s$ and $\LARGE t$ each require their own partial derivatives.
		$\LARGE f(x,y)$ is a [[#$ LARGE f$ A Mapping Scalar Functions as a Subset of Functions Real-Valued function (i.e. a Scalar Function) of $ LARGE text{ textcolor{pink}{several real variables}}$.|multi-variable scalar function]].
		$\LARGE \Phi$ (i.e. $\LARGE x(s,t), y(s,t)$) is/are a [[#$ LARGE nabla f$ A Vector function of $ LARGE text{ textcolor{pink}{several real variables}}$.|Multi-Variable Vector Function(s)]].
		$\LARGE \nabla f(x,y)$ is a [[#$ LARGE nabla f$ A Vector function of $ LARGE text{ textcolor{pink}{several real variables}}$.|Multi-Variable Vector Function]] (i.e. a gradient of a partial variables of a scalar function $\LARGE f$).
### "Change of Variables"
Refers to a mathematical process where you express a function in terms of a new set of variables, instead of the original ones.
	This is often done to simplify a problem, make computations easier, or because the new variables might better reflect the structure of the problem.
##### Coordinate Systems and Transformations
Imagine you are working with a function $f(x,y)$ that depends on two variables, $x$ and $y$. 
	These variables are in a particular **coordinate system** (e.g., Cartesian coordinates).
		Now, suppose you want to **change the coordinate system** by introducing new variables $s$ and $t$, where $x$ and $y$ are now functions of $s$ and $t$. 
			**This transformation is described by the function $\LARGE \Phi(s, t)$, which maps the new coordinates $(s, t)$ to the original coordinates $(x, y).**
				In the context of a "change of variables," the function $\LARGE \Phi$ is typically a **vector-valued function** that maps one set of variables (like $s$ and $t$) to another $t$ of variables (like $x$ and $y$).
					$\LARGE \Phi$ is a [[#Direct Transformations|Direct Transformation]].

I.e. In the function $f(x, y)$ that depends on two variables $x$ and $y$. 
	A change of variables occurs when you introduce new variables, say $s$ and $t$, and express $x$ and $y$ in terms of $s$ and $t$.
		Where instead of working directly with $x$ and $y$, you work with $s$ and $t$. 
			The function $f(x, y)$ now becomes a function of $s$ and $t$ through $x(s,t)$ and $y(s,t)$:
$$\LARGE z = f(x, y) = f(x(s,t), y(s,t))$$
#### Inner Functions, $\LARGE \Phi$
The transformation function $\LARGE \Phi$ can indeed be considered a **vector-valued function** that is composed of **scalar functions**.
	Furthermore, when viewed in the context of transformations and changes of variables, $\Phi$ can also be thought of as part of a **composite function**.

This is the function or transformation that maps the variables $s$ and $t$ to the variables $x$ and $y$, where: 
$$\LARGE \Phi(s, t) = (x(s,t), y(s,t))$$
The $\Phi$ function in this context is referring specifically to the change of variables that maps from the variables $s$ and $t$ to $x$ and $y$.
	This mapping is captured by the functions $x(s,t)$ and $y(s,t)$. 
		Therefore, $\Phi$ represents the transformation from the $(s,t)$ coordinate system to the $(x,y)$ coordinate system.

The functions $\LARGE x(s,t)$ and $\LARGE y(s,t)$ together form the mapping that is referred to as the $\LARGE\Phi$ function in this context.
	$\LARGE \Phi(s,t)$ is a vector-valued function that represents the transformation from the new variables $s$ and $t$ to the original variables $x$ and $y$.
		This means: 
$$\LARGE \Phi(\textcolor{red}{s}, \textcolor{green}{t}) = \begin{pmatrix} \textcolor{orange}{x}(\textcolor{red}{s},\textcolor{green} {t}) \\ \textcolor{violet}{y}(\textcolor{red}{s}, \textcolor{green}{t}) \end{pmatrix}$$
This is a vector function that takes the input variables $s$ and $t$ (which are in $\LARGE \mathbb{R}^2$) and outputs a pair of new variables, $x$ and $y$, also in $\LARGE \mathbb{R}^2$.
	**Input:** The function $\LARGE \Phi$ takes a point $\LARGE (s, t)$ in $\LARGE \mathbb{R}^2$.
	**Output:** The output is a new point $\LARGE (x(s,t), y(s,t))$ in $\LARGE \mathbb{R}^2$, where $x$ and $y$ are functions of $s$ and $t$.
##### $\LARGE \Phi$ as a Vector Function
$\LARGE \Phi$ is a function that maps from one coordinate space to another.
	Specifically, if 
$$\LARGE \Phi : \mathbb{R}^n \to \mathbb{R}^m$$
		then  $\Phi$  takes a vector from  $\mathbb{R}^n$ and produces a vector in $\mathbb{R}^m$.

The function $\Phi$ can be written as a vector whose components are scalar functions. 
	For example, if 
$$\LARGE \Phi : \mathbb{R}^2 \to \mathbb{R}^2$$ it could look like this:
$$\LARGE \Phi(s,t) = 
\begin{pmatrix}
x(s,t) \\
y(s,t)
\end{pmatrix}$$
Where $x(s,t)$ and $y(s,t)$ are scalar functions of the variables $s$ and $t$.
##### $\LARGE \Phi$ as a Composite Function
![[Pasted image 20240825133440.png]]
When you have a scalar function $f(x,y)$ and you express the variables $x$ and $y$ in terms of new variables $s$ and $t$, the function $f$ becomes a composite function.
	This is because $f$ is now being evaluated with inputs that are themselves functions of other variables

In this case, the overall function $\LARGE f \circ \Phi$ can be written as:
$$\LARGE f(x(s,t), y(s,t)) = f(\Phi(s,t))$$
Here,$f$ is composed with the vector function $\LARGE \Phi$, making $f \circ \Phi$ a composite function.
	The scalar output of $f$ depends on the transformed variables $x(s,t)$ and $y(s,t)$, which are the components of the vector function $\Phi$.

When you want to understand how this transformation affects the function $f$, you use the **Jacobian matrix** of $\Phi$, which is built from the partial derivatives of the scalar functions $x(s,t)$ and $y(s,t)$. 
	The Jacobian helps apply the **chain rule** to compute derivatives of the composite function $\circ \Phi$ with respect to the new variables $s$ and $t$.
##### The Derivative of $\Phi$ (a [[Jacobian Matrix|Jacobian Matrix]])
$$\LARGE D\Phi = \begin{pmatrix} \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{red}{s}} \space \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{green}{t}} \\ \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{red}{s}} \space \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{green}{t}} \end{pmatrix}$$

The **Jacobian matrix** $\LARGE D\Phi$ tells us how the new coordinates $s$ and $t$ relate to the old coordinates $x$ and $y$. 
	Specifically, it provides the partial derivatives of the old coordinates with respect to the new ones.
		The Jacobian matrix $D\Phi$ captures how $x$ and $y$ change with respect to $s$ and $t$.
				I.e. It consists of the partial derivatives of $x$ and $y$ with respect to $s$ and $t$.
### Outer Function $f$
The function $f$ takes the transformed variables $x(s,t)$ and $y(s,t)$ as its inputs.
	So $f(x(s,t), y(s,t))$ represents the composition $f \circ \Phi$.
		The gradient of $f$ is with respect to $x$ and $y$, not directly with respect to $s$ and $t$. 
			However, using the chain rule, the gradient of $f$ in the new coordinates $(s,t)$ involves both the gradient of $f$ with respect to $x$ and $y$ and the Jacobian matrix $D\Phi$.
##### The Derivative of $f$ (a [[Gradients|gradient]])
$$\LARGE \nabla f = \begin{pmatrix} \frac{\partial f}{\partial \textcolor{orange}{x}} , \frac{\partial f}{\partial \textcolor{violet}{y}} \end{pmatrix}$$
##### Variant 4 Chain Rule $\LARGE z'$ (i.e. the Derivative of the Composite Function)
$\LARGE z$ is the value of the function $f$ evaluated at the transformed variables $x(s,t)$ and $y(s,t)$. 
	In other words, $z$ represents the output of the function after the change of variables has been applied.
		The matrix multiplication $\LARGE \nabla f \cdot D\Phi$ combines the information about the rate of change of the function $f$ (in terms of the original variables $x$ and $y$) with the information about how the coordinates themselves change (from the new variables $s$ and $t$ to $x$ and $y$).
$$\LARGE \nabla f \cdot D\Phi = \nabla f = \begin{pmatrix} \frac{\partial f}{\partial \textcolor{orange}{x}} , \frac{\partial f}{\partial \textcolor{violet}{y}} \end{pmatrix} \cdot D\Phi = \begin{pmatrix} \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{red}{s}} \space \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{green}{t}} \\ \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{red}{s}} \space \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{green}{t}} \end{pmatrix} =$$
$$\LARGE = \begin{pmatrix} \frac{\partial z}{\partial \textcolor{orange}{x}} \cdot \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{red}{s}} + \frac{\partial z}{\partial \textcolor{violet}{y}} \cdot \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{red}{s}}, \space  \frac{\partial z}{\partial \textcolor{orange}{x}} \cdot \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{green}{t}} + \frac{\partial z}{\partial \textcolor{violet}{y}} \cdot \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{green}{t}} \end{pmatrix} = \begin{pmatrix} \frac{\partial z}{\partial \textcolor{red}{s}}, \space \frac{\partial z}{\partial \textcolor{green}{t}}\end{pmatrix}$$
#### For $\mathbb{R}^3$
![[Pasted image 20240825142726.png]]

## Examples of Problems Using Variants
#### 1. Variant 4 Example
$$\LARGE f: \mathbb{R^2} \to \mathbb{R^n}, \quad u, v: \mathbb{R^2} \to \mathbb{R}$$
$$\LARGE f(u(x,t), v(y,t)), \quad u(x,t) = xt, \quad v(y,t) = yt$$
![[Pasted image 20240826160738.png]]
#### 2. Variant 3 Example
$$\LARGE f: \mathbb{R^2} \to \mathbb{R^n}, \quad u: \mathbb{R^2} \to \mathbb{R}, \quad v: \mathbb{R} \to \mathbb{R}$$
$$\LARGE f(u(x,y), v(x)), \quad u(x,y) = xy^2, \quad v(x) = x^3$$
![[Pasted image 20240826155010.png]]
#### 3. General Variant Example
$$\LARGE = \textcolor{red}{f'_1(x(t), y(t))} \cdot \textcolor{orange}{x'(t)} + \textcolor{green}{f'_2(x(t), y(t))} \cdot \textcolor{orange}{y'(t)} = \textcolor{violet}{(\frac{\partial f}{\partial x}, \frac{\partial f}{\partial y})} \cdot \textcolor{orange}{(x'(t), y'(t))}$$
$$\LARGE f: \mathbb{R^2} \to \mathbb{R^n}, \quad u: \mathbb{R^2} \to \mathbb{R}, \quad v: \mathbb{R} \to \mathbb{R}$$
$$\LARGE z(x,y,z) = f(u(x,y), v(y,z)), \quad u(x,y) = \frac{x}{y}, \quad v(y,z) = \frac{y}{z}$$
![[Pasted image 20240827055027.png|400]]
![[Pasted image 20240827054949.png]]
![[Pasted image 20240827054900.png]]
#### 4. Variant 4 Example
$$\LARGE f: \mathbb{R^2} \to \mathbb{R}, \quad x,y: \mathbb{R^2} \to \mathbb{R}$$
$$\LARGE z= f(x(s,t), y(s,t)), \quad x(s,t) = 2s+3t, \quad y(s,t) = 3s-2t$$
###### Variant 4 Chain Rule
$$\LARGE \left( \frac{\partial z}{\partial s},  \frac{\partial z}{\partial t} \right)= \nabla f \cdot D\Phi = \nabla f = \begin{pmatrix} \frac{\partial f}{\partial \textcolor{orange}{x}} , \frac{\partial f}{\partial \textcolor{violet}{y}} \end{pmatrix} \cdot D\Phi = \begin{pmatrix} \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{red}{s}} \space \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{green}{t}} \\ \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{red}{s}} \space \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{green}{t}} \end{pmatrix} =$$
$$\LARGE  \left(\frac{\partial z}{\partial s},  \frac{\partial z}{\partial t}\right) = \begin{pmatrix} \frac{\partial z}{\partial \textcolor{orange}{x}} \cdot \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{red}{s}} + \frac{\partial z}{\partial \textcolor{violet}{y}} \cdot \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{red}{s}}, \space  \frac{\partial z}{\partial \textcolor{orange}{x}} \cdot \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{green}{t}} + \frac{\partial z}{\partial \textcolor{violet}{y}} \cdot \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{green}{t}} \end{pmatrix} = \begin{pmatrix} \frac{\partial z}{\partial \textcolor{red}{s}}, \space \frac{\partial z}{\partial \textcolor{green}{t}}\end{pmatrix}$$
##### 1. Obtain [[#First Order Partial Derivatives|First Order Partial Derivatives]] of $x,y$ with Respect to $s,t$
![[Pasted image 20240827060259.png]]
$$\LARGE \text{Where the First Order Partial Derivatives of } x,y \space \text{ wrt to } s,t \text{ are:} $$
$$\LARGE D\Phi = \begin{pmatrix}\textcolor{violet}{\frac{\partial x}{\partial s} = 2 \quad \frac{\partial x}{\partial t} = 3} \\ \textcolor{lightgreen}{\quad \frac{\partial y}{\partial s} = 3 \quad \frac{\partial y}{\partial t} = - 2}\end{pmatrix}$$
##### 2. Obtain First Order Derivatives of $z$  (i.e. the composite function) with Respect to $s, t$
![[Pasted image 20240827063645.png]]
$$\LARGE \text{The Chain Rule: }\quad \frac{\partial z}{\partial \textcolor{red}{s}} = \frac{\partial z}{\partial \textcolor{orange}{x}} \cdot \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{red}{s}} + \frac{\partial z}{\partial \textcolor{violet}{y}} \cdot \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{red}{s}}$$
$$\LARGE \text{Substitute the Partial Derivatives: } \quad \textcolor{violet}{\frac{\partial x}{\partial s} = 2},  \textcolor{lightgreen}{\quad \frac{\partial y}{\partial s} = 3}$$
$$\large \text{Therefore, the First Order Derivative wrt s of the Composite Function is: }$$
$$\LARGE \textcolor{orange}{\frac{\partial z}{\partial s}} = \frac{\partial z}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial s}} + \frac{\partial z}{\partial y} \cdot \textcolor{lightgreen}{\frac{\partial y}{\partial s}} = \textcolor{violet}{2}\frac{\partial z}{\partial x} + \textcolor{lightgreen}{3} \frac{\partial z}{\partial y}$$
$$\large \text{And, the First Order Derivative wrt t of the Composite Function is: }$$
$$\LARGE \textcolor{teal}{\frac{\partial z}{\partial t}} = \frac{\partial z}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial t}} + \frac{\partial z}{\partial y} \cdot \textcolor{lightgreen}{\frac{\partial y}{\partial t}} = \textcolor{violet}{3}\frac{\partial z}{\partial x} + \textcolor{lightgreen}{-2} \frac{\partial z}{\partial y}$$
##### 3. Obtain the [[#Second Order Partial Derivatives|Second Order Partial Derivatives]] of $z$ (i.e. the composite function) with Respect to $s,t$
I.e. the First Order Derivative of the First Order Derivative.
	*Use the [[Linearity of Differentiation]] where the derivative of this sum is equal to sum of the derivatives and the constants.*	
###### A. Obtain the [[#Second Order Partial Derivatives|Second Order Partial Derivatives]] of $x,y$ with Respect to $s$
$$\LARGE \text{Second Order Derivatives: } \quad \frac{\partial^2 f}{\partial x_i^2} = \frac{\partial}{\partial x_i} \left( \frac{\partial f}{\partial x_i} \right)$$
$$\LARGE \text{Where } x_i \text{ is a component of the Vector }x=[x_1,x_2,\dots,x_i]$$
$$\large \text{Where } \quad \nabla z = \begin{pmatrix}\frac{\partial z}{\partial x} \\ \frac{\partial z}{\partial y} \end{pmatrix}$$
$$\text{And } \quad\large D\Phi = \begin{pmatrix}\textcolor{violet}{\frac{\partial x}{\partial s} = 2 \quad \frac{\partial x}{\partial t} = 3} \\ \textcolor{lightgreen}{\quad \frac{\partial y}{\partial s} = 3 \quad \frac{\partial y}{\partial t} = - 2}\end{pmatrix}$$
$$\LARGE \textcolor{orange}{\frac{\partial z}{\partial s}} = \nabla z \cdot D\Phi$$
$$\large \textcolor{orange}{\frac{\partial z}{\partial s}} = \frac{\partial z}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial s}} + \frac{\partial z}{\partial y} \cdot \textcolor{lightgreen}{\frac{\partial y}{\partial s}} = \textcolor{violet}{2}\frac{\partial z}{\partial x} + \textcolor{lightgreen}{3} \frac{\partial z}{\partial y}$$
$$\LARGE \frac{\partial^2 z}{\partial s^2} = \frac{\partial}{\partial s} \left( \frac{\partial z}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial s}} + \frac{\partial z}{\partial y} \cdot \textcolor{lightgreen}{\frac{\partial y}{\partial s}} \right)$$
$$\large \frac{\partial^2 z}{\partial s^2} = \frac{\partial}{\partial s}\left( \textcolor{orange}{\frac{\partial z}{\partial s}}\right), \space \text{Second Order Partial Derivative of } \textcolor{orange}{\frac{\partial z}{\partial s}} = \textcolor{violet}{2}\frac{\partial z}{\partial x} + \textcolor{lightgreen}{3} \frac{\partial z}{\partial y}$$
$$\LARGE \text{Substitute the expression, } \textcolor{violet}{2}\frac{\partial z}{\partial x} + \textcolor{lightgreen}{3} \frac{\partial z}{\partial y}, \text{ for } \textcolor{orange}{\frac{\partial z}{\partial s}}$$
$$\LARGE \frac{\partial^2 z}{\partial s^2} = {\frac{\partial}{\partial s} }\left( \textcolor{orange}{\frac{\partial z}{\partial s}} \right) = {\frac{\partial}{\partial s} }\left(\textcolor{violet}{2}\frac{\partial z}{\partial x} + \textcolor{lightgreen}{3} \frac{\partial z}{\partial y}\right)$$
$$\LARGE \text{Distribute } \frac{\partial}{\partial s} \text{ to Expand the Equation:}$$
$$\LARGE = \textcolor{violet}{2} \frac{\partial}{\partial s} \left(\frac{\partial z}{\partial x}\right) + \textcolor{lightgreen}{3} \frac{\partial}{\partial s}  \left( \frac{\partial z}{\partial y}\right)$$
![[Pasted image 20240827064744.png|400]]
###### B. Applying the Chain Rule Again (i.e. Taking the Partial Derivative of the Partial Derivative of z wrt s), $\LARGE \frac{\partial}{\partial s} \left( \frac{\partial z}{\partial x} \right)$
$$\LARGE \text{The 1st Order Chain Rule: }\quad \frac{\partial z}{\partial \textcolor{red}{s}} = \frac{\partial z}{\partial \textcolor{orange}{x}} \cdot \frac{\partial \textcolor{orange}{x}}{\partial \textcolor{red}{s}} + \frac{\partial z}{\partial \textcolor{violet}{y}} \cdot \frac{\partial \textcolor{violet}{y}}{\partial \textcolor{red}{s}}$$
$$\LARGE \quad \frac{\partial^2 z}{\partial s^2} = \frac{\partial}{\partial s}\left( \textcolor{orange}{\frac{\partial z}{\partial s}}\right)$$
$$\large \text{Remember, } \quad \textcolor{orange}{\frac{\partial z}{\partial s}} = \frac{\partial z}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial s}} + \frac{\partial z}{\partial y} \cdot \textcolor{lightgreen}{\frac{\partial y}{\partial s}} = \textcolor{violet}{2}\frac{\partial z}{\partial x} + \textcolor{lightgreen}{3} \frac{\partial z}{\partial y}$$
$$\LARGE \text{And }\quad \frac{\partial^2 z}{\partial s^2} = \frac{\partial}{\partial s} \left( \frac{\partial z}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial s}} + \frac{\partial z}{\partial y} \cdot \textcolor{lightgreen}{\frac{\partial y}{\partial s}} \right)$$
$$\LARGE \text{Substitute the expression, } \textcolor{violet}{2}\frac{\partial z}{\partial x} + \textcolor{lightgreen}{3} \frac{\partial z}{\partial y}, \text{ for } \textcolor{orange}{\frac{\partial z}{\partial s}}$$
$$\LARGE \frac{\partial^2 z}{\partial s^2} = {\frac{\partial}{\partial s} }\left( \textcolor{orange}{\frac{\partial z}{\partial s}} \right) = {\frac{\partial}{\partial s} }\left(\textcolor{violet}{2}\frac{\partial z}{\partial x} + \textcolor{lightgreen}{3} \frac{\partial z}{\partial y}\right)$$
$$\large \text{And} \left(\frac{\partial}{\partial s}\right) \text{ has been distributed:}$$
$$\LARGE \frac{\partial^2 z}{\partial s^2}  = \textcolor{violet}{2} \textcolor{yellow}{\frac{\partial}{\partial s} \left(\frac{\partial z}{\partial x}\right)} + \textcolor{lightgreen}{3} \frac{\partial}{\partial s}  \left( \frac{\partial z}{\partial y}\right)$$
$$\LARGE \text{\textcolor{yellow}{Differentiating $\LARGE \frac{\partial z}{\partial x}$​ with respect to $s$} = } \textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial x} \right)} $$
Differentiate $\LARGE \frac{\partial z}{\partial x}$​ and $\LARGE \frac{\partial z}{\partial y}$​ with respect to $s$, so **apply the chain rule again, to** $\LARGE \frac{\partial}{\partial s}\left( \frac{\partial z}{\partial x} \right)$
	*Remember that we already differentiated $\LARGE \frac{\partial z}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial s}}$  as a component of $\LARGE \frac{\partial z}{\partial s}$*.
		Now we are doing it again, to get the Second Order Partial Derivative of $\LARGE \frac{\partial z}{\partial s}$ which is $\LARGE \frac{\partial^2 z}{\partial s^2}$.
$$\LARGE \text{The 2nd Order Chain Rule: } \textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial x} \right)} = \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial s}} + \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial y} \cdot \textcolor{lightgreen}{\frac{\partial y}{\partial s}}$$
$$\LARGE \text{Where: } \quad \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x} == \frac{\partial}{\partial x} \left(\frac{\partial z}{\partial x}\right), \quad \text{and }\quad \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial y}  =\space \frac{\partial}{\partial x} \left(\frac{\partial z}{\partial y}\right) $$
##### Why $\LARGE \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x}$ and $\LARGE \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x}$ Appears
This term appears because you are applying the chain rule to the partial derivative $\LARGE \frac{\partial z}{\partial x}$ with respect to another variable $s$.
	The chain rule in multivariable calculus tells us that when we take the derivative of a function that depends on multiple variables, we must account for how each of those variables changes.
		The term $\LARGE \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x}​$​ in the second-order derivative is analogous to the term $\LARGE \frac{\partial z}{\partial x}​$ in the first-order chain rule, which itself represents how $z$ changes with respect to $x$. 
			The term $\LARGE \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x}​$ represents how $\LARGE \frac{\partial z}{\partial x}$​ changes with respect to $x$ as $s$ changes.
$$\large \text{Substitute known Partials: } \quad \textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial x} \right)} = \frac{\partial}{\partial x} \left(\frac{\partial z}{\partial x}\right) \cdot \textcolor{violet}{2} + \frac{\partial}{\partial x} \left(\frac{\partial z}{\partial y}\right)\cdot \textcolor{lightgreen}{3}$$
$$\LARGE \text{Where: } \quad \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x} == \frac{\partial}{\partial x} \left(\frac{\partial z}{\partial x}\right) = \frac{\partial^2 z}{\partial x} $$
$$\LARGE \text{And Where: } \quad \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial y} == \frac{\partial}{\partial y} \left(\frac{\partial z}{\partial x}\right) = \frac{\partial^2 z}{\partial x \partial y} $$

$$\LARGE \text{Simplify: } \quad \frac{\partial}{\partial s} \left( \frac{\partial z}{\partial x} \right) = \frac{\partial ^2 z}{\partial x^2} \cdot \textcolor{violet}{2} + \frac{\partial^2 z}{\partial x \partial y} \cdot \textcolor{lightgreen}{3}$$
$$\LARGE \textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial x} \right)} = \textcolor{violet}{2} \frac{\partial ^2 z}{\partial x^2} +  \textcolor{lightgreen}{3} \frac{\partial^2 z}{\partial x \partial y}$$
$$\LARGE \text{Reinsert } \textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial x} \right)} \text{ back into } \frac{\partial^2 z}{\partial s^2}  = \textcolor{violet}{2} \textcolor{yellow}{\frac{\partial}{\partial s} \left(\frac{\partial z}{\partial x}\right)} + \textcolor{lightgreen}{3} \frac{\partial}{\partial s}  \left( \frac{\partial z}{\partial y}\right)$$
$$\LARGE =\frac{\partial^2 z}{\partial s^2}  = \textcolor{violet}{2} \left(\textcolor{violet}{2} \frac{\partial ^2 z}{\partial x^2} +  \textcolor{lightgreen}{3} \frac{\partial^2 z}{\partial x \partial y}\right)+ \textcolor{lightgreen}{3} \frac{\partial}{\partial s}  \left( \frac{\partial z}{\partial y}\right)$$
![[Pasted image 20240827065615.png]]
$$\LARGE \text{\textcolor{yellow}{Differentiating $\LARGE \frac{\partial z}{\partial y}$​ with respect to $s$} = } \textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial y} \right)} $$
$$\LARGE \text{We have: } \frac{\partial^2 z}{\partial s^2}  = \textcolor{violet}{2} \left(\textcolor{violet}{2} \frac{\partial ^2 z}{\partial x^2} +  \textcolor{lightgreen}{3} \frac{\partial^2 z}{\partial x \partial y}\right)+ \textcolor{lightgreen}{3} \textcolor{yellow}{\frac{\partial}{\partial s}  \left( \frac{\partial z}{\partial y}\right)}$$
Differentiate $\LARGE \frac{\partial z}{\partial x}$​ and $\LARGE \frac{\partial z}{\partial y}$​ with respect to $s$, so **apply the chain rule again, to** $\LARGE \frac{\partial}{\partial s}\left( \frac{\partial z}{\partial y} \right)$
	*Remember that we already differentiated $\LARGE \frac{\partial z}{\partial x} \cdot \textcolor{violet}{\frac{\partial y}{\partial s}}$  as a component of $\LARGE \frac{\partial z}{\partial s}$*.
		Now we are doing it again, to get the Second Order Partial Derivative of $\LARGE \frac{\partial z}{\partial s}$ which is $\LARGE \frac{\partial^2 z}{\partial s^2}$.
$$\large \text{The 2nd Order Chain Rule: } \textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial y} \right)} = \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial s}} + \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial y} \cdot \textcolor{lightgreen}{\frac{\partial y}{\partial s}}$$
$$\LARGE \text{Where: } \quad \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial x} == \frac{\partial}{\partial x} \left(\frac{\partial z}{\partial x}\right), \quad \text{and }\quad \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial y}  =\space \frac{\partial}{\partial x} \left(\frac{\partial z}{\partial y}\right) $$
##### Why $\LARGE \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial x}$ and $\LARGE \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial y}$ Appears
This term appears because you are applying the chain rule to the partial derivative $\LARGE \frac{\partial z}{\partial y}$ with respect to another variable $s$.
	The chain rule in multivariable calculus tells us that when we take the derivative of a function that depends on multiple variables, we must account for how each of those variables changes.
		The term $\LARGE \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial y}​$​ in the second-order derivative is analogous to the term $\LARGE \frac{\partial z}{\partial y}​$ in the first-order chain rule, which itself represents how $z$ changes with respect to $x$. 
			The term $\LARGE \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial y}​$ represents how $\LARGE \frac{\partial z}{\partial y}$​ changes with respect to $x$ as $s$ changes.

$$\LARGE \text{Substitute known Partials: } \quad \textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial y} \right)} = \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial x} \cdot \textcolor{violet}{2} + \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial y} \cdot \textcolor{lightgreen}{3}$$
$$\LARGE \text{Where: } \quad \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial x} == \frac{\partial}{\partial x} (\frac{\partial z}{\partial y}) = \frac{\partial^2 z}{\partial y \partial x} $$
$$\LARGE \text{And Where: } \quad \frac{\partial \left( \frac{\partial z}{\partial y} \right)}{\partial y} == \frac{\partial}{\partial y} (\frac{\partial z}{\partial y}) = \frac{\partial^2 z}{\partial y^2} $$
$$\LARGE \text{Simplify: } \quad \textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial y} \right)} = \frac{\partial ^2 z}{\partial y \partial x} \cdot \textcolor{violet}{2} + \frac{\partial^2 z}{\partial y^2} \cdot \textcolor{lightgreen}{3}$$
$$\LARGE \textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial y} \right)}= \textcolor{violet}{2} \frac{\partial ^2 z}{\partial y \partial x} +  \textcolor{lightgreen}{3}\frac{\partial^2 z}{\partial y^2}$$
$$\LARGE \text{Therefore, } \quad \textcolor{lightgreen}{3}\textcolor{yellow}{\frac{\partial}{\partial s} \left( \frac{\partial z}{\partial y} \right)}= \textcolor{lightgreen}{3}\left(\textcolor{violet}{2} \frac{\partial ^2 z}{\partial y \partial x} +  \textcolor{lightgreen}{3}\frac{\partial^2 z}{\partial y^2}\right)$$
###### C. Substitute These Expressions into the Equation for $\LARGE \frac{\partial^2 z}{\partial s^2}$ 

![[Pasted image 20240827065943.png]]
If the Second Order Partial Derivatives of the $f$ are Continuous, then can use the Schwartz Theorem.
	Which means like terms can be combined.
![[Pasted image 20240827070202.png]]
$$\LARGE \text{The Second Order Derivative } \quad \frac{\partial^2 z}{\partial s^2} = 4\frac{\partial^z}{\partial x^2} + 12\frac{\partial^2 z}{\partial x \partial y} + 9\frac{\partial^2 z}{\partial y^2}$$
###### C. Obtain the [[#Second Order Partial Derivatives|Second Order Partial Derivatives]] of $x,y$ with Respect to $t$
$$\large \text{The First Order Derivative wrt t of the Composite Function is: }$$
$$\LARGE \textcolor{teal}{\frac{\partial z}{\partial t}} = \frac{\partial z}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial t}} + \frac{\partial z}{\partial y} \cdot \textcolor{lightgreen}{\frac{\partial y}{\partial t}} = \textcolor{violet}{3}\frac{\partial z}{\partial x} + \textcolor{lightgreen}{-2} \frac{\partial z}{\partial y}$$
$$\large \frac{\partial^2 z}{\partial t^2} =  \frac{\partial}{\partial s}\left( \textcolor{teal}{\frac{\partial z}{\partial t}}\right), \space \text{Second Order Partial Derivative of } \textcolor{teal}{\frac{\partial z}{\partial t}} = \textcolor{violet}{3} \frac{\partial z}{\partial x} \textcolor{lightgreen}{- 2} \frac{\partial z}{\partial y}$$
![[Pasted image 20240827130350.png|400]]
To differentiate $\LARGE \frac{\partial z}{\partial x}$​ and $\LARGE \frac{\partial z}{\partial y}$​ with respect to $t$, we need to apply the chain rule again:
$$\LARGE \text{Differentiating $\LARGE \frac{\partial z}{\partial x}$​ with respect to $t$: }$$
$$\LARGE {\frac{\partial}{\partial t} }\left( \frac{\partial z}{\partial x} \right) = \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x} \cdot \textcolor{violet}{\frac{\partial x}{\partial t}} + \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial y} \cdot \textcolor{lightgreen}{\frac{\partial y}{\partial t}}$$
$$\LARGE \text{Substitute known Partials: } \quad \frac{\partial}{\partial t} \left( \frac{\partial z}{\partial x} \right) = \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x} \cdot \textcolor{violet}{3} + \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial y} \cdot \textcolor{lightgreen}{-2}$$
$$\LARGE \text{Simplifying: } \quad \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial x} == \frac{\partial}{\partial x} (\frac{\partial z}{\partial x}) = \frac{\partial^2 z}{\partial x} $$
$$\LARGE \text{And Simplifing: } \quad \frac{\partial \left( \frac{\partial z}{\partial x} \right)}{\partial y} == \frac{\partial}{\partial y} (\frac{\partial z}{\partial x}) = \frac{\partial^2 z}{\partial x \partial y} $$

$$\LARGE \text{Simplify: } \quad \frac{\partial}{\partial t} \left( \frac{\partial z}{\partial x} \right) = \frac{\partial ^2 z}{\partial x^2} \cdot \textcolor{violet}{3} + \frac{\partial^2 z}{\partial x \partial y} \cdot \textcolor{lightgreen}{-2}$$
## Matrix Transformations Derived from Variant 4
The matrix transformation equation involving transformations between different $\LARGE \mathbb{R}^n$ spaces is essentially a generalization of this concept of Variant 4.
	In multivariable calculus, when you perform a change of variables, the derivative of the composed function is given by the product of the gradients (or derivatives) and the Jacobian matrices, as shown in Variant 4.

This idea generalizes to transformations between any two vector spaces $\LARGE \mathbb{R}^n$ and $\LARGE \mathbb{R}^m$, where:
- The **Jacobian matrix** describes the transformation of the space.
	That is, $\LARGE \text{Matrix } A$

- The **gradient vector** describes the rate of change of the function in the original space.
	That is, $\LARGE \nabla f$ is analogous to the **vector** $\LARGE \mathbf{x}$ being transformed by the matrix $A$.
		$\LARGE \nabla f$ is also a vector, but instead of being a point in space, it represents the directional rates of change of the function.

- The resulting matrix multiplication gives the derivative of the composite function, taking into account both the function's behavior and the transformation of the space.

In the context of **Variant 4** and matrix transformations, the transformation $T_A(x, y, z) = A \cdot \mathbf{x} + \dots$ refers to a linear transformation that maps a vector $\mathbf{x} = (x, y, z)$ in $\mathbb{R}^3$ to another vector in $\mathbb{R}^3$ (or possibly a different space) using a matrix $A$.
#### Relation to Variant 4 and Chain Rule
In **Variant 4**, when you compute derivatives of a function after applying a transformation (like a change of variables), you're essentially dealing with a more generalized version of this matrix transformation. 
	The **Jacobian matrix** in **Variant 4** acts like the transformation matrix $A$, where it transforms small changes in the input coordinates into changes in the output coordinates. 
		The gradient of the function, when multiplied by the Jacobian, gives the derivative in the new coordinate system.

The matrix $A$ in this context is analogous to the Jacobian matrix $D\Phi$ in **Variant 4**, which describes how the coordinates $(x, y, z)$ change with respect to the new variables $(s, t, u)$ (for a 3D example).

#### Formal Definition
Given a matrix $A \in \mathbb{R}^{m \times n}$ and a vector $\mathbf{x} \in \mathbb{R}^n$, the matrix transformation $T_A$ is defined as:
$$\LARGE
T_A(\mathbf{x}) = A \cdot \mathbf{x},
$$
	where $A$ is an $m \times n$ matrix and $\mathbf{x}$ is an $n \times 1$ column vector.
		 The result of this matrix multiplication is a new vector $T_A(\mathbf{x})$ in $\mathbb{R}^m$.
##### Example in $\mathbb{R}^3$
Suppose $A$ is a $3 \times 3$ matrix and $\mathbf{x} = \begin{pmatrix} x \\ y \\ z \end{pmatrix}$ is a vector in $\mathbb{R}^3$. The linear transformation $T_A$ is then given by:
$$\LARGE 
T_A(x, y, z) = A \cdot \begin{pmatrix} x \\ y \\ z \end{pmatrix}.
$$
If $A$ is the matrix:
$$\LARGE
A = \begin{pmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{pmatrix},
$$
then the transformation is:
$$\LARGE 
T_A(x, y, z) = \begin{pmatrix} a_{11}x + a_{12}y + a_{13}z \\ a_{21}x + a_{22}y + a_{23}z \\ a_{31}x + a_{32}y + a_{33}z \end{pmatrix}.
$$
##### Geometric Interpretation
- **Linear Transformation:** The matrix transformation $T_A(\mathbf{x})$ represents a linear transformation that can scale, rotate, reflect, or shear the vector $\mathbf{x}$. The specific operation depends on the entries of the matrix $A$.
- **Mapping Between Spaces:** If $A$ is a $3 \times 3$ matrix, it maps vectors from $\mathbb{R}^3$ to $\mathbb{R}^3$. However, if $A$ is an $m \times n$ matrix, it maps vectors from $\mathbb{R}^n$ to $\mathbb{R}^m$.
##### Example of a Matrix Transformation
Consider the following matrix $A$:
$$\LARGE
A = \begin{pmatrix} 2 & 0 & 0 \\ 0 & 3 & 0 \\ 0 & 0 & 4 \end{pmatrix}.
$$
For a vector $\mathbf{x} = \begin{pmatrix} x \\ y \\ z \end{pmatrix}$, the transformation $T_A$ would be:
$$\LARGE
T_A(x, y, z) = \begin{pmatrix} 2x \\ 3y \\ 4z \end{pmatrix}.
$$
This transformation scales the $x$, $y$, and $z$ components of the vector by factors of 2, 3, and 4, respectively. This is an example of a diagonal matrix that performs axis-aligned scaling.
