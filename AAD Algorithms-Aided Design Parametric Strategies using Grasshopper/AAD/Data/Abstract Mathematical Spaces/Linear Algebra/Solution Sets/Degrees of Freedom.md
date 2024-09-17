# Degrees of Freedom
The concept of **degrees of freedom** refers to the number of independent variables that can vary freely without violating any constraints imposed by equations.
	In a system with $n$ variables and $m$ independent equations, the degrees of freedom are $\LARGE n−m$.
[[Equations as Constraints]]
[[Functions as Solution Sets]]
## Dimensions and Degrees of Freedom
The key to understanding why equations in higher dimensions can represent lines or surfaces lies in the concept of **degrees of freedom**.
	Because there are more variables than equations, not all variables are fully constrained.
#### General Rule $(n-1)$ 
In $n$-dimensional space, an equation reduces the degrees of freedom by one, defining an $\LARGE (n−1)$-dimensional object.
	**In higher dimensions ($n>1$)** 
		Equations can represent lines, planes, or hypersurfaces, depending on the number of variables and equations.
	**In a system with remaining degrees of freedom** 
		There's room for continuous variation, leading to solution sets that are lines, curves, or surfaces.
##### Degrees of Freedom in $\LARGE \mathbb{R}^1$
A single variable $x$ has one degree of freedom.
	A single equation in one variable typically doesn't produce an interval because there's only one degree of freedom, and the equation removes that freedom by specifying exact values.
		An equation like $\LARGE f(x) = 0$ constrains that freedom, typically resulting in discrete solutions.

**Interpretation:**
	No degrees of freedom remain.
		The equation fully determines the value of $x$. 
			There's only one solution.
###### The Spatial Nature of R1\mathbb{R}^1R1:
- Imagine a **tightrope**, stretching infinitely in both directions. This is R1\mathbb{R}^1R1—a **one-dimensional space**. You can move only **forward** or **backward** along this line.
- Every point on this line can be represented by a **single number** (the xxx-coordinate). You can think of this space as **extremely constrained**—there is no room to move up, down, or in any other direction.
###### Degrees of Freedom in R1\mathbb{R}^1R1:
- In R1\mathbb{R}^1R1, you have **one degree of freedom**. This means that a variable like xxx is free to move **only along this single dimension** (the number line).
- An **equation** like x=3x = 3x=3 imposes a **constraint**: it **fixes** xxx to one specific value, meaning xxx cannot move anymore—it is trapped at x=3x = 3x=3.

Because there is only **one degree of freedom**, an equation in R1\mathbb{R}^1R1 almost always produces a **single solution** (a single point on the number line). There’s no room to move in any other direction to create a **set** of solutions. In R1\mathbb{R}^1R1, equations effectively **pin** the variable to a specific value, locking down the freedom of movement.
##### Degrees of Freedom in $\LARGE \mathbb{R}^2$ 
Two variables $x$ and $y$ have two degrees of freedom.
	A single equation with two variables still leaves one degree of freedom, allowing for a continuous set of solutions (a line or curve).
		An equation like $\LARGE f(x,y)=0$ reduces the degrees of freedom by one, leaving one degree of freedom.
			 This remaining freedom allows for a continuous set of solutions—a line or curve.

**Interpretation:** One degree of freedom remains.
	You can freely choose a value for one variable, and the equation will determine the corresponding value of the other variable.
		 This results in infinitely many solutions that form a line in the plane.
###### The Spatial Nature of R2\mathbb{R}^2R2:
- Now imagine you’ve stepped off the tightrope and onto a **sheet of paper** that stretches infinitely in two directions. This is R2\mathbb{R}^2R2—a **two-dimensional plane** where you can move **forward, backward, left, or right**.
- Every point on this plane can be described by **two numbers**: xxx and yyy. Now, instead of just a single number line, you have an **entire plane** of possibilities.
###### Degrees of Freedom in R2\mathbb{R}^2R2:
- In R2\mathbb{R}^2R2, there are **two degrees of freedom**: one for the xxx-axis and one for the yyy-axis.
- Without any constraints, xxx and yyy are free to take on any values, moving around the plane.
###### Equations as Constraints in R2\mathbb{R}^2R2:
- An equation like x+y=4x + y = 4x+y=4 introduces a **constraint**. This constraint **links** the two degrees of freedom (the two variables xxx and yyy) together in a specific way.
- **Abstractly**: The equation doesn’t pin xxx or yyy to a specific value independently, but rather says: "For any value of xxx, yyy must adjust so that the sum of xxx and yyy is always 4." This creates a **relationship** between xxx and yyy.

Because of the two degrees of freedom in R2\mathbb{R}^2R2, the equation doesn’t lead to a single point but to a **set of points**. These points form a **line** on the plane, which represents all the possible pairs (x,y)(x, y)(x,y) that satisfy the equation.

In essence, the presence of two degrees of freedom allows variables to "play off" one another, meaning that even though there’s a constraint, they can still explore a whole **set of possible solutions** (the line).
##### Degrees of Freedom in $\LARGE \mathbb{R}^3$ 
Two variables $x$ and $y$ have three degrees of freedom.
	A single equation with three variables still leaves two degree of freedom, allowing for a continuous set of solutions (a line or curve).
		An equation like $\LARGE f(x,y,z)=0$ reduces the degrees of freedom by one, leaving two degree of freedom.
			 This remaining freedom allows for a continuous set of solutions—a plane.
###### The Spatial Nature of R3\mathbb{R}^3R3:
- Now, imagine you're no longer confined to a flat plane—you’re in **open space** where you can move **forward/backward, left/right, and up/down**. This is R3\mathbb{R}^3R3—a three-dimensional space.
- Every point in this space is described by **three numbers**: xxx, yyy, and zzz. These coordinates allow you to locate any point within this infinite, three-dimensional volume.
###### Degrees of Freedom in R3\mathbb{R}^3R3:
- In R3\mathbb{R}^3R3, there are **three degrees of freedom**. The variables xxx, yyy, and zzz are independent and can move freely in three different directions.
- Without constraints, you can move in any direction—up, down, forward, or sideways.
###### Equations as Constraints in R3\mathbb{R}^3R3:
- An equation like x+y+z=7x + y + z = 7x+y+z=7 introduces a **constraint** between the three variables. But now, because there are **three degrees of freedom**, the equation doesn’t lock the variables into a single point or a line. Instead, the constraint creates a **surface** in R3\mathbb{R}^3R3.
    
- **Abstractly**: The equation ensures that for any combination of xxx and yyy, zzz must adjust so that the sum of all three variables equals 7. This flexibility creates a **surface** (a plane in this case), which represents the set of all possible points (x,y,z)(x, y, z)(x,y,z) that satisfy the equation.

In three-dimensional space, equations like this produce **surfaces**, not just lines or points. This is because each variable has enough freedom to adjust while still satisfying the constraint. The three degrees of freedom allow for a more complex set of solutions—a **surface** rather than just a line.
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
