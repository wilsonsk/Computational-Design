# Parametrization
[[Curves as Parametric Functions|Description of a curve]] with a [[Parameters vs. Variables|parameter]].
*[[Curves Theory|Curves can describe many things.]]*
In essence, parametrization abstracts the **essence of control** over variability, encoding how a system's characteristics are structured, bounded, and explored via independent parameters.

**Parametrization** can be viewed as the process of introducing a **set of independent variables** (parameters) that **govern** or **describe** the possible states, positions, or configurations of a system within a defined space. 
	These parameters **structure** how the variability of the system's characteristics (dimensions/properties) is expressed, effectively transforming a complex, potentially unconstrained set of possibilities into a manageable form.

Parametrization is a key part of the constraint aspect, as it provides a structured way to define and explore the possible variations within a differentiated state. 
	By introducing parameters, you effectively "shape" or "limit" the state, determining how its characteristics are expressed and related. 
		This process confines the infinite possibilities into a manageable and structured form, defining the boundaries of that state.
### Key Aspects of Parametrization
1. **Mapping Potential Variance:**
    - Parametrization provides a way to **map the possible variations** (or states) of an object or system by **assigning independent variables (parameters)**. 
	    - These parameters act as "handles" that systematically adjust and control the features of the system.
    - For example, when defining a curve in space, parametrization assigns a parameter ttt (like time) that "traces out" every point on the curve.
	    - This parameter ttt encapsulates the variance in the curve's shape and position.
1. **Constraining the Degrees of Freedom:**
    - In an abstract sense, parameters are introduced to **structure** the space by reducing its **degrees of freedom**. Before parametrization, a system might have infinite ways to express its dimensions. Through parametrization, a specific **configuration** of the system is outlined, which "bounds" the potential states of the variables involved.
    - This structuring turns a potentially complex system into a more **ordered set** governed by the parameters.
2. **Representation as Component Functions:**
    - In the specific case you're familiar with (defining scalar component functions as vector components), **parametrization** breaks down a complex entity (like a curve, surface, or vector field) into **simpler, scalar components** that vary according to one or more parameters.
    - For example, the parametric representation of a vector in 3D space might be: r(t)=(x(t),y(t),z(t)),\mathbf{r}(t) = (x(t), y(t), z(t)),r(t)=(x(t),y(t),z(t)), where ttt is the parameter, and x(t)x(t)x(t), y(t)y(t)y(t), and z(t)z(t)z(t) are scalar functions describing how each coordinate changes with respect to ttt.
4. **Abstract Conceptualization:**
    - **Parametrization**, at its most abstract, is the **act of defining a system's potential states** in terms of a **smaller, independent set of variables**. These parameters serve as the **coordinates** or **variables of control** that systematically explore the system's full range of possibilities.
    - By choosing parameters, you are essentially **embedding** or **structuring** the object within a new framework that captures its essential features through a simpler set of independent variables. This is why, in mathematics, parametric equations are used to describe curves, surfaces, and other geometries in terms of one or more parameters.


