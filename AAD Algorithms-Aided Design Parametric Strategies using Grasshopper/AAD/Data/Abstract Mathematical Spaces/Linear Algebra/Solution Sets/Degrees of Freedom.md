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
##### Degrees of Freedom in $\LARGE \mathbb{R}^2$ 
Two variables $x$ and $y$ have two degrees of freedom.
	A single equation with two variables still leaves one degree of freedom, allowing for a continuous set of solutions (a line or curve).
		An equation like $\LARGE f(x,y)=0$ reduces the degrees of freedom by one, leaving one degree of freedom.
			 This remaining freedom allows for a continuous set of solutions—a line or curve.

**Interpretation:** One degree of freedom remains.
	You can freely choose a value for one variable, and the equation will determine the corresponding value of the other variable.
		 This results in infinitely many solutions that form a line in the plane.
## Degrees of Freedom and Solution Sets
The number of degrees of freedom directly affects the nature of the solution set.
##### Single Variable and Single Equation ($\mathbb{R}^1$)
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
