# Equations as Constraints
###### Variables
The dimensions in which the problem exists.
###### Equations
The constraints imposed on those variables.
###### Degrees of Freedom
The remaining variability after applying constraints.
## Solution Sets
A **solution set** is the collection of all values that satisfy a given equation or system of equations. 
	It represents all possible solutions that make the equation true.
###### [[Degrees of Freedom]]

##### Intersections of Solution Sets
When multiple equations are involved, the solution set is the intersection of individual solution sets.
- **Example:**
    - **Equation 1:** x+y=4x + y = 4x+y=4 (a line in R2\mathbb{R}^2R2)
    - **Equation 2:** x−y=0x - y = 0x−y=0 (another line in R2\mathbb{R}^2R2)
    - **Solution Set:** Single point where the two lines intersect.
    - **Degrees of Freedom:** 2−2=02 - 2 = 02−2=0
- **Graphical Interpretation:** The unique point (2,2)(2, 2)(2,2) satisfies both equations.
#### Solution Sets in In $\mathbb{R}^1$ (a number line)
The solution set consists of real numbers, i.e. scalar values.
	With one variable and one equation, you usually get discrete solutions.
###### Points 
Represent solutions to equations.
###### Intervals
Represent solutions to inequalities.
##### Inequalities and Intervals
In $\mathbb{R}^1$, to get intervals (continuous sets of values), inequalities are used.
	**Inequalities** allow for a range of values that satisfy the condition.

- **Example:** $x > 1$
    - **Solution Set:** All real numbers greater than 1.
    - **Graph:** Half-line extending from $x=1$ to infinity.
##### Why Don't Equations in $\mathbb{R}^1$ Produce Solution Sets (containing $>1$ element)?
**Constraint** fully determines the value of the variable.
	I.e. The **Equations** specify exact values where the condition is met.
	**Result:** Discrete solutions (often a single value).
- **Degrees of Freedom:** $n−m=0$
- **Result:** The variable cannot vary freely within the constraints of the equations.
- **Example in $\mathbb{R}^1$:** $x+2=6$
    - **Variables:** $x$
    - **Equations:** 1
    - **Degrees of Freedom:** $1−1=1$
    - **Interpretation:** The only variable is determined by the equation, $x = 4$.

**Example:** $x+2=4$
- **Solution:** $x=2$
- **Solution Set:** $\{2\}$
- **Graphical Representation:** A single point (single scalar value) at $x=2$ on the number line.
- **Variables:** 1 ($x$)
- **Equations:** 1
- **[[Degrees of Freedom|Degrees of Freedom]] (DoF):** $1−1=0$
    - **Interpretation:** The variable is fully constrained by the equation.
#### Solution Sets in In $\mathbb{R}^2$ (Cartesian Plane)
The solution set consists of ordered pairs $(x,y)$.
###### Lines and Curves
Represent solutions to equations with two variables.
###### Regions
Represent solutions to inequalities or systems with inequalities.
##### Why Do Equations in Higher Dimensions Produce Sets of Solutions?
Because there are more variables than equations, not all variables are fully constrained.
- **Degrees of Freedom:** $n−m>0$
- **Result:** Variables can vary freely within the constraints of the equations.
- **Example in $\mathbb{R}^2$:** $x+y=6$
    - **Variables:** $x,y$
    - **Equations:** 1
    - **Degrees of Freedom:** $2−1=1$
    - **Interpretation:** One variable can be chosen freely; the second is determined by the equation.

The set of all points (x,y)(x, y)(x,y) that satisfy an equation like x+y=4x + y = 4x+y=4 forms a **line** in R2\mathbb{R}^2R2. This line represents the entire set of possible solutions, all of which maintain the balance described by the equation.

**Common Outcome:** Often, especially with **continuous equations**, you get infinitely many solutions forming a curve (line, circle, etc.) because there's one degree of freedom—choosing a value for one variable determines the other.

**Exceptions to the General Case**: However, the **nature of the equation** significantly affects the solution set. Here are some scenarios where the number of solutions is finite or nonexistent:
#### Solution Sets in In $\mathbb{R}^3$ (Space)
The solution set consists of $n$-tuples $(x_1, x_2, \dots, x_n)$.
###### Planes and Surfaces 
Represent solutions to equations with three variables.
###### Volumes
Represent solutions to inequalities involving three variables.
##### Why Do Equations in Higher Dimensions Produce Sets of Solutions?
Because there are more variables than equations, not all variables are fully constrained.
- **Degrees of Freedom:** $n−m>0$
- **Result:** Variables can vary freely within the constraints of the equations.
- **Example in $\mathbb{R}^3$:** $x+y+z=6$
    - **Variables:** $x,y,z$
    - **Equations:** 1
    - **Degrees of Freedom:** $3−1=1$
    - **Interpretation:** Two variables can be chosen freely; the third is determined by the equation.
## Equations Constrain Relationships Between Variables
When an equation involves multiple variables, it doesn't just constrain each variable individually. 
	Instead, it defines a **relationship** between the variables.
		 This relationship specifies how the value of one variable affects the value of another to satisfy the equation.
			 This relational constraint leaves room for variables to vary [[Degrees of Freedom|freely]] within the limits set by the equation, leading to a set of solutions.
				 The remaining degrees of freedom after accounting for the constraints determine the [[Degrees of Freedom#Dimensions and Degrees of Freedom|dimensionality of the solution set]].

- **Example:** In the equation $x+y=4$, $x$ and $y$ are linked.
	- Choosing a value for $x$ determines $y$, and vice versa.
		- The equation doesn't restrict $x$ and $y$ to specific individual values but to pairs of values that together sum to 4.
###### In $\mathbb{R}^1$
An equation like $x=3$ is a simple **constraint**: it fixes the value of $x$ to a single point. 
	There’s only one variable involved, so the equation just tells you exactly what value $x$ must take.
		There’s no other variable for $x$ to relate to. 
			You get a **single solution**.
###### In $\mathbb{R}^2$ (or higher)
An equation doesn’t just constrain a single variable to a value—it defines a **relationship** between two or more variables. 
	This relationship constrains **how the variables interact with each other**.
		If you change $x$, the value of $y$ must also change in a specific way so that the equation remains true.
			This interplay between $x$ and $y$ creates a **set of solutions**—an infinite number of points that satisfy the equation, forming a line or curve.

## Why Relationships Between Variables Lead to Sets of Solutions
**A multi-variable equation ($\mathbb{R}^2,\mathbb{R}^3$** doesn’t just constrain a single variable to a fixed value—it often constrains **how one variable can behave relative to another variable**.
	This constraint on the relationship between variables is what produces a **set of solutions** rather than a single point.
		In $\mathbb{R}^2$, this set of solutions often forms a **line** (in the case of a linear equation), which represents the **continuous set of points** where the variables $x$ and $y$ satisfy the equation together.

Because the equation involves two variables connected by a relationship, fixing one variable doesn't fix the other. 
	Instead, it determines the other variable through the equation.

- **Selecting $x$:** If you choose $x=1$, then $y=3$.
- **Selecting $y$:** If you choose $y=0$, then $x=4$.

This interdependence creates a **set of solutions** rather than a single solution, forming a line when graphed in $\mathbb{R}^2$.