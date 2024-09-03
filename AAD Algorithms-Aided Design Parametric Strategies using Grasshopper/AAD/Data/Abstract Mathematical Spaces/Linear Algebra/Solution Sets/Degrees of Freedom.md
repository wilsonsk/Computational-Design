# Degrees of Freedom
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
