# Partial Derivatives
##### *Note: a Derivative (and Partial Derivative) **is** a vector.*
*That vector being the [[Derivatives#4. Is the Unit Tangent Vector|Unit Tangent Vector]] to a given point.*
	*Therefore the Vector of the Partial Derivatives is a Unit Tangent Vector describing the direction of the function in a single dimension.*
		*But the **Gradient vector** describes the direction and rate of the steepest increase in a multi-dimensional space.*

##### *Note: Role of Scalar Fields in Learning Derivatives*
*Understanding derivatives in the context of scalar fields is crucial for analyzing how these quantities change in space.* 

- - -
## The Differential Equations of Partial Derivatives
##### 2D
$$\LARGE df = \Delta z= \frac{\partial f}{\partial x}dx + \frac{\partial f}{\partial y}dy$$
##### 3D
$$\LARGE df = \frac{\partial f}{\partial x}dx + \frac{\partial f}{\partial y}dy + \frac{\partial f}{\partial z}dz$$
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
## For a ([[Components of Motion#2D Components of the Velocity Vector|2D]]) Function $f(x, y)$ aka a Surface
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
##### Function, $\LARGE f(x,y)$
![[Pasted image 20240623221622.png|300]]
##### Differential of $f(x,y)$, $\LARGE \frac{\partial}{\partial x}f(x,y)$
![[Pasted image 20240705151637.png|400]]
When we first approach this very, very steep slope here where this derivative has a large peak.
	Then when you approach the top, this slope gets less steep.
		Then at the plateau, the slope is zero.
			This is why you get here a very large flat region in between the convex and concave regions, where the derivative is basically zero.
##### Function, $\LARGE f(x,y)$
![[Pasted image 20240623222925.png|300]]
##### Differential of $f(x,y)$, $\LARGE \frac{\partial}{\partial y}f(x,y)$
![[Pasted image 20240705151727.png|400]]
When we first approach this very, very steep slope here where this derivative has a large peak.
	Then when you approach the top, this slope gets less steep.
		Then at the plateau, the slope is zero.
			This is why you get here a very large flat region in between the convex and concave regions, where the derivative is basically zero.
- - -
### 2D Partial Derivative of $f$ with Respect to $x$
Simply compute single variable derivative of one variable while keeping the other variable(s) as constant.  
$$\frac{\partial f}{\partial x} = \partial_x f(a,b) = {\partial \over \partial x}f(a,b) = f'_{x}(a,b) = f'_{1}(a,b) = \lim_{h \rightarrow 0} {f(a+h,b) - f(a,b) \over h} = g'(a)$$
$$g(x) = f(x, b)$$
*Remember: The [[Limits#Limit at a Specific Point|Limit]] in the following form represents the rate of change at a specific point, $a$.*

The partial derivative is simply a single variable calculus function, enabled by holding one variable constant. 
	Because $y$ is a constant $b$, this function no longer represents a 3D surface, but a 2D Curve.
$$\text{Where } g=(x) \text{ represents the equivalent single variable function from single variable calculus.}$$
$$g(x) \text{ is defined by a function } f(x,b) \text{ that has a constant variable } b.$$
### $y=b$ Represents a Plane
And thus a domain for $g(x) = f(x,b)$.
	Parallel to the $xz$-plane.
### $z=f(x,y)$ Represents a 3D Surface
Where points within a $xy$-plane are mapped to a $z$ value and thus an additional dimension.
### $z_{curve} = g(x)$ Represents a 2D Vertical [[#Cross-Section Curves|Cross-Section Curve]] Within a Single Plane on the 3D Surface
Because the the $y$ variable is constant, the function becomes that of a 2D curve is within the plane/domain defined by the constant $y$, and thus parallel to the $xz$-plane.
	That is, variable $x$ within are mapped to unique $z_{curve}$ values. 
		$g(x)$ is equivalent to $f(x,b)$ where $b$ is constant.

- - -
### 2D Partial Derivative of $f$ with Respect to $y$
Simply compute single variable derivative of one variable while keeping the other variable(s) as constant.  
$$\frac{\partial f}{\partial y} = \partial_y f(a,b) = {\partial \over \partial y}f(a,b) = f'_{y}(a,b) = f'_{2}(a,b) = \lim_{k \rightarrow 0} {f(a,b+h) - f(a,b) \over k} = h'(b)$$
$$h(y) = f(a, y)$$
*Remember: The [[Limits#Limit at a Specific Point|Limit]] in the following form represents the rate of change at a specific point, $a$.*

The partial derivative is simply a single variable calculus function, enabled by holding one variable constant. 
	Because $y$ is a constant $b$, this function no longer represents a 3D surface, but a 2D Curve.
$$\text{Where } h=(y) \text{ represents the equivalent single variable function from single variable calculus.}$$
$$h(y) \text{ is defined by a function } f(a,y) \text{ that has a constant variable } a.$$
### $a=x$ Represents a Plane
And thus a domain for $h(y) = f(a,y)$.
	Parallel to the $zy$-plane.
### $z=f(x,y)$ Represents a 3D Surface
Where points within a $xy$-plane are mapped to a $z$ value and thus an additional dimension.
### $z_{curve} = h(y)$ Represents a 2D Vertical [[#Cross-Section Curves|Cross-Section Curve]] Along a Single Plane Within the 3D Surface
Because the the $x$ variable is constant, the function becomes that of a 2D curve is within the plane defined by the constant $y$, and thus parallel to the $zy$-plane.
	That is, variable $y$ within are mapped to unique $z_{curve}$ values. 
		$h(y)$ is equivalent to $f(a,y)$ where $a$ is constant.

Vertical Cross-Sections Parallel to the $yz$-Plane
	These are obtained by holding $x$ constant (say, $x=a$) and varying $y$ and $z$: $z = f(a, y)$ This gives a curve in the $yz$-plane.

- - -
## Tangent Vector of 2D Curve

$$\LARGE \text{3D Surface } z=f(x,y)$$
The Domain of $f(x,y)$ exists (*blue plane*) as a Subset of the $xy$-plane.
![[Pasted image 20240727064407.png|500]]

Some point in the $xy$-plane and its position on the surface (i.e. in the function $f(x,y)$).
![[Pasted image 20240727064901.png|500]]
### Cross-Section Curves
Notice the **Cross-Section curves** (*green and red*).
Cross-section curves are obtained by slicing the surface with vertical planes. 
	Cross-Section Curves represents how the surface behaves along the line where $y$ is fixed at $b$ and $x$ varies (or as $x$ is fixed at $a$ and $y$ varies).
		It essentially provides a "slice" of the surface at that particular $x$-value or $y$-value, allowing for the study of the behavior of that surface along that "slice" (i.e. plane).
			These curves are generated by holding one of the variables constant and allowing the other variable to vary. 
				There are two primary types of cross-section curves:
					a. Vertical Cross-Sections Parallel to the $yz$-Plane
						These are obtained by holding $x$ constant (say, $x=a$) and varying $y$ and $z$: $z = f(a, y)$ This gives a curve in the $yz$-plane.
					b. Vertical Cross-Sections Parallel to the $xz$-Plane
						These are obtained by holding $y$ constant (say, $y = b$) and varying $x$ and $z$: $z = f(x, b)$ This gives a curve in the $xz$-plane.

To produce the *red* curve, take the plane $y=b$ that is **parallel** to the $xz$-plane. 
Where $y$ variable is held constant, as in the [[#2D Partial Derivative of $f$ with Respect to $x$|partial derivative with respect to x.]] 
$$\text{Point } (a, b, f(a,b)) \text{ ; } \text{Surface } z= f(x,y) \text{ ; } \text{Plane }y=b\text{ ; } \text{Curve }z=f(x,b) = g(x))$$
The plane as a constant $y$ value (being $b$ in this case), 
	Therefore, any point on this plane has the second coordinate always equal to b.
		The $x$ variable is free to vary within the bounds/domain (i.e. the initial blue plane) set by the curve (i.e. $z= f(x,y)$).
			This plane intersects the surface in this *red* curve.
				This curve ($z=f(x,y)$) represents the single variable calculus function $g(x) = f(x, b)$, which itself is the function from which the partial derivative with respect to $x$ is derived from. 
![[Pasted image 20240727065106.png|500]]

The *green* curve is produced via the plane, $x=a$ 
Where $x$ variable is held constant, as in the [[#2D Partial Derivative of $f$ with Respect to $y$|partial derivative with respect to y]] 
$$ \text{Point } (a, b, f(a,b)) \text{ ; }\text{Surface } z = f(x, y) \text{ ; } \text{Plane }x=a\text{ ; } \text{Curve }z=f(a,y) = h(y)$$
The plane as a constant $x$ value (being $a$ in this case), 
	Therefore, any point on this plane has the second coordinate always equal to b.
		The $y$ variable is free to vary within the bounds/domain (i.e. the initial blue plane) set by the curve (i.e. $z= f(x,y)$).
			This plane intersects the surface in this *green* curve.
				This curve ($z=f(x,y)$) represents the single variable calculus function $h(y) = f(a, y)$, which itself is the function from which the partial derivative with respect to $y$ is derived from. 
![[Pasted image 20240727070252.png|500]]
### Tangent Line of $g(x)$
The Tangent Line to the *red* curve, $g(x)$ lies **within** the same plane, $y=b$.
	The **Slope** of this Tangent Line is the [[#2D Partial Derivative of $f$ with Respect to $x$|Derivative]] of $g(a)$ at a given point, $(a, b, f(a, b))$.
		Remember, it is the Derivative of $g(a)$ because the variable b is held constant.
			Thus, it is the **Partial Derivative** of the function $f(a, b)$ with respect to $a$, making $b$ a constant.  

Therefore the [[Derivatives#3. The Differential Ratio *is* the Limit *of* the Slope of the Tangent Line The Limit of the Slope of the Secant Line and the Slope of the Tangent Line|Slope of the Tangent Line]] is equal to the Derivative.
### [[#Tangent Vector Components|Tangent Vector]] in Terms of Partial Derivatives 
The tangent vector to the surface $z = f(x, y)$ at a point $(a, b)$ can be expressed using the partial derivatives of $f$.
	If you move by small amounts $\Delta x$ and $\Delta y$ from the point $(a, b)$, the change in $z$, denoted as $\Delta z$, can be approximated using the partial derivatives:
$$\LARGE \Delta z \approx \frac{\partial f}{\partial x}(a, b) \Delta x + \frac{\partial f}{\partial y}(a, b) \Delta y$$
  The corresponding tangent vector $\mathbf{T}(\Delta x, \Delta y)$ at the point $(a, b, f(a, b))$ is a [[Mapping#Higher-Level Functions (i.e. Composite Functions) Higher-Level Functions|Vector Function]]
$$\LARGE \mathbf{T}(\Delta x, \Delta y) = \begin{pmatrix} \Delta x \\ \Delta y \\ \Delta z \end{pmatrix} = \begin{pmatrix} \Delta x \\ \Delta y \\ \frac{\partial f}{\partial x}(a, b) \Delta x + \frac{\partial f}{\partial y}(a, b) \Delta y \end{pmatrix}$$
### Direction Vector in the Plane $y = b$ 
The **direction vector** is a specific instance of the [[#Tangent Vector Components]] when considering a particular direction in a plane (e.g., the plane $y = b$).
	It is formally called the Direction Vector *of* the Tangent Line.

If you are considering the direction vector in the plane $y = b$, then $\Delta y = 0$.
	In this case, the tangent vector simplifies to:
$$\LARGE \mathbf{T}(\Delta x, 0) = \begin{pmatrix} \Delta x \\ 0 \\ \frac{\partial f}{\partial x}(a, b) \Delta x \end{pmatrix}$$
This can be further simplified to:
$$\LARGE \mathbf{T}(\Delta x, 0) = \Delta x \begin{pmatrix} 1 \\ 0 \\ \frac{\partial f}{\partial x}(a, b) \end{pmatrix}$$
Here, the vector $\begin{pmatrix} 1 \\ 0 \\ \frac{\partial f}{\partial y}(a, b) \end{pmatrix}$ is the direction vector in the plane $x = a$.
To produce this tangent line in [[Abstract Mathematical Spaces#$ mathbb{R} 3$ - Three-Dimensional Vector Space|R^3]] space, we use a direction vector.
	Instead of using the Slope of the Tangent Line, utilize the Direction Vector.
		Because this Vector is completely included in the plane, $y=b$, this means the Vector has no $y$ component, and thus $0$ for the $y$ component. 
$$\LARGE \text{Direction Vector } = \begin{pmatrix} 1 \\ 0 \\ f'_{x}(a,b) \end{pmatrix} = \begin{pmatrix} 1 \\ 0 \\ \frac{\partial f}{\partial x}(a,b) \end{pmatrix}$$
$$\Large \text{Where } f'_{x}(a,b) = \frac{\partial f}{\partial x}(a,b) = g'(a)$$
##### Coordinates of the Tangent Direction Vector of the Tangent Line of $g(x)$
Therefore the [[Derivatives#3. The Differential Ratio *is* the Limit *of* the Slope of the Tangent Line The Limit of the Slope of the Secant Line and the Slope of the Tangent Line|Slope of the Tangent Line]] is equal to the Derivative.
$$\LARGE \text{For a given point } (a, b, f(a,b)): \space \frac{\Delta z}{\Delta x} = g'(a)$$
Therefore, for the sake of easy computation, just make $\LARGE \Delta x = 1$. 
$$\LARGE \Delta z = g'(a) \cdot \Delta x$$
$$\LARGE \Delta z = g'(a) \cdot 1$$
$$\large \text{The coordinates of the Direction Vector of the Tangent Line (i.e. Tangent Vector):}$$
$$\LARGE = \vec{v} = \left[ 1, 0, g'(a) \right] = \left[ 1, 0, \frac{\partial f}{\partial x}(a,b) \right]$$
![[Pasted image 20240727081213.png]]
![[Pasted image 20240809054135.png]]
### Tangent Line of $h(y)$
The Tangent Line to the *green* curve, $h(y)$ lies **within** the same plane, $x=a$.
	The **Slope** of this Tangent Line is the [[#2D Partial Derivative of $f$ with Respect to $x$|Derivative]] of $h(b)$ at a given point, $(a, b, f(a, b))$.
		Remember, it is the Derivative of $h(b)$ because the variable $a$ is held constant.
			Thus, it is the **Partial Derivative** of the function $f(a, b)$ with respect to $b$, making $a$ a constant.  
### Direction Vector in the Plane $x = a$ 
The **direction vector** is a specific instance of the [[#Tangent Vector Components]] when considering a particular direction in a plane (e.g., the plane $x = a$).
	It is formally called the Direction Vector *of* the Tangent Line.

If you are considering the direction vector in the plane $x = a$, then $\Delta x = 0$. In this case, the tangent vector simplifies to:
 $$\LARGE \mathbf{T}(0, \Delta y) = \begin{pmatrix} 0 \\ \Delta y \\ \frac{\partial f}{\partial y}(a, b) \Delta y \end{pmatrix} $$
This can be further simplified to:
 $$\LARGE \mathbf{T}(0, \Delta y) = \Delta y \begin{pmatrix} 0 \\ 1 \\ \frac{\partial f}{\partial y}(a, b) \end{pmatrix}$$
Here, the vector $\begin{pmatrix} 0 \\ 1 \\ \frac{\partial f}{\partial y}(a, b) \end{pmatrix}$ is the direction vector in the plane $x = a$.

To produce this tangent line in [[Abstract Mathematical Spaces#$ mathbb{R} 3$ - Three-Dimensional Vector Space|$\mathbb{R}^3$]] space, we use a direction vector.
	Instead of using the Slope of the Tangent Line, utilize the Direction Vector.
		Because this Vector is completely included in the plane, $x=a$, this means the Vector has no $x$ component, and thus $0$ for the $x$ component. 
$$\LARGE \text{Direction Vector } = \begin{pmatrix} 0 \\ 1 \\ f'_{y}(a,b) \end{pmatrix} = \begin{pmatrix} 0 \\ 1 \\ \frac{\partial f}{\partial y}(a,b) \end{pmatrix}$$
$$\Large \text{Where } f'_{y}(a,b) = \frac{\partial f}{\partial y}(a,b) = h'(b)$$
##### Coordinates of the Tangent Direction Vector of the Tangent Line of $h(y)$
Therefore the [[Derivatives#3. The Differential Ratio *is* the Limit *of* the Slope of the Tangent Line The Limit of the Slope of the Secant Line and the Slope of the Tangent Line|Slope of the Tangent Line]] is equal to the Derivative.
$$\LARGE \text{For a given point } (a, b, f(a,b)): \space \frac{\Delta z}{\Delta x} = h'(b)$$
Therefore, for the sake of easy computation, just make $\LARGE \Delta y = 1$. 
$$\LARGE \Delta z = h'(b) \cdot \Delta y$$
$$\LARGE \Delta z = h'(b) \cdot 1$$
$$\large \text{The coordinates of the Direction Vector of the Tangent Line (i.e. Tangent Vector):}$$
$$\LARGE = \vec{u} = \left[ 0, 1, h'(b) \right] = \left[ 0, 1, \frac{\partial f}{\partial y}(a,b) \right]$$
![[Pasted image 20240727083419.png]]
###### Therefore Each Tangent Vector is Composed of a Single Partial Derivative
- - -
## Tangent Plane of a 3D Surface
Tangent Plane to the Surface $z = f(x,y)$ in the point $(a,b, f(a,b))$.

A plane through the point $(a,b, f(a,b))$.
	Which contains the [[#Tangent Line of $g(x)$|tangent line]] to $z = f(x, b) = g(x)$ in the plane $y = b$, through the point  $(a,b, f(a,b))$.
		Thus the line with the slope of $g'(a)$.
	Which also contains the [[#Tangent Line of $h(y)$|tangent line]] to $z = f(a, y) = h(y)$ in the plane $x = a$, through the point  $(a,b, f(a,b))$.
		Thus the line with the slope of $h'(b)$.
### Need a Normal Vector (to a 3D Surface) First
![[Pasted image 20240728064143.png|400]]
#### Normal Vector to a 3D Surface
The Normal Vector must be orthogonal to the Tangent Plane and thus both [[#Direction Vector in the Plane $y = b$|Directional Vectors]] (Tangent Vectors).
	A Vector that is perpendicular to two given Vectors is the Vector that is the [[Statics Analysis#Cross Product|Cross Product]] of two given Vectors.
		Which requires knowing the **coordinates** of the two Tangent Vectors (i.e. Direction Vectors).
##### Vector $\LARGE \vec{v}$ 
![[Pasted image 20240728064200.png]]
###### Coordinates of the $\LARGE \vec{v}$ of the Tangent Line of $g(x)$
*See above: [[#Coordinates of the $ LARGE vec{v}$ of the Tangent Line of $g(x)$|Coordinates of the Tangent Vector of the Tangent Line of]]* $g(x)$.

It is the Direction Vector of the Tangent Line of the 1D function $\LARGE g(x)$ in the plane $\LARGE y=b$.
	Because this Tangent Line and thus Direction Vector, $\vec{v}$ is limited to the plane $y=b$, there will be no change in the $y$ direction.
		Which means that the $y$ coordinate of the Direction Vector, $\vec{v}$ must be $0$. 
			There will never be a change in the $y$ direction.
				So only the $x$ and $z$ coordinates are needed.
$$\LARGE = \vec{v} = \left[ 1, 0, g'(a) \right] = \left[ 1, 0, \frac{\partial f}{\partial x}(a,b) \right]$$
##### Vector $\LARGE \vec{u}$
![[Pasted image 20240728064208.png]]
###### Coordinates of the $\LARGE \vec{u}$ of the Tangent Line of $h(y)$
*See above: [[#Coordinates of the $ LARGE vec{v}$ of the Tangent Line of $h(y)$|Coordinates of the Tangent Vector of the Tangent Line of]]* $h(y)$.

It is the Direction Vector of the Tangent Line of the 1D function $\LARGE h(y)$ in the plane $\LARGE x=a$.
	Because this Tangent Line and thus Direction Vector, $\vec{u}$ is limited to the plane $x=a$, there will be no change in the $x$ direction.
		Which means that the $x$ coordinate of the Direction Vector, $\vec{u}$ must be $0$. 
			There will never be a change in the $x$ direction.
				So only the $y$ and $z$ coordinates are needed.
$$\LARGE = \vec{u} = \left[ 0, 1, h'(b) \right] = \left[ 0, 1, \frac{\partial f}{\partial y}(a,b) \right]$$
##### Normal Vector as a [[Cross Product|Cross Product]] (Between the two Tangent Vectors of Partial Derivatives)
$$\LARGE \vec{n_{\perp}} =  \vec{v} \times \vec{u}$$
The Normal Vector to a plane is the cross product of the two directional vectors $\vec{v}$ and $\vec{u}$.
$$\LARGE \left| \begin{matrix} \vec{i} \quad \quad \vec{j} \quad \quad \vec{k} \\ 1 \quad 0 \quad f_{x}'(a,b) \\ 0 \quad 1 \quad f'_{y}(a,b)\end{matrix} \right| =   = (-f'_{x}(a,b), -f'_{y}(a,b), 1)$$
$$\LARGE = \text{The Normal Vector } (-\frac{\partial f}{\partial x}(a,b), - \frac{\partial f}{\partial y}(a,b), 1)$$
$$\LARGE \text{To point the point } (a,b, f(a,b))$$
The Normal Vector is thus **composed of two partial derivatives** 
### Back to the Tangent Plane
Once the normal vector to the [[#Cross-Section Curves|cross section curves]], the tangent plane can now be calculated via the Normal Equation.
![[Pasted image 20240810055336.png]]
#### The Normal Equation of the Plane
The Normal Equation of the plane, $\LARGE \pi$ through $\LARGE x_0 = (x_0, y_0, z_0)$ and orthogonal to the vector $\LARGE \mathbf{n} = (a,b,c)$:
$$\LARGE ax + by + cz + d = 0$$
$$\LARGE \text{Where } d = -ax_0 - by_0 - cz_0$$
***If*** a point $\LARGE x = (x,y,z)$ belongs to $\LARGE \pi$, ***then*** the vectors $\LARGE \mathbf{n} = (a,b,c)$ and $\LARGE x - x_0 = (x-x_0, y-y_0, z- z_0)$ must be orthogonal, which means that their dot product must be 0:
$$\LARGE (a,b,c) \cdot (x-x_0 y - y_0, z- z_0) = 0$$
$$\LARGE \text{If and only if} $$
$$\LARGE ax-\textcolor{red}{ax_0}+by-\textcolor{red}{by_0} +cz-\textcolor{red}{cz_0}={0}$$
$$\LARGE \text{If and only if} $$
$$\LARGE ax- +by  +cz + \textcolor{red}{d}= 0$$
##### Computing the Normal Equation
![[Pasted image 20240810060854.png]]
$$\LARGE (x,y,z) \Leftrightarrow (x-a,y-b,z-f(a,b)) \cdot (f'_x(a,b), f'_y(a,b), -1) = 0$$
##### 1. Compute the Directional Vector (i.e. Tangent Vector)
- - -
## Interpreting Partial Derivatives
Recall that the graph of a function of two variables is a surface in $\mathbf{R^3}$.

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
## Deriving the Tangent Vector Components
For a scalar function of multiple variables, the concept of the tangent vector can be extended using partial derivatives. 

For a scalar function with multiple variables, the components of the tangent vector at a point are derived using the small changes in each variable and the corresponding changes in the function's value, approximated by the partial derivatives. 
	The tangent vector provides a direction in the multidimensional space, showing how the function changes with respect to the variables.
### Why These Components?
###### Small Increments:
$\Delta x$, $\Delta y$, and $\Delta z$ are small increments in the variables and the function value. 
	They provide an approximation of how the function changes locally.
###### Partial Derivatives
The partial derivatives $\frac{\partial f}{\partial x}$ and $\frac{\partial f}{\partial y}$ give the rate of change of the function in each direction. 
	When multiplied by the small increments $\Delta x$ and $\Delta y$, they approximate the change in $z$.
###### Directional Changes
The components $\Delta x$, $\Delta y$, and $\Delta z$ describe the change in the function's value as we move in the direction of the tangent vector.
	The vector components are related to how the function changes with respect to the input variables.
### Scalar Function with Two Variables
Consider a scalar function $f(x, y)$.
### Partial Derivatives
The partial derivatives of $f$ with respect to $x$ and $y$ are:
$$
\LARGE \frac{\partial f}{\partial x}, \quad \frac{\partial f}{\partial y}
$$
### Tangent Plane and Tangent Vector
The tangent vector $T(\Delta x, \Delta y)$ visually and mathematically represents the instantaneous rate of change of the function $f$ at a point $x,y$.
	The components of the vector capture the differential changes in the input and output, providing a linear approximation of the function's behavior near that point.

$$\LARGE \text{The derivative, (i.e. the limit of the slope of the secant line) } $$
$$\LARGE \text{is } df = \Delta z = \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y$$
$$\LARGE \text{Which itself is the Slope of the Tangent Vector}$$
$$\LARGE \text{And is a component of the Tangent Vector}$$
At a point $P = (x_0, y_0, f(x_0, y_0))$, the tangent plane to the surface $z = f(x, y)$ can be defined, and we can derive the tangent vector components from this.
### Steps to Derive the Tangent Vector Components
Consider the [[Abstract Mathematical Spaces#Scalar Functions|scalar function]]
1. **Point on the Surface:**
   Consider the point $P = (x_0, y_0, f(x_0, y_0))$ on the surface.

2. **Small Changes in $x$ and $y$:**
   Let $\Delta x$ and $\Delta y$ be small changes in $x$ and $y$, respectively.

3. **Partial Derivatives at the Point:**
	Compute the partial derivatives of the function at the point $(x_0, y_0)$:

$$\LARGE \frac{\partial f}{\partial x} \bigg|_{(x_0, y_0)}, \quad \frac{\partial f}{\partial y} \bigg|_{(x_0, y_0)}$$

4. **Corresponding Change in $z$:**
   The corresponding change in $z$, denoted $\Delta z$, can be approximated using the partial derivatives:
   $$\LARGE df = \Delta z = \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y$$
### Tangent Vector Components
#### [[Abstract Mathematical Spaces#Vector Function|Vector-Valued Functions]]
The tangent vector itself can be seen as a vector-valued function when we express how changes in $x$ and $y$ (or higher dimensions) affect the function $f$.
	The points $\Delta x$, $\Delta y$, and $\Delta z$ are mapped to a vector $\mathbf{T}$, this mapping represents a vector function. 
		Specifically, $\mathbf{T}$ is a vector whose components are functions of the variables $\Delta x$ and $\Delta y$,.

The tangent vector at the point $P$ in the direction of changes $\Delta x$ and $\Delta y$ has components:
- A small change in $x$ is denoted by $\Delta x$.
- A small change in $y$ is denoted by $\Delta y$.
- The corresponding change in $z$ is given by: 
$$\LARGE 
\mathbf{T} = \mathbf{T}(\Delta x, \Delta y) \begin{pmatrix} \Delta x \\ \Delta y \\ \Delta z \end{pmatrix} = \begin{pmatrix} \Delta x \\ \Delta y \\ \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y \end{pmatrix}
$$
$$\text{Compared with the 1D Derivative } \mathbf{T} = \mathbf{T}(\Delta x) \begin{pmatrix} \Delta x \\ \Delta y \end{pmatrix} = \begin{pmatrix} \Delta x \\ f'(x) \Delta x \end{pmatrix}$$
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
### Example

Consider a function $f(x, y) = x^2 + y^2$ and find the tangent vector at $(x_0, y_0) = (1, 1)$:

1. **Function and Partial Derivatives:**
   $$
   f(x, y) = x^2 + y^2
   $$
   $$
   \frac{\partial f}{\partial x} = 2x, \quad \frac{\partial f}{\partial y} = 2y
   $$
2. **Point on the Surface:**
   At $(x_0, y_0) = (1, 1)$, the point on the surface is $P = (1, 1, f(1, 1)) = (1, 1, 2)$.

3. **Small Changes $\Delta x$ and $\Delta y$:**
   Let $\Delta x = 0.1$ and $\Delta y = 0.1$.

4. **Corresponding Change $\Delta z$:**
$$\LARGE \Delta z = \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y$$ 
$$\LARGE = \Delta z = 2 \Delta x + 2 \Delta y$$
$$\LARGE    \Delta z = \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y = 2 \cdot 1 \cdot 0.1 + 2 \cdot 1 \cdot 0.1 = 0.2 + 0.2 = 0.4$$
1. **Tangent Vector Components:**

| Evaluated Vector                                                                                                                             | Vector Function/Field                                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| $$\LARGE \mathbf{T} = \begin{pmatrix} \Delta x \\ \Delta y \\ \Delta z \end{pmatrix} = \begin{pmatrix} 0.1 \\ 0.1 \\ 0.4 \end{pmatrix}$$<br> | $$\LARGE \mathbf{T} = \begin{pmatrix} \Delta x \\ \Delta y \\ \Delta z \end{pmatrix} = \begin{pmatrix} \Delta x \\ \Delta y \\ 2 \Delta x + 2 \Delta y \end{pmatrix}$$<br> |
### Generalization
For a scalar function $\LARGE f(x_1, x_2, \ldots, x_n)$ with multiple variables, the tangent vector components can be derived similarly using the partial derivatives. 
	The tangent vector at a point $\LARGE (x_1, x_2, \ldots, x_n, f(x_1, x_2, \ldots, x_n))$ is:
$$\LARGE 
\mathbf{T} = \begin{pmatrix} \Delta x_1 \\ \Delta x_2 \\ \vdots \\ \Delta x_n \\ \Delta z \end{pmatrix} = \begin{pmatrix} \Delta x_1 \\ \Delta x_2 \\ \vdots \\ \Delta x_n \\ \sum_{i=1}^n \frac{\partial f}{\partial x_i} \Delta x_i \end{pmatrix}
$$
- - -
## Relationship Between Partial Derivatives and Gradients
### [[Gradients]]
The gradient of the function is defined to be which can be generalized to a function of any number of independent variables.

The gradient can be used in a formula to calculate the directional derivative. 
	The gradient indicates the direction of greatest change of a function of more than one variable

The gradient of a scalar function $f(x, y, z)$ in 3D is a vector that points in the direction of the greatest rate of increase of the function. 
	It is composed of the partial derivatives with respect to each variable:
$$\LARGE \nabla f = \left( \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z} \right)$$
## Relationship Between Partial Derivatives and Directional Derivatives
### [[Directional Derivatives|Directional Derivative]]
![[Pasted image 20240705152625.png|400]]
Directional derivatives measure the rate of change of a function in any given direction and generalize the concept of partial derivatives to arbitrary directions.

The directional derivative can be expressed in terms of the partial derivatives. 
	Specifically, if you have a function $f(x, y)$ and a direction vector $\mathbf{v} = (a, b)$, the directional derivative $D_{\mathbf{v}} f$ in the direction of $\mathbf{v}$ is given by:
$$\LARGE D_{\mathbf{v}} f(x_0, y_0) = \nabla f(x_0, y_0) \cdot \mathbf{u}$$

where $\mathbf{u} = \left( \frac{a}{\sqrt{a^2 + b^2}}, \frac{b}{\sqrt{a^2 + b^2}} \right)$ is the unit vector in the direction of $\mathbf{v}$, and $\nabla f(x_0, y_0)$ is the gradient of $f$ at the point $(x_0, y_0)$, which consists of the partial derivatives:

$$\LARGE \nabla f(x_0, y_0) = \left( \frac{\partial f}{\partial x}(x_0, y_0), \frac{\partial f}{\partial y}(x_0, y_0) \right)$$

Therefore, the directional derivative can be written as:
$$\LARGE D_{\mathbf{v}} f(x_0, y_0) = \frac{\partial f}{\partial x}(x_0, y_0) \cdot \frac{a}{\sqrt{a^2 + b^2}} + \frac{\partial f}{\partial y}(x_0, y_0) \cdot \frac{b}{\sqrt{a^2 + b^2}}$$
### Special Cases
1. When $\mathbf{v}$ is aligned with the $x$-axis ($\mathbf{v} = (1, 0)$), the directional derivative simplifies to the partial derivative with respect to $x$:
$$\LARGE D_{\mathbf{v}} f = \frac{\partial f}{\partial x}$$ 

2. When $\mathbf{v}$ is aligned with the $y$-axis ($\mathbf{v} = (0, 1)$), the directional derivative simplifies to the partial derivative with respect to $y$:
$$\LARGE D_{\mathbf{v}} f = \frac{\partial f}{\partial y}$$
## How the Gradient Uses Partial Derivatives to Calculate the Directional Derivative
> [!note]
> ##### 1. Directional Derivative
> The directional derivative of a function $f$ in the direction of a unit vector $\LARGE \mathbf{u} = \langle u_x, u_y, u_z \rangle$ is a measure of the rate at which $f$ changes in that direction. 
> The gradient allows us to calculate the directional derivative as follows:
> $$\LARGE D_{\mathbf{u}} f = \nabla f \cdot \mathbf{u} = \frac{\partial f}{\partial x} u_x + \frac{\partial f}{\partial y} u_y + \frac{\partial f}{\partial z} u_z$$
> Where:
> $\LARGE D_{u}f$ gives the rate at which the function $f$ changes as you move from a point in the direction of $\mathbf{u}$.​
> 
> Here’s how this works:
> - The gradient $\LARGE \nabla f$ gives the vector of partial derivatives of $f$.
> - The dot product $\LARGE \nabla f \cdot \mathbf{u}$ projects the gradient vector onto the direction vector $\mathbf{u}$, yielding the rate of change of $f$ in that direction.
> ##### 2. Finding Maximal Increase
> The gradient points in the direction of the steepest ascent of the scalar field $f$. 
> By knowing the gradient, one can determine how to move in space to increase the function $f$ most rapidly.

- - -
## [[Directional Derivatives|Directional Derivatives]]


- - -