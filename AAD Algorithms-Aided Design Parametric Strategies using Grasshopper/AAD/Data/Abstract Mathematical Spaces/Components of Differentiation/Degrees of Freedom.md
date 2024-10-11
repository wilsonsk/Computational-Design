# Degrees of Freedom
In general, **degrees of freedom** represent the number of independent values or choices you can make in a system without violating its constraints. In a system of equations, the degrees of freedom tell you how much "freedom" you have in selecting values for the unknowns.

The concept of **degrees of freedom** refers to the number of independent variables that can vary freely without violating any constraints imposed by equations.
	In a system with $n$ free variables and $m$ independent equations, the degrees of freedom are $\LARGE n−m$.
[[Equations as Constraints]]
[[Functions as Solution Sets]]
## [[Parameters vs. Variables|Parameters]] as Free Variables
In many mathematical models (such as equations, parametric curves, or systems of equations), a **parameter** is a quantity that can take on different values but is not constrained by the system's other variables or equations.
	This gives it the status of a **free variable**.

**Free variable** means the parameter can vary independently without being determined by other variables in the system.
	**Parameters** are often introduced in situations where not all variables are fully constrained by equations. For example, in a system of equations with fewer constraints than variables, parameters represent the remaining degrees of freedom.
### Parameters and Degrees of Freedom
The number of **parameters** you introduce to describe the solution is equal to the number of degrees of freedom left after applying the constraints. 
	Each parameter corresponds to one degree of freedom and allows you to describe how the system can "move" or "vary" within the space.

Just because you're working in **$\mathbb{R}^2$** (a 2D space) with two variables $x$ and $y$, it **does not necessarily mean there are two degrees of freedom**. 
	The number of degrees of freedom is determined by the **constraints** (independent equations) in the system, not just the number of variables.

**The number of degrees of freedom depends on the constraints**, not just the number of variables.
	You might have two variables $x$ and $y$ in $\mathbb{R}^2$, but the degrees of freedom are reduced if there are constraints (independent equations) that relate the variables.
###### [[Equations as Constraints|Constraints]] (independent equations)
Limit the degrees of freedom.
	For every independent equation you have, one degree of freedom is "used up" because it imposes a restriction on how the variables $x$ and $y$ can vary.

**Parameters represent the remaining degrees of freedom**.
	Once the independent equations are applied, the remaining variables that can still vary freely are represented by **parameters**. 
		The number of parameters introduced corresponds to the number of degrees of freedom left in the system.
#### Parameters in Systems of Equations
In a system of equations with more variables than independent equations, some variables are not fully determined by the system. 
	These variables are often expressed in terms of **parameters**, which are **free variables** because they are not directly determined by the system’s constraints.
		In a system of equations, the degrees of freedom tell you how much "freedom" you have in selecting values for the unknowns.

For example:
$$\LARGE x+y=2$$
If you introduce a parameter $\LARGE t$, you might set $\LARGE x=t$, making $\LARGE t$ a free variable. 
	Then you can express $\LARGE y$ in terms of $\LARGE t$:
$$\LARGE y=2−t$$
Here, $t$ is free to vary, making it a **free variable**.
##### Parameters represent degrees of freedom
In a system of equations, when there aren't enough independent constraints (equations) to uniquely determine all the variables, you introduce **parameters** to describe the remaining freedom in the system. 
	Each parameter corresponds to one **degree of freedom**.
###### Degrees of freedom = Number of parameters
The number of degrees of freedom in a system is exactly equal to the number of **parameters** you need to fully describe the solution.
	Every parameter you introduce allows one variable (or some combination of variables) to vary freely within the system, meaning the system has flexibility or "freedom" in choosing those values.

- If you have **one parameter**, you have **one degree of freedom**.
- If you have **two parameters**, you have **two degrees of freedom**, and so on.
##### Parameters Control How Variables Change
Once you've introduced parameters, the other variables in the system become dependent on those parameters. 
	This means that the degrees of freedom (i.e., the number of parameters) determine how the system can evolve or change.
##### Parameters vs. Variables in a System of Equations
In a **system of equations**, we have **primary (or independent) variables**, like $x$ and $y$, which are the unknowns we're trying to solve for. 
	However, when the system doesn't have enough constraints (independent equations) to uniquely determine $x$ and $y$, we introduce **parameters** to express the relationship between them.

