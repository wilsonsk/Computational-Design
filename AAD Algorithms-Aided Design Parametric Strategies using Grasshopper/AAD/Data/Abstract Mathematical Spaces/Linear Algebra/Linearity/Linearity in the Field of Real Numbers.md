# Linearity in the [[Abstract Mathematical Spaces#The Role of Composite Spaces in Inheritance and Extension Building on the Foundation Generating Vector Spaces *on Top of* the Real Number Field|Field of Real Numbers]]
Linearity in $\mathbb{R}$ is a natural consequence of the field's algebraic properties and its geometric interpretation. 
	Linear functions and equations arise from the basic operations of addition and multiplication within $\mathbb{R}$ and their corresponding graphical representations as straight lines. 
		The completeness and continuity of $\mathbb{R}$ support the well-defined nature of linear relationships, making $\mathbb{R}$ a fundamental setting for studying linearity.
### Field of Real Numbers
The [[Abstract Mathematical Spaces#The Sequential Generation of the Field of Real Numbers and the Vector Space Fields (i.e. Algebraic Fields)|field]] of real numbers $\mathbb{R}$ is a set equipped with two operations: addition and multiplication. 
	These operations satisfy the properties of associativity, commutativity, distributivity, existence of identity elements (0 for addition and 1 for multiplication), and the existence of inverse elements.

The field of real numbers $\mathbb{R}$ is complete and continuous, meaning it contains all limit points of sequences of real numbers. 
	This allows for the smooth and uninterrupted behavior of linear functions.

Real numbers provide a way to scale and direct magnitudes. 
	The homogeneity property ($f(cx) = cf(x)$) relies on the ability to scale inputs by any real number $c$.
## Linear Relationship
A linear relationship between two variables is one in which the **change** in the dependent variable ($y$) is directly proportional to the **change** in the independent variable ($x$), plus a constant.
	This is described by the [[#Constant of Proportionality (i.e. Constant Rate of Change)|Constant of Proportionality]]
## Linearity (for the Field of Real Numbers)
"Linearity" and "linear relationship" refer to the same concept in mathematics.
	Linearity in the field of real numbers refers to the property of a mathematical relationship or function that can be described by a linear equation.
		This means that the relationship between two variables can be represented by a straight line when plotted on a graph.
			Linearity generally refers to a relationship that can be represented by a linear equation of the form $y = mx + b$, where $m$ is the slope and $b$ is the y-intercept.
				Linearity also refers to the property of a function or relationship where the output changes at a constant rate with respect to the input.
### The Linearity Properties 
These properties are directly related to the algebraic structure of $\mathbb{R}$.
	The defining characteristics of linearity for the Field of Real Numbers.
		Or more generally for any field of scalars.

For a function $f: \mathbb{R} \to \mathbb{R}$ to be linear, it must satisfy the following conditions:
#### 1. Proportionality of Linearity
The proportionality property of linearity refers to the characteristic of a linear relationship where the dependent variable **changes** at a constant rate with respect to the independent variable.
	The proportionality property of linearity is fundamentally about a constant rate of change between two variables.
		Specifically, this property indicates that the relationship between $y$ and $x$ can be expressed by a linear equation of the form:
$$\LARGE y = mx +b$$
"The proportionality property of linearity indicates that the dependent variable $y$ changes at a constant rate with respect to the independent variable $x$, as described by the equation $y=mx+b$. Here, $m$ represents the constant rate of change, and $b$ is the y-intercept, providing a linear relationship between $y$ and $x$."

Proportionality of Linearity is **not** the same thing as [[#Direct Proportionality (a "Special Case" of Linear Relationships)|Direct Proportionality]].
##### Constant of Linear Proportionality is a Constant Rate of Change ($\LARGE m$)
The constant $m$ is the slope, which represents the rate of change of $y$ with respect to $x$, but there is an additional offset $b$.
	This represents the change in $y$ divided by the change in $x$.
$$\LARGE \text{For } y = mx + b, \space m = \frac{\Delta y}{\Delta x}$$
The constant of proportionality is a fixed value that relates the input and output variables in a directly proportional relationship.
	The dependent variable $y$ changes at a constant rate with respect to the independent variable $x$. 
		This rate is given by the slope $m$. 
			For every unit increase in $x$, $y$ changes by $m$ units.
				The constant of proportionality ($\LARGE m$ in $\LARGE y = mx$) determines the rate at which the output changes with respect to the input.
					$m$ is the constant of proportionality that scales the input $x$ to produce the output $y$.
						The Rate of Change remains constant regardless of the value of the y-intercept $b$.

The rate of change is a measure of how one quantity changes in response to changes in another quantity. 
##### [[Division#Division as a Proportional Relationship (i.e. Direct Proportionality)|Direct Proportionality]] (a "Special Case" of Linear Relationships)
*Is a "Special Case" where* $\LARGE b = 0 \text{ in } y = mx + b$ 
	The output (dependent variable) changes in direct proportion to the input (independent variable) that is being scaled by a constant of proportionality.

###### Think About it...
If 10 = a \cdot 5 where a = 2, then 10 is 2 times 5 and 5 is 1 half 10 meaning that it requires 2 5's to equal 10.  
###### Constant of Direct Proportionality is a Constant Ratio ($\LARGE k$)
$$\LARGE y = kx$$
This ratio compares the values of $y$ and $x$ directly.

The ratio or rate of the two quantities remains constant. 
	Direct proportionality means that if $\LARGE k$ is the constant of proportionality and $b=0$, then $\LARGE y$ is directly proportional to $\LARGE x$, and the ratio $\LARGE \frac{y}{x}$ remains constant. 
		If $\LARGE y = kx$, then $\LARGE k = \frac{y}{x}$ for all values of $\LARGE x$ and $\LARGE y$ in the relationship.
			The graph of a directly proportional relationship between two variables is a straight line that passes through the origin (0,0).

The constant of proportionality, $k$ can be a ratio or a rate.
	The constant is specifically the constant of proportionality, and it directly links $y$ and $x$ without any offset.

If $b \neq 0 \text{ in } y=mx+b$, $y$ is not directly proportional to $x$ because the y-intercept $b$ introduces a constant term that shifts the line vertically.
	This means the ratio $\frac{y}{x}$​ is not constant for all $x$.
		This is called a linear relationship.
#### 2. Linearity of the Equation
The general form of a linear equation in two variables is $ax + by = c$, where $a$, $b$, and $c$ are constants.
	The graph of such an equation is a straight line.
#### 3. Additivity
The function $f$ satisfies the property $f(x + y) = f(x) + f(y)$ for all $x$ and $y$ in the domain.
$$\LARGE f(x + y) = f(x) + f(y) \text{ for all } x, y \in \mathbb{R}$$

***Example***: The function $f(x) = ax$, where $a \in \mathbb{R}$, satisfies these conditions:
$$\LARGE 
f(x + y) = a(x + y) = ax + ay = f(x) + f(y)
$$
#### 4. Homogeneity (of Degree 1)
The function $f$ satisfies the property $f(kx) = kf(x)$ for all real numbers $c$ and all $x$ in the domain.
$$\LARGE f(kx) = kf(x) \text{ for all } x \in \mathbb{R} \text{ and }k \in \mathbb{R}$$

***Example***: The function $f(x) = ax$, where $a \in \mathbb{R}$, satisfies these conditions:
$$\LARGE 
f(kx) = a(kx) = k(ax) = kf(x)
$$

This confirms that $f(x) = ax$ is a linear function in the field of real numbers.
## Linear Scaling
A scaling with no exponents or with one term having an exponent of 1 (like $\LARGE a \cdot b^1$) is indeed a linear scaling.
	Where  one terms is considered a "constant".
		This is an example of a **direct proportion**.
## Linear Functions/Equations
A linear equation in one variable has the form $ax + b = 0$, where $a$ and $b$ are real numbers, and $a \neq 0$.
	Solving this equation involves operations within $\mathbb{R}$.

Extending to two variables, a linear equation has the form $ax + by = c$, where $a$, $b$, and $c$ are real numbers.
	The set of solutions to this equation forms a straight line in the Cartesian plane.