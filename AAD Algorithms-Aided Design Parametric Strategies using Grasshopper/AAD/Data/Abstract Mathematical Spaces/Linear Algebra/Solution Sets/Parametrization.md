# Parametrization
[[Curves as Parametric Functions|Description of a curve]] with a [[Parameters vs. Variables|parameter]].
*[[Curves Theory|Curves can describe many things.]]*

![[Pasted image 20240903055710.png]]
$$\LARGE \vec{r}(t), \quad \vec{r}(t) = [x(t),\space y(t),\space z(t)]$$
$$\LARGE \text{Where $\vec{r}$ is a Vector-Valued Function, and $t$ is a parameter.}$$
$$\LARGE \text{And $x(t), \space y(t), \space z(t)$ are Component Scalar Functions, $\mathbb{R}\to \mathbb{R}$} $$
The Scalars returned by these component scalar functions compose the "points" of the returned vector. 
###### $\LARGE t$ as a Parameter
In the context of the parametric function $\vec{r}(t)$, where $\vec{r}(t)$ is typically a vector-valued function describing a curve or path in space, the variable $t$ is identified as a parameter.
## To Find the "Parametrization of a Curve"
Means to establish (two or three) component functions ($\LARGE x(t), y(t), z(t)$) of $\LARGE \vec{r}(t), \quad \vec{r}(t) = [x(t),\space y(t),\space z(t)]$.
##### Examples of Curves Being Parametrized
###### 1. 2D Parametric Curve
![[Pasted image 20240903160459.png|400]]
$$\LARGE \text{The Parametrization: } \quad (x(t), y(t)) = (t, f(t)), \quad t \in [a,b]$$
You simply define the independent variable $\LARGE x$ equal to the parameter, $\LARGE t$ (i.e. the component function $\LARGE x(t) = t$).
	Then define make the second component function (i.e. dependent variable) a **function of the parameter $t$** (i.e. the component function $\LARGE y(t) = f(t)$).
###### 2. 2D Parametric Curve
![[Pasted image 20240903160537.png|400]]
$$\LARGE \text{The Parametrization: } \quad (x(t), y(t)) = (g(t), t), \quad t \in [c,d]$$
You simply define the independent variable $\LARGE x$ equal to the parameter, $\LARGE t$ (i.e. the $y$ component function $\LARGE y(t) = t$).
	Then define make the $x$ component function (i.e. dependent variable) a **function of the parameter $t$** (i.e. the component function $\LARGE x(t) = g(t)$).
###### 3. 1D Parametric Equation of a Circle
![[Pasted image 20240903160550.png|400]]
Here the parameter is the **angle** between the positive $x$-axis and the radius corresponding to the point being described by the parameter $t$. 
	When $r$ described within the equation for [[Circular Motion#Polar Coordinates|polar coordinates]], it is variable (and $t$ is analogous to $\theta$, i.e. the [[Circular Motion#Arc s|arc angle]].
$$\text{Polar Coordinates: }\quad r \cdot \cos \theta$$
		But when making a parametrization of a circle, $r$ is constant ($\LARGE r \cdot \cos t$.
$$\LARGE \text{A Parametrization: }\quad (x(t),y(t)) = (r \cdot \cos t, r \cdot \sin t), \quad t \in [0,2\pi]$$
$$\LARGE \text{A Parametrization: }\quad (x(t),y(t)) = (r \cdot \cos 2t, r \cdot \sin 2t), \quad t \in [0,\pi]$$
$$\LARGE \text{A Parametrization: }\quad (x(t),y(t)) = (r \cdot \cos \frac{t}{r}, r \cdot \sin \frac{t}{r}), \quad t \in [0,2\pi r]$$
			Only $t$ is a parameter as it still varies along the "curve" of the circle.
				Therefore, the circle is a 1D Curve 
As it relates to the Definition of a Circle by Distance 
![[Pasted image 20240904064640.png|500]]
Where the same geometrical considerations as in polar coordinates (i.e. $(x,y) = (r \cos \theta, r \sin \theta$)  gives the parametrization of a circle.
###### 4. 3D Parametric Straight Line
![[Pasted image 20240903160603.png|400]]
*Remember that for the [[Straight Lines#Point Vector Form of a Line in Space (i.e. Parametric Equation)|the parametric equation of a straight line]], you need a point on the line and a directional vector that is parallel to the line.*
$$\large\text{The Parametrization: } \quad \vec{r} = (x(t),y(t),z(t)) = (x_0,y_0,z_0) + t(v_1,v_2,v_3), \quad t \in \mathbb{R}$$
$$\LARGE = (x_0 + tv_1,\space y_0+ tv_2, \space z_0 + tv_3)\quad t \in \mathbb{R}$$
This straight line can be described by many different parametrizations.
	As any point on the straight line can be chosen, as well as any variation of the parallel directional vector in terms of length, and direction.

### A single curve can have many "parametrizations".