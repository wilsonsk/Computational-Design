# Parametrization
[[Curves as Parametric Functions|Description of a curve]] with a [[Parameters vs. Variables|parameter]].
*[[Curves Theory|Curves can describe many things.]]*

**Parametrization** can be viewed as the process of introducing a **set of independent variables** (parameters) that **govern** or **describe** the possible states, positions, or configurations of a system within a defined space. 
	These parameters **structure** and **constrain** how the variability of the system's characteristics (dimensions/properties as potential states) is expressed, effectively transforming a complex, potentially unconstrained set of possibilities into a manageable form.
		In essence, parametrization abstracts the **essence of control** over variability, encoding how a system's characteristics are structured, bounded, and explored via independent parameters.

The **arrangement** of **parameters** and **variables** within a system defines the relationships between them and determines how the system behaves, ultimately affecting the **instances** produced. 
	These arrangements govern the **constraints**, **behavior**, and **potential outcomes** of a system, influencing the structure of the solution space. 
		Broadly, the way parameters and variables are arranged affects the **nature of the solutions**, including how values for variables are determined, how they change in response to parameters, and how they are constrained by the system’s structure.

**Parametrization** is a key part of the [[Constraints|constraint]] aspect, as it provides a structured way to define and explore the possible variations within a differentiated state. 
	By introducing parameters, you effectively "shape" or "limit" the state, determining how its characteristics are expressed and related. 
		This process confines the infinite possibilities into a manageable and structured form, defining the boundaries of that state.
### Key Aspects of Parametrization
##### Mapping Potential Variance
Parametrization provides a way to **map the possible variations** (or states) of an object or system by **assigning independent variables (parameters)**. 
	These parameters act as "handles" that systematically adjust and control the features of the system.
		For example, when defining a curve in space, parametrization assigns a parameter $t$ (like time) that "traces out" every point on the curve.
			This parameter $t$ encapsulates the variance in the curve's shape and position.
##### Constraining the Degrees of Freedom
In an abstract sense, parameters are introduced to **structure** the space by reducing its **degrees of freedom**. Before parametrization, a system might have infinite ways to express its dimensions. 
	Through parametrization, a specific **configuration** of the system is outlined, which "bounds" the potential states of the variables involved.
		This structuring turns a potentially complex system into a more **ordered set** governed by the parameters.
##### Representation as Component Functions
In the specific case you're familiar with (defining scalar component functions as vector components), **parametrization** breaks down a complex entity (like a curve, surface, or vector field) into **simpler, scalar components** that vary according to one or more parameters.
	For example, the parametric representation of a vector in 3D space might be: r$\mathbf{r}(t) = (x(t), y(t), z(t))$ where $t$ is the parameter, and $x(t)$, $y(t)$, and $z(t)$ are scalar functions describing how each coordinate changes with respect to $t$.
##### Abstract Conceptualization
**Parametrization**, at its most abstract, is the **act of defining a system's potential states** in terms of a **smaller, independent set of variables**. 
	These parameters serve as the **coordinates** or **variables of control** that systematically explore the system's full range of possibilities.
		By choosing parameters, you are essentially **embedding** or **structuring** the object within a new framework that captures its essential features through a simpler set of independent variables.
			 This is why, in mathematics, parametric equations are used to describe curves, surfaces, and other geometries in terms of one or more parameters.
