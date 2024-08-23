# Chain Rule
Of Multi-Variable Functions
## [[Mapping#A Composite Function as a Subset of Functions|Composite Functions]]
$$\LARGE f \circ g \circ h: \mathbb{R} \xrightarrow{h}\mathbb{R} \xrightarrow{g}  \mathbb{R} \xrightarrow{f} \mathbb{R}$$
$$\LARGE \frac{d}{dx}f(g(h(x))) = \frac{d}{dg(h(x))}f(g(h(x))) \cdot \frac{d}{dh(x)}g(h(x)) \cdot \frac{d}{dx}h(x)$$
$$\LARGE ==  f'(g(h(x)) \cdot g'(h(x)) \cdot h'(x)$$
## [[Derivatives#Chain Rule Chain Rule of Single Variable Functions|Chain Rule of Single Variable Functions]]
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
## Notation of the Four Variants of the Chain Rule
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
## Variant 0
The one-dimensional Chain Rule for 
$$\LARGE f \circ g : \mathbb{R} \xrightarrow{g}\mathbb{R} \xrightarrow{f}  \mathbb{R}$$
$$\LARGE \frac{d}{dx}f(g(x)) =  f'(g(x)) \cdot g'(x)$$
$$\LARGE \text{With the notation } u = f(v),\space v = g(x)$$
$$\LARGE \text{We can write } \frac{du}{dx} = \frac{du}{dv} \cdot \frac{dv}{dx}, \quad u:\mathbb{R} \to \mathbb{R}$$
## Variant 1
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
## Variant 2
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
## Variant 3
The most frequently used variant in our case.
	It is essentially the [[Dot Product|dot product]] (because of the two vectors in the equation) of the gradient (i.e. the vector composed of partial derivatives) of the outer function by the derivative of the [[#$ LARGE vec{v}$ A Mapping Higher-Level Functions (i.e. Composite Functions) Higher-Level Functions Vector-Valued function (i.e. a Vector Function) of $ LARGE text{ textcolor{lightblue}{one real variable}}$.|single variable vector function]].
		$\LARGE f(x,y)$ is a [[#$ LARGE f$ A Mapping Scalar Functions as a Subset of Functions Real-Valued function (i.e. a Scalar Function) of $ LARGE text{ textcolor{pink}{several real variables}}$.]].
		$\LARGE \vec{v}(t) = [x(t), y(t), z(t)]$ is a [[#$ LARGE vec{v}$ A Mapping Higher-Level Functions (i.e. Composite Functions) Higher-Level Functions Vector-Valued function (i.e. a Vector Function) of $ LARGE text{ textcolor{lightblue}{one real variable}}$.|Single Variable Vector Function]].
		$\LARGE \nabla f(x,y)$ is a [[#$ LARGE nabla f$ A Vector function of $ LARGE text{ textcolor{pink}{several real variables}}$.|Multi-Variable Vector Function]].
$$\LARGE f \circ \vec{v} : \mathbb{R} \xrightarrow{\vec{v}} \mathbb{R}^2 \xrightarrow{f} \mathbb{R}$$
$$\LARGE \frac{d}{dt} [f(\vec{v}(t))] = \nabla f(\vec{v}(t)) \cdot \vec{v}'(t) $$
$$\LARGE \nabla f(\vec{v}(t)) \cdot \vec{v}'(t) = (\frac{\partial f}{\partial x} \cdot x'(t)) + (\frac{\partial f}{\partial y} \cdot y'(t)) + (\frac{\partial f}{\partial z} \cdot z'(t))$$
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
$$\LARGE \frac{d}{dt}f(\vec{v}(t)) = f'_1(\vec{v}(t))x'(t) + f'_2(\vec{v}(t)y'(t)  + f'_3(\vec{v}(t))z'(t) $$
$$\LARGE \text{Where } f'_1(x,y,z) = \frac{\partial f}{\partial x}xz+\cos y  = z, \quad (\vec{v}(t))_z = \ln(t^2+1)$$
$$\LARGE f'_2(x,y,z) = \frac{\partial f}{\partial y}xz+\cos y = -\sin y, \quad (\vec{v}(t))_y = t^2$$
$$\LARGE f'_3(x,y,z) = \frac{\partial f}{\partial z}xz+\cos y = x, \quad (\vec{v}(t))_x = \sin t $$
$$\LARGE \text{And }$$
$$\LARGE \text{Where } (\vec{v}'(t))_x = \frac{d}{dt}\sin t = \cos t$$
$$\LARGE  (\vec{v}'(t))_y = \frac{d}{dt}t^2 = 2t$$
$$\LARGE  (\vec{v}'(t))_z = \frac{d}{dt}\ln(t^2+1) = \sin t \cdot \frac{2t}{1+t^2}$$