For example, consider this system:
$$\LARGE x=t, \quad y=t+5$$
Here, $x=t$ and $y=t+5$ are **scalar equations** because they give specific values of $x$ and $y$ for any value of $t$. 
	In this context, the parameter $t$ is a free variable that lets you describe the relationship between $x$ and $y$ for an infinite number of solutions.
		$x$ and $y$ are the **primary variables** (or independent variables) in the system because they are the unknowns we're solving for.
			**$t$** is introduced as a **parameter** because we lack enough equations to fully determine $x$ and $y$ uniquely. 
				Instead of solving for $x$ and $y$ directly, we express them in terms of $t$, which can take any value.
##### Why is $t$ Considered a Parameter?
Even though $t$ directly defines $x$ and $y$, it is called a **parameter** because it represents the **degree of freedom** in the system.
	That is, $t$ can take on any value, and the values of $x$ and $y$ depend on $t$. 
		So, instead of solving $x$ and $y$ as fixed values, you're saying that they are defined **in terms of a free parameter** $t$.

**In systems with degrees of freedom**, parameters like $t$ are introduced to express how the variables $x$ and $y$ change in relation to each other.
	Parameters are "free" in the sense that they can vary independently, while the values of $x$ and $y$ are constrained by the choice of $t$.

$t$ **defines** both $x$ and $y$, but it is still considered a **parameter** because it’s **not constrained by the system of equations**.
	The system doesn’t directly specify what $t$ must be; it only tells you that $x$ and $y$ are related through $t$. 
		Therefore, $t$ is free to take any value, which is what makes it a parameter.
			**$x$** and **$y$**, on the other hand, are **primary variables** because they are the quantities we’re ultimately solving for, but their values are dependent on $t$.
				To make this clearer, think of $t$ as the **input** that you choose, and $x$ and $y$ as the **outputs** that result from that choice.
					 The parameter $t$ provides the flexibility to choose any value, and that choice defines $x$ and $y$.
### Parameters in Parametric Curves
#### Scalar Functions in Vector-Valued Functions
A **vector function** is a function that gives a vector as its output.
	Each component of the vector is typically a **scalar function** of a parameter, just like how $x=t$ and $y=t+5$ are scalar functions of $t$.