### Effects of the Configuration of Parameters Relative to Variables
The **arrangement** of parameters and variables is critical in determining the **[[Abstract Mathematical Spaces#3. Third-Level Differentiation (Definition of an Instance to a Defined Constraint within the Defined Dimension Quantification Implemented by Value Assignment)|instances]]** produced by a system. 
	Parameters define the **rules** that govern how variables behave, and the way they interact with variables (through scaling, shifting, multiplication, conditionality, etc.) dictates the **nature of the [[Abstract Mathematical Spaces#The Set of Instances Solution Sets|solutions]]** or **instances**. 
		By controlling the **structure** of the relationships, the system can produce a wide variety of behaviors, from simple linear outcomes to complex, non-linear, or conditional instances.

The **arrangement** of parameters and variables in a system directly impacts the **produced instances** by controlling the nature of the relationships between them. 
	Parameters can act as **scaling factors**, **shifting constants**, or **conditional triggers**, and their configuration relative to the variables determines the shape, size, and behavior of the resulting instances.
		 As we move from simpler linear relationships to more complex non-linear, parametric, or conditional systems, the role of parameters becomes increasingly intricate, allowing for more refined and specialized outcomes.

The **arrangement** of **parameters** and **variables** in a system defines the rules and relationships that govern how the system evolves and produces **specific instances** or **solutions**. 
	The way parameters and variables are configured impacts the **range**, **behavior**, and **types of instances** that are produced, and this applies across various mathematical, computational, and physical systems.
#### Direct Relationships: Parameters as Scaling and Shifting Factors
**Parameters** often act as **scaling** or **shifting factors** in direct relationships with variables. 
	This configuration directly influences the rate of change or the position of the variable in space.
##### Linear Scaling
When a parameter multiplies a variable, it **scales** that variable, affecting how quickly the variable changes as the system evolves.
	The parameter aa controls the **stretching** or **compression** of the relationship between $x$ and $y$. 
		A larger aa makes $y$ grow faster as $x$ increases, while a smaller $a$ slows down the growth.

 - **Example**: $y = ax$
 - **Variables**: $x$ (the independent variable) and $y$ (the dependent variable).
 - **Parameter**: $a$ (scaling factor).
 - **Effect on the instance**: The parameter $a$ determines how **fast or slow** $y$ changes as $x$ increases. 
	 - A larger $a$ causes $y$ to grow faster, while a smaller $a$ causes a slower growth.
		 - The instance produced is a **line**, and the slope of the line is determined by the value of $a$.
##### Additive Arrangements: Shifting
The parameter $b$ moves the relationship between $x$ and $y$ by a constant amount.
	This kind of arrangement affects the **starting point** or baseline for the variable $y$, but it doesn’t alter the rate of change as $x$ changes.
		Parameters can also **shift** a variable, moving its value up or down by a constant amount.

- **Example**: $y = x + b$
- **Variables**: $x$ and $y$.
- **Parameter**: $b$ (shift factor).
- **Effect on the instance**: The parameter $b$ shifts the entire graph of $y = x$ vertically by $b$ units.
	- This changes the **starting point** of the line, but the overall rate of change remains the same.
		- The instance produced is a **shifted straight line**.
##### Combined Scaling and Shifting
- **Example**: $y = ax + b$
- **Variables**: $x$ and $y$.
- **Parameters**: $a$ (scaling) and $b$ (shifting).
- **Effect on the instance**: $a$ controls the **slope** of the line, while $b$ shifts the line vertically. 
	- Together, these parameters define the line’s angle and position in the plane. 
		- The instance produced is a **straight line**, but with its slope and intercept governed by the parameters.

In cases where parameters directly **multiply**, **add**, or otherwise operate on variables, the **produced instances** are often straightforward and predictable. 
	For example, in a linear system like:
$$\LARGE y=ax+b$$
The parameter $a$ **scales** the variable $x$, determining the **rate of change** of $y$ as $x$ changes, while $b$ **shifts** the entire relationship vertically. 
	These kinds of relationships tend to produce **proportional** or **linear** outcomes. 
		The instance produced here is a **straight line**, whose slope is determined by $a$ and intercept by $b$.
#### Non-Linear Influence: Parameters Creating Curvature and Exponential Growth
##### Indirect Relationships: Non-Linear Arrangements
These occur when parameters influence variables in a way that causes the relationship to become **non-proportional**—for example, when variables are squared, cubed, or involved in exponential growth.
	**Non-linear influences** can often be considered **indirect relationships** between parameters and variables, depending on the specific configuration.
		 This is because, in a **non-linear system**, the relationship between a parameter and a variable is **not proportional** or direct (as it would be in a linear system, where a parameter directly scales or shifts the variable in a straightforward manner). 
			 Instead, non-linear influences tend to introduce **curved** or **exponential** behavior, where the effect of the parameter on the variable changes at varying rates depending on the variable's value.

If a parameter indirectly influences a variable (for example, by operating through other parameters or through more complex functions), the produced instance can exhibit more complex behavior. 
	For instance, in a non-linear system such as:
$$\LARGE    y=a(x^2)+b$$
The parameter $a$ indirectly influences how quickly $y$ grows relative to $x$, producing a **parabolic curve** where the shape of the parabola is determined by $a$.
	Here, $x$ is squared first, and only then does aa scale the result, introducing non-linearity into the system. 
		The instance is a **curve**, and changing the value of aa produces different curves.
##### Quadratic Relationships
- **Example**: $y = ax^2 + bx + c$
- **Variables**: $x$ and $y$.
- **Parameters**: $a$, $b$, and $c$ (coefficients of the quadratic equation).
- **Effect on the instance**: The parameter $a$ influences the **curvature** of the parabola, determining whether it opens upwards or downwards and how "wide" or "narrow" it is.
	- The parameter $b$ affects the **tilt** of the parabola, and $c$ shifts it vertically. 
		- The instance produced is a **parabolic curve** whose shape and position are controlled by the parameters. 
			- A large $a$ makes the parabola narrow, while a small $a$ flattens it.
##### Exponential Growth or Decay
In this case, the parameter $a$ influences the **rate** of exponential growth or decay.
	A larger aa causes $y$ to grow much faster as $x$ increases.
		This produces **instances** where growth is much more dramatic than in linear systems.

- **Example**: $y = e^{ax}$
- **Variables**: $x$ and $y$.
- **Parameter**: $a$ (rate of growth/decay).
- **Effect on the instance**: The parameter $a$ controls the **rate** of exponential growth (if $a > 0$) or decay (if $a < 0$).
	- The higher the value of $a$, the faster $y$ grows or decays.
		- The instance produced is an **exponential curve** that becomes steeper or shallower depending on $a$.
##### Power Relationships
- **Example**: $y = ax^n$ (e.g., $n = 2$, quadratic; $n = 3$, cubic).
- **Variables**: $x$ and $y$.
- **Parameter**: $a$ (scaling factor) and $n$ (power).
- **Effect on the instance**: The parameter $a$ scales the curve, while $n$ determines the **degree of the relationship** (e.g., quadratic, cubic).
	- When $n = 2$, the instance produced is a **parabola**.
		- When $n = 3$, the instance is a **cubic curve**, which has a different curvature and inflection behavior compared to the quadratic.
#### Parametric Relationships: Parameters Controlling Paths and Trajectories
In **parametric systems**, parameters define the **path** or **trajectory** of a variable across multiple dimensions. 
	These relationships are particularly useful for describing curves and surfaces in space.

- **Example**: 
$$x = a \cdot \cos(t), \quad y = b \cdot \sin(t)$$
- **Variables**: $x$, $y$, and $t$ (the parameter controlling the curve).
- **Parameters**: $a$ and $b$ (scaling factors for the ellipse).
- **Effect on the instance**: The parameters $a$ and $b$ control the **shape** and **size** of the ellipse traced by $x$ and $y$ as $t$ varies.
	- When $a = b$, the ellipse becomes a **circle**, but when $a \neq b$, the instance is an **ellipse**. The parameters define how the variables move in relation to each other over the course of the parameter $t$.
##### Cycloid or Spirals
- **Example**: 
$$x = r \cdot (t - \sin(t)), \quad y = r \cdot (1 - \cos(t))$$
- **Variables**: $x$, $y$, and $t$ (parameter controlling the curve).
- **Parameter**: $r$ (radius controlling the size of the cycloid).
- **Effect on the instance**: The parameter \(r\) controls the **scale** of the cycloid.
	- The larger $r$, the longer and higher the cycloid loops.
		- The instance produced is a **curve** with periodic loops, and the size of the loops is governed by the parameter $r$.
#### Conditional Constraints: Parameters Introducing Branching Behavior
**Conditional constraints** involve parameters that cause variables to behave differently under certain conditions, introducing **branching behavior**.
	When parameters and variables are arranged in a system with **conditional** logic, such as in logical constraints (e.g., "if-then" conditions), the produced instances depend on the **conditions** being satisfied. 
		**Conditionality** in such systems adds a layer of **context-sensitive behavior**, where the system can switch between different relationships or behaviors based on the value of the variable or parameter.
##### If-Then Logic
- **Example**: 
$$\text{if } x > 0, \quad y = ax \quad \text{else} \quad y = -ax$$
- **Variables**: $x$ and $y$.
- **Parameter**: $a$ (scaling factor, applied differently based on the condition).
- **Effect on the instance**: The parameter $a$ controls the **rate of change** of $y$, but the system **branches** based on whether $x$ is positive or negative.
	- If $x > 0$, $y$ follows a positive slope, but if $x < 0$, $y$ follows a negative slope.
		- The instance produced here depends on the **condition**, and the parameter influences both branches of the behavior.
##### Piecewise Functions
- **Example**:
$$f(x) =
\begin{cases} 
ax + b, & \text{if } x < 0 \\
cx^2 + d, & \text{if } x \geq 0
\end{cases}$$
- **Variables**: $x$ and $f(x)$.
- **Parameters**: $a$, $b$, $c$, and $d$.
- **Effect on the instance**: This defines a **piecewise function**, where \(x\) behaves differently based on its value. 
	- For $x < 0$, the instance is a **line** determined by $a$ and $b$, while for $x \geq 0$, the instance is a **parabola** governed by $c$ and $d$.
		- The parameters define different behaviors in different parts of the domain, creating a **composite instance** that combines two distinct forms.

#### Multi-Parameter Systems: Interactions Between Multiple Parameters and Variables
When multiple parameters interact with a variable, the produced instance depends on the **interplay** between these parameters.
##### Quadratic Equations with Multiple Parameters
- **Example**: 
$$y = ax^2 + bx + c$$
- **Variables**: $x$ and $y$.
- **Parameters**: $a$, $b$, and $c$.
- **Effect on the instance**: The parameter $a$ controls the **curvature** of the parabola, $b$ controls the **slope** or **tilt**, and $c$ shifts the parabola **vertically**. 
	- The instance produced is a **parabola**, but changing any of the parameters alters the shape, position, and orientation of the parabola in the plane.
		- The interaction between $a$, $b$, and $c$ defines the exact form of the curve.
##### Complex Parametric Surfaces
- **Example**:
$$x(u, v) = a \cdot \cos(u) \cdot \sin(v), \quad y(u, v) = b \cdot \sin(u) \cdot \sin(v), \quad z(u, v) = c \cdot \cos(v)$$
- **Variables**: $x$, $y$, and $z$ (in 3D space).
- **Parameters**: $a$, $b$, and $c$ (scaling factors for each dimension).
- **Effect on the instance**: The parameters $a$, $b$, and $c$ scale the surface in each of the three dimensions. 
	- The instance produced is a **parametric surface**, such as an ellipsoid or sphere, and the exact shape depends on the values of the parameters. 
		- The interaction between these parameters controls the surface's curvature and size.


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