![[Pasted image 20240906071943.png]]
$$\LARGE \vec{r}(t) : [0,1] \to \mathbb{R}^3, \quad \vec{r}(t) = [x(t)\textcolor{red}{,}\space y(t)\textcolor{red}{,}\space z(t)], \quad x,y,z : [0,1] \to \mathbb{R} $$
$$\LARGE \equiv \mathbf{r}(t) = (x(t)\textcolor{red}{,}\space y(t)\textcolor{red}{,}\space z(t))$$
$$\LARGE \equiv \text{A linear Combo of Std. Unit Vectors: }\quad \vec{r}(t) = x(t)\vec{i} \textcolor{red}{+} y(t)\vec{j} \textcolor{red}{+} z(t)\vec{k} $$
$$\LARGE \equiv \text{A linear Combo of Std. Unit Vectors: }\quad\mathbf{r}(t) = x(t)\mathbf{i} \textcolor{red}{+} y(t)\mathbf{j} \textcolor{red}{+} z(t)\mathbf{k}$$
$$\text{Where } \quad \vec{i} = \mathbf{i} = (1,0,0), \quad \vec{j} = \mathbf{j} = (0,1,0), \quad \vec{k} = \mathbf{k} = (0,0,1)$$
$$\text{And where each component function scaled by a std. unit vector is another vector}$$
$$\quad x(t)\mathbf{i} = ( x(t), 0, 0), \quad y(t)\mathbf{j} = (0, y(t), 0), \quad z(t)\mathbf{k} = (0,0,z(t)) $$
$$\LARGE \implies \textcolor{red}{\neq} \cancel{\mathbf{r}(t) = \textcolor{red}{(}x(t)\mathbf{i}, y(t)\mathbf{j},z(t)\mathbf{k}\textcolor{red}{)}}$$
$$\text{As this would imply a vector composed of vectors, instead of a vector composed of scalars}$$
$$\LARGE \text{Where $\vec{r}$ (and $\mathbf{r}$) is a Vector-Valued Function, and $t$ is a parameter.}$$
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
		But when making a parametrization of a circle, $r$ is constant ($\LARGE r \cdot \cos t).$
$$\LARGE \text{A Parametrization: }\quad (x(t),y(t)) = (r \cdot \cos t, r \cdot \sin t), \quad t \in [0,2\pi]$$
$$\LARGE \text{A Parametrization: }\quad (x(t),y(t)) = (r \cdot \cos 2t, r \cdot \sin 2t), \quad t \in [0,\pi]$$
$$\LARGE \text{A Parametrization: }\quad (x(t),y(t)) = (r \cdot \cos \frac{t}{r}, r \cdot \sin \frac{t}{r}), \quad t \in [0,2\pi r]$$
			Only $t$ is a parameter as it still varies along the "curve" of the circle.
				Therefore, the circle is a 1D Curve.
					Notice that by scaling $t$ in a component function, that the position's "velocity" increases because for a given $t$ the position is "ahead" if scaled vs non-scaled or less scaled.

