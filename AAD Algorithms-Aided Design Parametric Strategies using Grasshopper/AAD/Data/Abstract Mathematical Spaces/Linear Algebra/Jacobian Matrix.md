# Jacobian Matrix
It is a matrix of all first-order partial derivatives of a vector-valued function. 
	It generalizes the concept of the derivative to functions that map from $\LARGE\mathbb{R}^n$ to $\LARGE \mathbb{R}^m$. 
		The Jacobian matrix describes how a function transforms small changes in input variables into changes in output variables, essentially providing the best linear approximation to the function at a given point.
			In the context of [[Mapping#A Transformation as a Subset of Multi-Variable Composite Functions Composite Functions ($1 1$, $m 1$)|transformations]] and chain rules, it acts as the bridge between different coordinate systems, enabling the calculation of derivatives in transformed coordinates.

*Remember, a [[Gradients|Gradient]] is a vector of the all first order partial derivatives of a Scalar Function.*

The multi-variable (i.e. several-variable) counterpart of the first [[Derivatives|derivative]], generally.
	This is, it is the [[Multi-Variable Composite Functions|derivative of a composite function that takes multiple variables]].
		For [[Mapping#Higher-Level Functions (i.e. Composite Functions) Higher-Level Functions|Vector-Valued Functions]] due to the [[Abstract Mathematical Spaces#Vector Spaces and $ mathbb{R} n$|multi-variable nature]].
			Can Linearize Non-Linear Functions.
				But can also be utilized for linear functions.
					The Jacobian matrix for a function $\LARGE\Phi: \mathbb{R}^n \to \mathbb{R}^m$ is an  $\LARGE m\times n$ matrix.
$$\LARGE \vec{y} = \vec{f}(\vec{x}) : \mathbb{R}^n \to \mathbb{R}^m$$
$$\text{Alternative Notation:  } \space \mathbf{y} = \mathbf{f}(\mathbf{x})$$
This is a [[Mapping#An Example of a Vector Function that is composed of Scalar Functions (Linear)|Vector-Valued Function]] composed of the [[Mapping#Fundamental Functions (i.e. Base-Level Functions) Lower-Level Functions|component functions]], $\LARGE f_1, \dots f_m, \space \mathbb{R}^n \to \mathbb{R}$ i.e.
$$\LARGE \begin{Bmatrix} y_1 = f_1(x_1, \dots, x_n) \\ y_2 = f_2(x_1, \dots, x_n) \\ \vdots  \\ y_m = f_m(x_1, \dots, x_n)\end{Bmatrix}$$
$$\LARGE \text{Jacobian Matrix } = m \times n \space \text{matrix} \space=  D\vec{f}(\vec{x}) = \begin{pmatrix} \frac{\partial f_1}{\partial x_1} \space \dots \space \frac{\partial f_1}{\partial x_n} \\ \frac{\partial f_2}{\partial x_1} \space \dots \space \frac{\partial f_2}{\partial x_n}\\ \vdots \quad \ddots \quad \vdots \\ \frac{\partial fm}{\partial x_1} \space \dots \space \frac{\partial f_m}{\partial x_n} \end{pmatrix}$$
Every row $\LARGE j$ of the Jacobian Matrix is the [[Gradients|Gradient]] $\LARGE \nabla f_j(\vec{x})$ of one component function ($\LARGE f_i$).
$$\LARGE \text{Alternative Notation:  } \space \mathbf{J}_\mathbf{f}(\mathbf{x})$$
### Example of Jacobian Matrix: As a Linear Map $T_A : \mathbb{R}^3 \to \mathbb{R}^4$
Remember that the [[Derivatives#Derivative of a Linear Term, ($ LARGE ax$)|Derivative of a Linear Function is a Constant]]. 
$$\LARGE \text{i.e. } \space f(x)=ax == \text{A Linear Term}$$
###### An Example of a Vector Function that is composed of Scalar Functions (Linear functions in this case)
Where **each $f_i$ is a lower-level component function** composing the higher-level function, and subsequently each $f_i$ represents a coordinate of $\mathbb{R}^4$
$$\LARGE T_A: \mathbb{R}^3 \to \mathbb{R}^4$$
$$\LARGE T_A(\vec{u})= T_A(x,y,z) = (\textcolor{magenta}{3x-5y+z}, \textcolor{red}{4x+6y+7z}, \textcolor{orange}{3x-z},\textcolor{green}{8y-9z})$$
$$\LARGE f_i: \mathbb{R}^3 \to \mathbb{R}$$
$$\LARGE \textcolor{magenta}{f_1(x,y,z) = 3x-5y+z}$$
$$\LARGE \textcolor{red}{f_2(x,y,z) = 4x+6y+7z}$$
$$\LARGE \textcolor{orange}{f_3(x,y,z) = 3x-z}$$
$$\LARGE \textcolor{green}{f_4(x,y,z) = 8y-9z}$$
$$\LARGE A = \begin{bmatrix} \textcolor{magenta}{3 \quad -5 \quad 1} \\ \textcolor{red}{4 \quad 6 \quad 7} \\ \textcolor{orange}{3 \quad 0 \quad -1} \\ \textcolor{green}{0 \quad 8 \quad -9}\end{bmatrix} =  \begin{bmatrix} \textcolor{magenta}{\frac{\partial f_1}{\partial x} \quad \frac{\partial f_1}{\partial y} \quad \frac{\partial f_1}{\partial z}} \\ \textcolor{red}{\frac{\partial f_2}{\partial x} \quad \frac{\partial f_2}{\partial y} \quad \frac{\partial f_2}{\partial z}} \\ \textcolor{orange}{\frac{\partial f_3}{\partial x} \quad \frac{\partial f_3}{\partial y} \quad \frac{\partial f_3}{\partial z}} \\ \textcolor{green}{\frac{\partial f_4}{\partial x} \quad \frac{\partial f_4}{\partial y} \quad \frac{\partial f_4}{\partial z}} \end{bmatrix} = DT_A(\vec{x}) = \mathbf{J}_{T_A}(\mathbf{x})$$
	Where $\LARGE A$ is the Jacobian Matrix. 
### Example of Jacobian Matrix: As a Non-Linear Function $\mathbf{f}: \mathbb{R}^3 \to \mathbb{R}^2$
###### An Example of a Vector Function that is composed of Scalar Functions (Non-Linear function in this case)
Where **each $f_i$ is a lower-level component function** composing the higher-level function, and subsequently each $f_i$ represents a coordinate of $\mathbb{R}^4$
$$\LARGE \vec{f}: \mathbb{R}^3 \to \mathbb{R}^2$$
$$\LARGE \vec{f}(x,y,z) = (\textcolor{magenta}{x^2+yz}, \textcolor{red}{y^2-x \ln z})$$
$$\LARGE f_i: \mathbb{R}^3 \to \mathbb{R}$$
$$\LARGE \textcolor{magenta}{f_1(x,y,z) = x^2+yz}$$
$$\LARGE \textcolor{red}{f_2(x,y,z) = y^2-x \ln z}$$
$$\LARGE  = D\vec{f}(\vec{x}) = \mathbf{J}_{T_A}(\mathbf{x}) =\begin{bmatrix} \textcolor{magenta}{\frac{\partial f_1}{\partial x} \quad \frac{\partial f_1}{\partial y} \quad \frac{\partial f_1}{\partial z}} \\ \textcolor{red}{\frac{\partial f_2}{\partial x} \quad \frac{\partial f_2}{\partial y} \quad \frac{\partial f_2}{\partial z}} \end{bmatrix} =  \begin{bmatrix} \textcolor{magenta}{2x \quad z \quad y} \\ \textcolor{red}{-\ln z \quad 2y \quad -\frac{x}{z}} \end{bmatrix}$$
### Example of Jacobian Matrix: As a Function $\mathbf{f}: \mathbb{R}^2 \to \mathbb{R}^2$: a Change of Variables

![[Pasted image 20240819065629.png]]