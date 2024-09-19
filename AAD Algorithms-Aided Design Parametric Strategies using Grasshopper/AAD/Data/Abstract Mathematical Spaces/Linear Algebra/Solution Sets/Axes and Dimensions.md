# Axes and Dimensions
An axis is a **conceptual dimension**, where the "value" along the axis corresponds to different states or outcomes of a system. 
	It doesn't have to be spatial at all.
		 It’s about representing the **[[Degrees of Freedom|degrees of freedom]]** or **[[Degrees of Freedom#Parameters and Degrees of Freedom|parameters]]** that define your system’s behavior.

An **axis** is essentially a **set of possibilities** or a **range of values** for some variable, just like a set defines possible elements. 
	An axis can be thought of as a **range** in which the system can exist or evolve, and it doesn’t need to be limited to physical space.
		Where a "variable" represents a potential value that corresponds with a given axis, that is, a set of possible values.
### Dimensions and Axes as Sets of Possible Values (Domains and Codomains)
Each axis in a coordinate system (whether it's 1D, 2D, 3D, or higher-dimensional) corresponds to a **range of values** that a variable can take. 
	These sets of possible values are often described as the **codomain** or **domain** of a function.
		Where $x$ and $y$ represent individual, variable values corresponding to a $x$ or $y$ domain or codomain (i.e. axis/set of all possible values).
###### Dimension/Axis
Each **axis** represents a **set of possible values**. 
	Moving along the xxx-axis is like exploring all possible values of xxx; the same is true for yyy and zzz.

In a Cartesian plane, each axis (e.g., $x$-axis, $y$-axis, etc.) represents the set of all possible values that the corresponding variable can take.
	**In one dimension**, such as a simple number line, the $x$-axis is a set of all possible values that $x$ can take.
		**In two dimensions**, the Cartesian plane has an $x$-axis and a $y$-axis. Each of these axes represents the range of values that the variables $x$ and $y$ can independently take.
			So, dimensions or axes are essentially **possibilities** — they define the **space** or **range** in which variables can exist.
###### Domain
If we think abstractly, each axis is really a **domain**, which is the set of all values that the independent variable (i.e. independent set of possible values) could map to. 
	For example, in $\LARGE y=f(x)$, the set of all possible $x$-values forms the **domain** of the function $f$.
###### Codomain
If we think abstractly, each axis is really a **codomain**, which is the set of all values that the dependent variable (i.e. dependent set of possible values) could map to. 
	For example, in $\LARGE y=f(x)$, the set of all possible $y$-values forms the **codomain** of the function $f$.
#### Variables
##### Variable as a Selector of Values
A **variable** is a **selector** that picks a specific value from the set of all possible values represented by an axis.

###### A Variable in 1D Space
there is just one axis (say, the xxx-axis), and the variable xxx selects a single point from this axis. 
	The value of xxx can vary freely, so you can think of the variable xxx as "moving" along the xxx-axis, selecting different values from its set of possibilities.
###### A Variable in 2D Space
(with xxx- and yyy-axes), the variables xxx and yyy select values from two independent sets of possible values.
	Together, these two variables select a specific point on the plane, defined by their respective values on the xxx-axis and yyy-axis.
##### Variable as a Coordinate
In the abstract sense, a variable is like a **coordinate** that marks where you are on an axis. 
	It tells you **which value** you are selecting from the set of possibilities that the axis represents.
		For instance, in 2D space, a point (x,y)(x, y)(x,y) is defined by its **coordinates** xxx and yyy. 
			These coordinates are the values chosen from the xxx-axis and yyy-axis, respectively.
				 The variable xxx selects a value from the xxx-axis, and yyy selects a value from the yyy-axis, together specifying a point in 2D space.
##### Variable as a Degree of Freedom
A variable represents a **degree of freedom** when no constraints are imposed on it. 
	Each variable corresponds to an axis along which you are free to move and select different values.
		In a system with nnn independent variables, you have nnn degrees of freedom, meaning you can move freely along each axis independently. Each variable represents one of these freedoms — an independent choice of value from a set of possibilities.

If you impose constraints (like through an equation), the variable may no longer be completely independent, and its value may become dependent on the values of other variables.
#### Degrees of Freedom as the Number of Independent Axes
The **degrees of freedom** are directly tied to the number of **independent axes** in the system.
	Each degree of freedom corresponds to an axis along which a variable can change freely and independently of other variables. In the absence of constraints.
		Thus, **degrees of freedom** represent how many axes are available for independent variation. 
			Each axis is like an open dimension that offers a full range of values, and having multiple degrees of freedom means you can explore these axes without restrictions.
###### Degrees of Freedom in a 1D system
There is **1 degree of freedom** because there is only one axis (the xxx-axis), and the system can move freely along it.
    The possible values of xxx form the **set of possible values** along the xxx-axis.
###### Degrees of Freedom in a 2D system
There are **2 degrees of freedom** because there are two independent axes (the xxx-axis and the yyy-axis). The system can move freely along both axes, meaning you can vary both xxx and yyy independently.
	The combination of xxx and yyy values forms a **plane** of possibilities, and the degrees of freedom represent the freedom to move along both axes.
###### Degrees of Freedom in a 3D system
There are **3 degrees of freedom** because the system can vary along the xxx-axis, yyy-axis, and zzz-axis. 
	You have full freedom to move in three independent directions, and each degree of freedom corresponds to a set of possible values along one of the axes.
#### Degrees of Freedom as Choices on Axes
You can also think of degrees of freedom in terms of **choices** you can make:
- If you have **one degree of freedom**, you can make a free choice about the value on one axis (say, the xxx-axis).
- With **two degrees of freedom**, you have two independent choices: one for xxx (along the xxx-axis) and one for yyy (along the yyy-axis).
- As you add more degrees of freedom, you’re adding more independent choices for values along additional axes.

So, each degree of freedom corresponds to an independent **choice** you can make about the value of a variable, and these choices are mapped onto the possible values represented by the axes.
#### Degrees of Freedom as Dimensions of Possibilities
In an abstract sense, each degree of freedom adds a new **dimension** to the set of possibilities:
- **1 degree of freedom** gives you a 1D space (a line), where your only choice is where to move along a single axis.
- **2 degrees of freedom** give you a 2D space (a plane), where you can move independently along both the xxx-axis and yyy-axis.
- **3 degrees of freedom** give you a 3D space (a volume), where you can vary independently along three axes.
#### Equations as Constraints on Those Possibilities (Codomains, i.e. Axes)
Think of each **axis** as representing the **entire range of possible values** a variable can take. 
	For example, the $x$-axis contains all the possible values that $x$ could assume. 
		Without any constraints, $x$ is free to roam anywhere on its axis, meaning you have **complete freedom** in choosing its value.
			The same goes for any other axis, like $y$, $z$, or even higher-dimensional axes.
				Now, an **equation** acts like a **rule** or a **restriction** on this freedom.
					 The equation tells you that **not all combinations** of values along these axes are valid — only the combinations that **satisfy the equation**.

Equations serve to **constrain** or **limit** the possibilities defined by the axes. 
	When you have multiple dimensions (e.g., $x$-axis and $y$-axis in a plane), the equation introduces a **relationship** between those dimensions.

When an equation or a relationship between variables is introduced, it typically **reduces the number of degrees of freedom** by constraining the possible values of one variable based on the values of others.
	Without constraints, you can move freely along all the axes, corresponding to **full degrees of freedom**.
		When a constraint (equation) is introduced, it effectively "ties" one variable to another, reducing your freedom to move independently.
			 The degrees of freedom are reduced because some variables are no longer free to vary independently — they are now dependent on other variables.

In a 2D space, you have two degrees of freedom: xxx and yyy can vary independently.
	If you impose a constraint like y=2xy = 2xy=2x, the equation restricts yyy to depend on xxx, so you lose one degree of freedom. Now, you only have **1 degree of freedom**, because once you choose a value for xxx, yyy is no longer free — it's determined by xxx.

For instance:
	In the equation of a circle $\LARGE x^2 + y^2 = r^2$, both $x$ and $y$ can take on any values from their respective axes (dimensions), but the **equation** constrains the possible pairs $(x,y)$ that satisfy this condition. 
		The equation restricts the values of $x$ and $y$ so that they must lie on the circle.

In this sense, **equations** are rules or conditions that **carve out specific subsets** of possibilities from the larger set of potential values on the axes. 
	They act like **filters** that limit what combinations of variables are allowed.
#### How Equations Reduce Degrees of Freedom
The number of **degrees of freedom** corresponds to the directions in which you can move independently. You can walk along the xxx-axis, the yyy-axis, and the zzz-axis without being forced to change direction on any other axis.

Initially, in an unconstrained system, each variable corresponds to an independent axis, and each axis represents a full **degree of freedom**. You can vary xxx, yyy, and zzz independently in 3D space. But when an **equation** is introduced, it imposes a relationship between variables, which effectively **reduces the degrees of freedom**.

- **Without the equation**, all points in the space are possible — you can move freely along all axes.
- **With the equation**, the movement is **restricted** to only those points that satisfy the equation. This filtering process reduces the dimensionality of the system, reducing the **degrees of freedom**.
- 
- **Before the equation**: Both xxx and yyy are free to vary independently, meaning you have 2 degrees of freedom. You could move anywhere along the xxx-axis and yyy-axis without restriction.
    
- **After the equation**: The equation forces xxx and yyy to satisfy the relationship x2+y2=r2x^2 + y^2 = r^2x2+y2=r2, meaning they can’t vary independently anymore. For any xxx you choose, yyy must be constrained to a specific value to satisfy the equation. Therefore, the equation reduces the system’s degrees of freedom from 2 to **1**. You are now constrained to move along a circle, not the entire xyxyxy-plane.
- In this case, you are left with **one degree of freedom** — the angle ttt that parameterizes the position on the circle (often expressed as parametric equations: x(t)=rcos⁡(t)x(t) = r\cos(t)x(t)=rcos(t) and y(t)=rsin⁡(t)y(t) = r\sin(t)y(t)=rsin(t)).
#### How Constraints Influence Parameters
A **parameter** is often introduced to describe the remaining freedom in a constrained system.
	Once an equation has reduced the degrees of freedom, the parameter provides a way to describe the **dependent relationships** between the remaining variables.
		In systems with constraints, parameters are used to capture the **remaining freedom** after equations have reduced the degrees of freedom.
			 When equations restrict movement along certain axes, parameters emerge as a way to describe **how the remaining variables move together**.

**After imposing constraints** through equations, the parameters allow you to **track the behavior** of the system as it moves within the constrained space.

In the circle example, after the equation $x^2 + y^2 = r^2$ has constrained the system, you’re left with one degree of freedom, which can be described by the parameter $t$ (the angle):
$$x(t) = r \cos(t), \quad y(t) = r \sin(t)$$
Here, $t$ acts as a **parameter** that governs the values of $x$ and $y$. 
	The equation constrains the relationship between $x$ and $y$, and the **parameter $t$** provides the **single degree of freedom** that allows you to move around the circle.
#### Parameters as Controllers of Axes
**Parameters** are values or variables that **control** the system’s behavior by influencing other variables. 
	They often act as **hidden dimensions** or **inputs** that affect the output of the system.
		**Parameters** are like hidden levers that influence how you move along these axes. 
			For example, if you are on a train moving along a track that weaves in all three directions (a parametric curve), you are following a specific path through the room, controlled by a parameter like $t$, even though the room itself has three dimensions.

Think of parameters as variables that define how the system's **axes** or **degrees of freedom** behave:
	In a parametric system, instead of having direct control over variables like $x$ and $y$, you introduce a **parameter** (say, $y$) that controls them.
		For instance, in parametric equations like: $x(t) = t, \quad y(t) = t + 5$ $t$ is the **parameter** that defines how both $x$ and $y$ change. 
			As t varies, it controls the values of xxx and yyy, giving you a way to describe their relationship through a **single degree of freedom**.
				Here, $t$ represents an **axis of control** — even though $x$ and $y$ vary, they are **dependent** on $t$, so we describe the system as having **one degree of freedom**.
#### Parameters and Degrees of Freedom
In parametric systems, a **parameter** represents the **freedom** remaining after constraints have been applied.

- For example, in a system constrained by an equation like x2+y2=r2x^2 + y^2 = r^2x2+y2=r2 (a circle), you no longer have two degrees of freedom because xxx and yyy are related by the equation.
- Instead, you introduce a **parameter** like ttt (which could represent an angle) to describe the remaining degree of freedom. The parameter ttt controls how both xxx and yyy vary together along the circle.
#### Converting Equations into Functions to Define Relationships
Once you have an equation that **constrains** the possible values of variables (i.e., the possibilities on the axes), you can often (but not always) **convert that equation into a function**. 
	When you do this, you're essentially **isolating** one variable (say, $y$) and expressing it as a function of another variable (say, $x$).

- For example, from the equation of a line $\LARGE y=2x+5$, you're expressing $y$ as a function of $x$, which establishes a direct **relationship** between the variables.

In this process, you're not just identifying a set of possibilities (as the equation does) — you're making **explicit the relationship** between those possibilities. 
	The function defines how, for any given value of $x$, there is a corresponding value of $y$, effectively defining the **mapping** between the dimensions (axes).

In parametric design, this is especially powerful because functions allow you to:
1. **Explore** the behavior of systems by varying inputs (independent variables).
2. **Understand** how changes in one variable affect others (dependent variables).
3. **Model** complex relationships in a more dynamic and manipulable way than with equations alone.
#### Equations and Functions in the Context of Axes (Possibilities/Codomains/Axes)
Equations are **static** constraints that describe a condition (like a circle, ellipse, or line) on the possible values of variables in different dimensions. 
	Functions, on the other hand, provide a **dynamic** description of how one dimension varies with another, defining the precise **relationship** between the variables.

So, to summarize the sequence you're describing:
1. **Axes** (or dimensions) are sets of possible values, defining the range of possibilities for each variable.
2. **Equations** impose **constraints** on those possibilities, limiting the combinations of values that can exist together.
3. **Functions** (derived from equations) express the **relationships** between variables, describing how one variable depends on another.