As it relates to the Definition of a Circle by Distance 
![[Pasted image 20240904064640.png|500]]
Where the same geometrical considerations as in polar coordinates (i.e. $(x,y) = (r \cos \theta, r \sin \theta$)  gives the parametrization of a circle.
![[Pasted image 20240904141857.png|500]]
###### 4. 3D Parametric Straight Line
![[Pasted image 20240903160603.png|400]]
*Remember that for the [[Straight Lines#Point Vector Form of a Line in Space (i.e. Parametric Equation)|the parametric equation of a straight line]], you need a point on the line and a directional vector that is parallel to the line.*
$$\large\text{The Parametrization: } \quad \vec{r} = (x(t),y(t),z(t)) = (x_0,y_0,z_0) + t(v_1,v_2,v_3), \quad t \in \mathbb{R}$$
$$\LARGE = (x_0 + tv_1,\space y_0+ tv_2, \space z_0 + tv_3)\quad t \in \mathbb{R}$$
This straight line can be described by many different parametrizations.
	As any point on the straight line can be chosen, as well as any variation of the parallel directional vector in terms of length, and direction.

### A single curve can have many "parametrizations".

## Example Parametrization Problems
##### Identify the curve given by the following parametrization:
$$\LARGE \vec{r} + (\cos 2t, \sin t), \quad t \in [0, 2\pi]$$
$$\LARGE \text{Therefore, }\quad x(t) = \cos 2t, \quad y(t) = \sin t$$
###### 1. Simplify the component functions so to get variables (i.e. parameters) defined in terms of each other
$$\LARGE x(t) = \cos 2t = \textcolor{violet}{\cos^2t - \sin^2t}$$$$\LARGE \text{To eliminate the $\cos^2t$ add $\textcolor{green}{\sin^2t}$ and then subtract it.}$$$$\LARGE = \textcolor{violet}{\cos^2t} + \textcolor{green}{\sin^2t} - \textcolor{green}{\sin^2t} \textcolor{violet}{- \sin^2t}$$$$\LARGE \text{$\textcolor{violet}{\cos^2t} + \textcolor{green}{\sin^2t}$ = 1}$$
$$\LARGE x(t) = \cos 2t = \textcolor{violet}{\cos^2t - \sin^2t}$$$$\LARGE \text{To eliminate the $\cos^2t$ add $\textcolor{green}{\sin^2t}$ and then subtract it.}$$$$\LARGE = \textcolor{violet}{\cos^2t} + \textcolor{green}{\sin^2t} - \textcolor{green}{\sin^2t} \textcolor{violet}{- \sin^2t}$$$$\LARGE \text{And $\quad$ $\textcolor{green}{\sin^2t} - \textcolor{violet}{\sin^2t} = 2\sin^2t$}$$$$\LARGE \text{Therefore, } \quad x(t) = 1- 2\sin^2t$$
###### 2. "Plugin" $x$ and $y$ in order to define them in terms of one another
$$\LARGE x= 1 -2y^2$$
$$\LARGE \text{Therefore, the curve given by this parametrization is a parabola.}$$
## Example of Identifying an Equation of a Parametric Curve
#### Identify the curve with the following parametrization:
$$\LARGE x = \frac{1}{1+t^2}, \quad y = \frac{t}{1+t^2}, \quad t \in \mathbb{R}$$
Notice that the denominator can never be $0$.
	And $x$ can never be $0$. 
		$y$ can be $0$ is $t=0$.
##### 1. Find $t$ in terms of $x$ and $y$ (i.e. Eliminate Parameter $t$) and then $x$ and $y$ in terms of each other
To do this, find the definition for $t$, then substitute that definition of $t$ within one of the definitions of either $x$ or $y$ depending on the how $t$ is defined.
	In this case it, the first step is to eliminate $t^2$ which also happens to eliminate the entire denominator of both variable definitions.
$$\LARGE \frac{y}{x} = \frac{\frac{t}{1+t^2}}{\frac{1}{1+t^2}} = \frac{t}{\cancel{1+t^2}} \left( \frac{\cancel{1+t^2}}{1} \right)$$
$$\LARGE = \frac{y}{x}= t$$
$$\LARGE  \text{Substitute new definition of $t$ in defintion of $x$} \implies x = \frac{1}{1+ \left(\frac{y}{x} \right)^2}$$
$$\LARGE = x = \frac{1}{1+ \left(\frac{y^2}{x^2} \right)} = \frac{1 \cdot x^2}{x^2 \left(1+ \left(\frac{y^2}{x^2} \right)\right)} = \frac{x^2}{\left( x^2 \cdot 1\right) \left( \cancel{x^2} \cdot \left( \frac{y^2}{\cancel{x^2}}\right) \right)}$$
$$\LARGE = x = \frac{x^2}{x^2 + y^2} = x \cdot \frac{x}{x^2 + y^2}$$
This new equation for $x$ holds for $x = 0$ because in that case it would just be $0 = 0$.
	But $x$ can never be $0$ anyways according to the original definition of $x$.
		Where if $t =0$ then $\LARGE x = \frac{1}{1+ 1^1} = 1$ 
		Any if $x \neq 0$, then logically for $\LARGE x = x \cdot \frac{x}{x^2+y^2}$ then the fraction in this equation ($\LARGE \frac{x}{x^2 y^2}$) must be equal to $1$ so that $x = x \cdot 1$.
			And for this fraction ($\LARGE \frac{x}{x^2 y^2}$) to equal $1$ then $x^2 + y^2 = x$ so that $\LARGE \frac{x}{x} = 1$.
				Therefore, $x = x \cdot 1$
$$\large x = 0 \quad \lor \quad x^2 + y^2 = x \implies x^2 - x + y^2 = 0$$
$$\LARGE \text{Completing the square:} \implies \left( x - \frac{1}{2}\right)^2 + y^2 = \frac{1}{4}$$
$$\LARGE \text{This is the equation of a circle $(x^2 + y^2 =1)$}$$
![[Pasted image 20240905064708.png]]
At the origin $(0,0)$ we know $x \neq 0$ so this point is never achieved.  
	Therefore, not all the points of the circle are included in this equation.
![[Pasted image 20240906054041.png|500]]
$$\LARGE x= \frac{1}{2}(1 + \cos \theta) , \quad y = \frac{1}{2} \sin \theta \quad \text{ for } \theta \in [0,2\pi]$$
## Another Example of Identifying an Equation of a Parametric Curve
#### Identify the curve with the following parametrization:
$$\LARGE x = \frac{1- t^2}{1+t^2}, \quad y = \frac{2t}{1+t^2}, \quad t \in \mathbb{R}$$
###### One Method is Just "Plugging In" Values for $t$
$$\LARGE t = 0 \implies x(t) = 1, \quad y(t) = 0$$
$$\LARGE t = 1 \implies x(t) = 0, \quad y(t) = 1$$
$$\LARGE t = -1 \implies x(t) = 0, \quad y(t) = -1$$
##### The Component Functions When $t$ Approaches $+ \infty, \space - \infty$ 
Requires taking the [[Limits|limit]].
###### Simplify form of the limit of $x(t)$
$$\LARGE \lim\limits_{t \to + \infty}x(t) = \lim\limits_{t \to + \infty}\frac{1 -t^2}{1 + t^2} = \lim\limits_{t \to +\infty}\frac{\frac{1}{t^2} - \frac{t^2}{t^2} }{ \frac{1}{t^2} + \frac{t^2}{t^2}} \equiv \lim\limits_{t \to +\infty}\frac{\cancel{t^2}(\frac{1}{t^2} - \frac{t^2}{t^2}) }{ \cancel{t^2}(\frac{1}{t^2} + \frac{t^2}{t^2})} $$
$$\LARGE = \lim\limits_{t \to + \infty}\frac{\frac{1}{t^2} -1}{\frac{1}{t^2} +1}$$
###### Evaluate the Limit of $x(t)$
As $\LARGE t \to + \infty$, the terms involving $\LARGE \frac{1}{t^2}$​ approach 0 because $\LARGE\frac{1}{t^2} \to 0$ as $\LARGE t$ grows larger.
$$\LARGE t \to + \infty \implies \frac{1}{t^2} \to 0 \implies \frac{0-1}{0+1} = \frac{-1}{1} =1$$
###### Simplify form of the limit of $y(t)$
$$\LARGE \lim\limits_{t \to + \infty}y(t) = \lim\limits_{t \to + \infty}\frac{2t}{1 + t^2} = \lim\limits_{t \to +\infty}\frac{2t}{t^2(\frac{1}{t^2} + \frac{t^2}{t^2})} =  \lim\limits_{t \to +\infty}\frac{2\cancel{t}}{\cancel{t^2}t(\frac{1}{t^2} + 1)}$$
$$\LARGE  \lim\limits_{t \to +\infty}\frac{2}{t(\frac{1}{t^2} +1)} = \lim\limits_{t \to +\infty}\frac{2}{(\frac{t}{t^2} + t)} = \lim\limits_{t \to +\infty}\frac{2}{(\frac{\cancel{t}1}{\cancel{t^2}t} + t)} = \lim\limits_{t \to +\infty}\frac{2}{(\frac{1}{t} + t)}$$
$$\LARGE  = \lim\limits_{t\to+\infty}y(t)= \lim\limits_{t \to +\infty}\frac{2}{(\frac{1}{t} + t)}$$
###### Evaluate the Limit of $y(t)$
As $\LARGE t \to + \infty$, the terms involving $\LARGE \frac{1}{t}$​ approach 0 because $\LARGE\frac{1}{t^2} \to 0$ as $\LARGE t$ grows larger.
	And where $\LARGE t \to + \infty$ in $\LARGE \frac{2}{\infty}$, $\LARGE \frac{2}{\infty} \to 0$  
$$\LARGE t \to + \infty \implies \frac{1}{t^2} \to 0 \implies \frac{2}{0+\infty} =0$$