For example, consider the parametric equation of a curve in two-dimensional space:
$$\LARGE \mathbf{r}(t) = \begin{pmatrix} x(t) \\ y(t) \end{pmatrix} = \begin{pmatrix} t \\ t + 5 \end{pmatrix}$$
Here, $\mathbf{r}(t)$ is a **vector function**, and its components, $x(t)=t$ and $y(t)=t+5$, are **scalar functions** of the parameter $t$.
- $\mathbf{r}(t)$ describes the position of a point as $t$ varies, and each component (in this case, $x(t)$ and $y(t)$) is a scalar function of $t$.
- As $t$ changes, the point $(x(t),y(t))$( traces a curve or a line, depending on the nature of the scalar functions.
#### Comparison to Systems of Linear Equations
Both in the **system of equations** example and the **vector function** example, you are dealing with **scalar functions** of a **parameter** $t$. 

1. The difference is how these scalar functions are used:
		**In a system of equations** like:
$$\LARGE x = t, \quad y = t + 5$$
		$x$ and $y$ are expressed as scalar functions of $t$ because the system has one degree of freedom (represented by $t$).
			 This allows you to describe an infinite set of solutions, typically representing a line in $\LARGE \mathbb{R}^2$
    
2. **In vector functions**, you often have something like:
$$\LARGE \mathbf{r}(t) = \begin{pmatrix} x(t) \\ y(t) \end{pmatrix}$$
    
    Each component of the vector is a scalar function of $t$. 
	    The vector function describes a point moving in space (or along a curve) as the parameter $t$ changes.
##### Similarities
In both cases, $t$ is a parameter that allows you to express how the components (either $x$ and $y$, or $x(t)$ and $y(t)$) change as $t$ varies.
	Each of the component functions $x(t)$ and $y(t)$ are **scalar functions** of the parameter $t$, which means they output a real number for each value of $t$.
##### Differences
In the **system of equations**, the parameter $t$ represents the freedom in the solution of the system. 
	It's a way of describing the relationship between the variables $x$ and $y$.

In the **vector function**, the parameter $t$ typically has a geometric or physical meaning (like time or distance) and describes how a point moves along a curve. 
	The scalar functions $x(t)$ and $y(t)$ describe the position of the point at any given $T$.
#### Parametric Equations
When you express equations like $x=t$ and $y=t+5$, you're defining **parametric equations**. 
	These are equations where both $x$ and $y$ are expressed as **functions of a common parameter** (in this case, $t$).
		$x(t)=t$ is a **function** of $t$ because for each value of $t$, there is a corresponding value of $x$.
			Similarly, $y(t)=t+5$ is also a **function** of $t$, because for each value of $t$, there is a corresponding value of $y$.

**Parametric Equations** are equations where both $x$ and $y$ are expressed as functions of a **shared parameter** $t$.
	This gives you a more complete picture of a system's behavior, describing both variables (e.g., $x$ and $y$) in terms of the same parameter.
		The following are the Parametric Equations, where both $x$ and $y$ are expressed in terms of the parameter $t$.
			$x=t$
			$y=t+5$
##### *Important*: Parametric Equations are Functions
$\LARGE x(t)=t$ and $\LARGE y(t)=t+5$ are both technically functions, however, more specifically they are parametric equations where both $x$ and $y$ are expressed as functions of the parameter $t$.
	These are called **parametric equations** because they express the coordinates $x$ and $y$ as functions of a common **parameter** $t$.

They **look like functions** because they **are** functions — they map the parameter $t$ to values for $x$ and $y$. 
	In parametric equations, instead of having a single equation like $y=f(x)$, you have **two functions**, one for $x$ and one for $y$, both depending on a shared parameter $t$.
		They are **equations** in the sense that they describe **relationships** between variables. 
			For instance, $x$ is related to $t$ by the equation $x=t$, and $y$ is related to $t$ by the equation $y=t+5$.
			    They are also **functions** because $x(t)$ and $y(t)$ explicitly describe how $x$ and $y$ depend on the parameter $t$.
				    Each of these is a function of $t$.
						In this case, the parametric equations are telling you that both $x$ and $y$ depend on the same parameter $t$, but they depend on $t$ in different ways (linearly for $y$, and identically for $x$).

So, **parametric equations** can be thought of as a **pair of functions**:
- One function that gives you the $x$-value for each $t$ (i.e., $x(t)=t$),
- Another function that gives you the $y$-value for each $t$ (i.e., $y(t)=t+5$).
These parametric equations describe how $x$ and $y$ vary as $t$ changes.

##### Parametric Equations vs. Standard Functions
In a standard function $y=f(x)$, you typically express $y$ directly as a function of $x$, like this:
$$y=2x+5$$
This is a **non-parametric function**, where you think of x as the independent variable, and $y$ depends on $x$.

In **parametric equations**, you're not directly relating $y$ to $x$. 
	Instead, you have a **third variable** (the parameter $t$) that both $x$ and $y$ depend on.
		 The goal of parametric equations is to describe a curve or relationship in terms of this parameter.
#### Parameters in Parametric Equations
In a parametric system, the parameter $t$ is the **independent variable** that defines both $x$ and $y$.
	It’s a **free parameter** that you can adjust, and as you do, the corresponding values of $x(t)$ and $y(t)$ change accordingly.
		The parameter $t$ **drives** both $x$ and $y$, but it’s not a function itself — it’s just the variable on which the functions depend.

In parametric equations, such as parametric curves, a parameter (like $\LARGE t$ in $\LARGE x(t)$ and $\LARGE y(t)$) is generally considered a **free variable** because:
	It can vary over a certain range (for instance, $\LARGE t \in [0, 2\pi]$ for a circle).
		The value of the parameter controls the behavior of the other variables (like $x(t)$ and $y(t)$), but it is not constrained by those variables.

In a parametric curve, the parameter $t$ controls the movement of the point along the curve.
	The curve itself is represented by the vector $\mathbf{r}(t)$, and as $t$ changes, the position $(x(t), y(t))$ of the point changes.
###### Single Parameter $t$
The entire curve is determined by the single parameter $t$, which can vary freely. 
	This means there is **one degree of freedom**—you have the freedom to choose $t$, and based on this choice, the values of $x(t)$ and $y(t)$ are determined.
###### Dependent Variables
The component functions $x(t)$ and $y(t)$ are **dependent** on the parameter $t$.
	You do not have the freedom to choose $x(t)$ and $y(t)$ independently because their values are constrained by the specific parametric relationship with $t$.
###### Intuition Behind **One** Degree of Freedom:
The degree of freedom in this context refers to how many independent choices you can make in describing the position of the point on the curve.
	Since the position of the point is fully controlled by the parameter $t$, which can vary freely, there is **one degree of freedom**.
		The curve can be thought of as a one-dimensional object (like a line or a path) in two-dimensional space, and you need just one parameter to describe the entire curve.
#### More General Parametric Curves
A **parametric curve** doesn’t need to be a simple shape like a circle—it can describe very complex shapes or paths. 
	For example, if you had the following parametric equations:
$$\LARGE x(t) = t^2 - 3t + 2, \quad y(t) = 2t + 1$$
As $t$ changes, the point $(x(t),y(t))$ traces a **parabola**. 
	Again, the curve is described by how $x$ and $y$ depend on the parameter $t$, so it's a parametric curve.
#### Vector Functions as Parametric Curves
When you represent a parametric curve using a vector function like:
$$\LARGE \mathbf{r}(t) = \begin{pmatrix} x(t) \\ y(t) \end{pmatrix}$$
You’re explicitly showing that the curve is **[[Data/Abstract Mathematical Spaces/Differential Geometry/Parametrization|parametrized]]** by $t$.
	The vector $\mathbf{r}(t)$ gives the position of the point as a function of $t$, and each component of the vector (the $x(t)$ and $y(t)$ functions) is a scalar function of the parameter.

So the curves described by vector functions are called **parametric curves** because the parameter $t$ (or sometimes more than one parameter) dictates how the point moves along the curve.
#### Parametric Curves in Higher Dimensions
In three dimensions, you can have a parametric curve like:
$$\LARGE \mathbf{r}(t) = \begin{pmatrix} x(t) \\ y(t) \\ z(t) \end{pmatrix}$$
Where each of $x(t)$, $y(t)$, and $z(t)$ are scalar functions of $t$.
	As $t$ varies, the point $(x(t),y(t),z(t))$  moves along a curve in three-dimensional space.
## [[Axes and Dimensions|Dimensions]] and Degrees of Freedom
The key to understanding why equations in higher dimensions can represent lines or surfaces lies in the concept of **degrees of freedom**.
	Because there are more variables than equations, not all variables are fully constrained.
#### General Rule $(n-1)$ 
In $n$-dimensional space, an equation reduces the degrees of freedom by one, defining an $\LARGE (n−1)$-dimensional object.
	**In higher dimensions ($n>1$)** 
		Equations can represent lines, planes, or hypersurfaces, depending on the number of variables and equations.
	**In a system with remaining degrees of freedom** 
		There's room for continuous variation, leading to solution sets that are lines, curves, or surfaces.
### The Implications of the Spatial Nature of the [[Axes and Dimensions|Dimensions]] of the Real Number Field and Vector Spaces
#### The Spatial Nature of $\LARGE \mathbb{R}^1$ (i.e. Real Number Field)
Imagine a **tightrope**, stretching infinitely in both directions. 
	This is $\mathbb{R}^1$—a **one-dimensional space**. 
		You can move only **forward** or **backward** along this line.
			Every point on this line can be represented by a **single number** (the $x$-coordinate). You can think of this space as **extremely constrained**—there is no room to move up, down, or in any other direction.
##### Equations as Constraints in $\LARGE \mathbb{R}^1$
Because there is only **one degree of freedom**, an equation in $\LARGE \mathbb{R}^1$ almost always produces a **single solution** (a single point on the number line). 
	There’s no room to move in any other direction to create a **set** of solutions. 
		In $\LARGE \mathbb{R}^1$, equations effectively **pin** the variable to a specific value, locking down the freedom of movement.
##### Degrees of Freedom in $\LARGE \mathbb{R}^1$
A single variable $x$ has one degree of freedom.
	A single equation in one variable typically doesn't produce an interval because there's only one degree of freedom, and the equation removes that freedom by specifying exact values.
		An equation like $\LARGE f(x) = 0$ constrains that freedom, typically resulting in discrete solutions.

In $\mathbb{R}^1$, you have **one degree of freedom**.
	This means that a variable like $x$ is free to move **only along this single dimension** (the number line).
		An **equation** like $\LARGE x=3$ imposes a **constraint**: it **fixes** $x$ to one specific value, meaning $x$ cannot move anymore—it is trapped at $\LARGE x=3$.

**Interpretation:**
	No degrees of freedom remain.
		The equation fully determines the value of $x$. 
			There's only one solution.
##### Solution Sets of Equations in $\LARGE \mathbb{R}^1$
The solution set of an equation in $\LARGE \mathbb{R}^1$ contains only a single element.
#### The Spatial Nature of $\LARGE \mathbb{R}^2$
Now imagine you’ve stepped off the tightrope and onto a **sheet of paper** that stretches infinitely in two directions. 
	This is $\LARGE \mathbb{R}^2$—a **two-dimensional plane** where you can move **forward, backward, left, or right**.
		Every point on this plane can be described by **two numbers**: $x$ and $y$.
			 Now, instead of just a single number line, you have an **entire plane** of possibilities.

In $\LARGE \mathbb{R}^2$, there are **two degrees of freedom**: one for the $x$-axis and one for the $y$-axis.
	Without any constraints, $x$ and $y$ are free to take on any values, moving around the plane.
##### Degrees of Freedom in $\LARGE \mathbb{R}^2$ 
Two variables $x$ and $y$ have two degrees of freedom.
	A single equation with two variables still leaves one degree of freedom, allowing for a continuous set of solutions (a line or curve).
		An equation like $\LARGE f(x,y)=0$ reduces the degrees of freedom by one, leaving one degree of freedom.
			 This remaining freedom allows for a continuous set of solutions—a line or curve.

**Interpretation:** One degree of freedom remains.
	You can freely choose a value for one variable, and the equation will determine the corresponding value of the other variable.
		 This results in infinitely many solutions that form a line in the plane.
##### Equations as Constraints in $\LARGE \mathbb{R}^2$
An equation like $\LARGE x + y = 4$ introduces a **constraint**. 
	This constraint **links** the two degrees of freedom (the two variables $x$ and $y$) together in a specific way.
###### Abstractly
The equation doesn’t pin $x$ or $y$ to a specific value independently, but rather says: "For any value of $x$, $y$ must adjust so that the sum of $x$ and $y$ is always 4."
	This creates a **relationship** between $x$ and $y$.

Because of the two degrees of freedom in $\LARGE \mathbb{R}^2$, the equation doesn’t lead to a single point but to a **set of points**.
	These points form a **line** on the plane, which represents all the possible pairs $(x, y)$ that satisfy the equation.

In essence, the presence of two degrees of freedom allows variables to "play off" one another, meaning that even though there’s a constraint, they can still explore a whole **set of possible solutions** (the line).
##### Solution Sets of Equations in $\LARGE \mathbb{R}^2$
The solution set of an equation in $\LARGE \mathbb{R}^2$ contains only a single element.
#### The Spatial Nature of $\LARGE \mathbb{R}^3$
Now, imagine you're no longer confined to a flat plane—you’re in **open space** where you can move **forward/backward, left/right, and up/down**.
	This is $\LARGE \mathbb{R}^3$—a three-dimensional space.
		Every point in this space is described by **three numbers**: $x$, $y$, and $z$. 
			These coordinates allow you to locate any point within this infinite, three-dimensional volume.
##### Degrees of Freedom in $\LARGE \mathbb{R}^3$
Two variables $x$ and $y$ have three degrees of freedom.
	A single equation with three variables still leaves two degree of freedom, allowing for a continuous set of solutions (a line or curve).
		An equation like $\LARGE f(x,y,z)=0$ reduces the degrees of freedom by one, leaving two degree of freedom.
			 This remaining freedom allows for a continuous set of solutions—a plane.
 
In $\LARGE \mathbb{R}^3$, there are **three degrees of freedom**. 
	The variables $x$, $y$, and $z$ are independent and can move freely in three different directions.
		Without constraints, you can move in any direction—up, down, forward, or sideways.
##### Equations as Constraints in $\LARGE \mathbb{R}^3$
An equation like $\LARGE x+y+z=7$ introduces a **constraint** between the three variables. 
	But now, because there are **three degrees of freedom**, the equation doesn’t lock the variables into a single point or a line. Instead, the constraint creates a **surface** in $\LARGE \mathbb{R}^3$.
###### Abstractly
The equation ensures that for any combination of $x$ and $y$, $z$ must adjust so that the sum of all three variables equals 7. 
	This flexibility creates a **surface** (a plane in this case), which represents the set of all possible points $(x, y, z)$ that satisfy the equation.

In three-dimensional space, equations like this produce **surfaces**, not just lines or points. 
	This is because each variable has enough freedom to adjust while still satisfying the constraint. 
		The three degrees of freedom allow for a more complex set of solutions—a **surface** rather than just a line.
##### Solution Sets of Equations in $\LARGE \mathbb{R}^3$
The solution set of an equation in $\LARGE \mathbb{R}^3$ contains only a single element.
## Degrees of Freedom and Solution Sets
The number of degrees of freedom directly affects the nature of the solution set.
##### Single Variable and Single Equation ($\mathbb{R}^1$) ($m=n$)
- **Constraint:** The equation fully determines the value of the variable.
- **Result:** Discrete solutions (often a single value).
##### Multiple Variables and Fewer Equations ($\mathbb{R}^n, m < n$)
- **Constraint:** The equation relates variables but doesn't fix them individually.
- **Result:** Infinite solutions forming geometric objects (lines, planes).
##### Number of Equations Equals Number of Variables ($m=n$)
- **Constraint:** Variables are fully determined.
- **Result:** Unique solution (single point), provided the equations are independent and consistent.
##### Zero Degrees of Freedom
The system is fully constrained. 
	There's a finite set of discrete solutions (often just one).
##### One Degree of Freedom
The system has a single independent variable.
	The solutions form a one-dimensional continuum (a line or curve).
##### Two Degrees of Freedom
The system has two independent variables. 
	The solutions form a two-dimensional continuum (a surface).
### Degree of Freedom in Parametric Curves
In the context of parametric curves, **a degree of freedom refers to the number of independent parameters** (or variables) that control the position of a point on the curve.
- In a parametric curve, you typically have a vector-valued function like:
$$ \vec{r}(t) = [\vec{x}(t), \vec{y}(t), \vec{z}(t)] $$

  where $t$ is the **single degree of freedom**. 
	  This is because $t$ alone controls the values of $\vec{x}(t)$, $\vec{y}(t)$, and $\vec{z}(t)$, and thus determines the entire position of a point along the curve.

The **degree of freedom** here refers to the fact that a single parameter, $t$, can be varied to generate different points along the curve. 
	In general:
	  A parametric curve in 2D space is controlled by one degree of freedom $t$.
	  A parametric curve in 3D space is still controlled by one degree of freedom $t$, but the points are represented in a higher-dimensional space.
#### Example:
For the parametric curve of a circle:

$$ \vec{r}(t) = [\cos(t), \sin(t)] $$

The degree of freedom is the parameter $t$, which controls the position of the point as it moves along the circle.
	As $t$ varies, different positions on the circle are traced out, but there is only one independent variable (degree of freedom) controlling the motion.
### Degree of Freedom in Linear Algebra Solution Sets
In linear algebra, **the degree of freedom refers to the number of free variables in the solution set of a system of linear equations**. 
	It represents the number of independent choices you can make in a solution, which is equivalent to the **dimension of the solution space**.

When solving a system of linear equations, the degree of freedom is the number of independent variables that can take any value, while the remaining variables depend on those free choices.
#### Key Concepts
##### Full Rank
A system of equations has **no degree of freedom** (i.e., a unique solution) if the number of independent equations matches the number of unknowns (variables).
##### Underdetermined System
If there are fewer independent equations than unknowns, the system is **underdetermined**, and it has **infinitely many solutions**. 
	In this case, the **degree of freedom** is the number of free variables that can vary independently.
##### Overdetermined System
If there are more equations than unknowns, the system may have **no solutions** unless the extra equations are dependent.
#### Example:
Consider the system of linear equations:
$$\LARGE 
\begin{align*}
x + y &= 2 \\
2x + z &= 3
\end{align*}
$$
In this case, there are three variables ($x$, $y$, $z$) but only two independent equations. 
	This means that the system is **underdetermined** and will have **one degree of freedom**. 
		You can choose one variable freely (say $y$), and then $x$ and $z$ will depend on the choice of $y$.

Solving the system:
1. From the first equation: $x = 2 - y$.
2. From the second equation: $z = 2y - 1$.

So the solution can be expressed as:
$$\LARGE 
(x, y, z) = (2 - y, y, 2y - 1)
$$
	Here, $y$ is the **free variable**, and the degree of freedom is 1 because you can freely choose $y$.
