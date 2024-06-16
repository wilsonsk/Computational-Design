---
up:
  - "[[Linear Algebra]]"
related: 
date created: 2024-06-16
---
# Linear Functions
### Foundations of Linear Functions
#### Definition and Basic Form
A linear function is a polynomial function of degree one. 
It is defined by the equation:
$$\LARGE y = mx + b$$

where:
- $y$ is the dependent variable.
- $x$ is the independent variable.
- $m$ is the slope, which represents the rate of change of $y$ with respect to $x$.
- $b$ is the $y$-intercept, the point where the line crosses the $y$-axis.
#### Polynomial Representation
A linear function is a special case of a polynomial function. 
	
Polynomial functions are sums of terms consisting of a variable raised to a non-negative integer power and multiplied by a coefficient.
	In general, a polynomial function of degree $n$ is represented as:
$$\LARGE P(x) = a_n x^n + a_{n-1} x^{n-1} + \ldots + a_1 x + a_0$$

For a linear function, the highest power of $x$ is 1, so it simplifies to:
$$\LARGE P(x) = mx + b$$
#### Characteristics of Linear Functions
1. **Degree**: A linear function is a first-degree polynomial.
2. **Graph**: The graph of a linear function is a straight line.
3. **Slope ($m$)**: Determines the steepness and direction of the line.
4. **Y-Intercept ($b$)**: The point at which the line crosses the $y$-axis.
5. **Additivity and Homogeneity**: Linear functions exhibit the properties of additivity $f(x_1 + x_2) = f(x_1) + f(x_2)$ and homogeneity $f(kx) = kf(x)$.
### Slope as a Scaling Factor
In the equation $y = mx + b$:
- **Slope ($m$)**: Acts as a scaling factor that determines how changes in $x$ affect $y$. If $x$ increases by 1 unit, $y$ changes by $m$ units.
- **Scaling Effect**: The input variable $x$ is scaled by $m$. 
	- For instance, if $m = 2$, every unit increase in $x$ results in a 2-unit increase in $y$.


### Slope as a Rate of Change
In essence, because $y(x)$ is the value being produced, the value of $m$ when either [[Division#Contracting|contracting]] or [[Scaling|scaling]] the input $x$ value (and combining with $b$).
	Therefore, if $m$ is scaling $x$, then that produces a $y$ output value that is larger than $x$ and thus increases at a "faster" rate than $x$.
		if $m$ is contracting $x$, then that produces a $y$ output value that is smaller than $x$ and thus increases at a "slower" rate than $x$.
			This is where the interpretation of $m$ as a slope or "[[#Slope as a Rate of Change|slope as the rate of change]]" comes from. 

In the equation of a linear function:
$$\LARGE y = mx + b$$
The slope $m$ represents the rate of change of $y$ with respect to $x$.
	This means that for each unit increase in $x$, the value of $y$ changes by $m$ units.
###### [[Derivatives|Derivative]] Interpretation
In calculus, the derivative of a function at a given point provides the instantaneous rate of change of the function with respect to one of its variables. 
	For a general function $f(x)$, the derivative $f′(x)$ at a point $x$ is defined as:
$$\LARGE f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$
###### Linear Function and Its Derivative
For a linear function $f(x)=mx+b$:
1. The function is of the form $y=mx+b$.
2. The derivative of this function with respect to $x$ is constant because the function is linear.
###### Calculating the Derivative
Let's calculate the derivative of the linear function $y=mx+b$:
$$\LARGE f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$
Substitute $f(x)=mx+b$:
$$\LARGE f'(x) = \lim_{h \to 0} \frac{m(x + h) + b - (mx + b)}{h}$$
Simplify the expression inside the limit:
$$\LARGE f'(x) = \lim_{h \to 0} \frac{mx + mh + b - mx - b}{h} \LARGE f'(x) = \lim_{h \to 0} \frac{mh}{h} \LARGE f'(x) = \lim_{h \to 0} m \LARGE f'(x) = m$$

Thus, the derivative of the linear function $y=mx+b$ is $m$, which confirms that $m$ is indeed the rate of change of $y$ with respect to $x$.
##### Role of $m$ (Slope) in Transformations
###### 1. Scaling Effect of $m$
The coefficient $m$ determines how the input variable $x$ is scaled to produce the output $y$. 
	Specifically, $m$ indicates the rate of change of $y$ with respect to $x$.
For any point (x,y):
- $x$ is the independent variable (input).
- $y$ is the dependent variable (output), which is calculated using the linear function.
###### 2. Transformation Process
Given an initial point $(x_0,y_0)$:
1. **Initial Point**:
    - Let the initial coordinates be$(x_0, y_0)$.
2. **Applying the Linear Function**:
    - Using the linear equation $y=mx+b$, calculate the new $y$ coordinate based on $x_0$​.
3. **Calculate the New Coordinates**:
    - The new coordinates $(x', y')$ are derived as follows:
        - $x' = x_0$
        - $y' = m x_0 + b$
###### Geometric Interpretation
1. **Slope ($m$)**:
    - The slope mmm represents the rate at which $y$ changes for a unit change in xxx.
    - If $m>1$, the line is steeper, indicating a larger change in $y$ for each unit change in $x$.
    - If $0<m<1$, the line is less steep, indicating a smaller change in $y$ for each unit change in $x$.
    - If $m<0$, the line slopes downward, indicating a negative change in $y$ for each unit change in $x$.
2. **Y-Intercept ($b$)**:
    - The $y$ intercept $b$ shifts the line vertically up or down, depending on its value.
    - This affects the $y$ coordinate of the point after the transformation.
### $B$ as a Coefficient
##### Role of $b$ (Y-Intercept) in Transformations
###### Definition and Basic Role
In the linear function $y=mx+b$:
- $b$ is the $y$ intercept.
- It represents the point where the line crosses the $y$ axis.
###### This means that when $\LARGE x=0$, $\LARGE y=b$.
###### Transforming a Point with $b$
Given an initial point $(x_0, y_0)$:
1. **Initial Point**:
    - The coordinates are $(x_0, y_0)$.
2. **Using the Linear Function**:
    - The equation $y=mx+b$ will be used to transform the point.
3. **Calculate the New Coordinates**:
    - The new coordinates $(x′,y′)$ are derived as follows:
        - $x' = x_0$
        - $y' = m x_0 + b$

This shows that the point $(x_0, y_0)$ is transformed to $(x_0, m x_0 + b)$.
###### Geometric Interpretation
1. **Y-Intercept ($b$)**:
    - The $y$ intercept $b$ shifts the entire line vertically up or down.
    - It does not affect the slope or angle of the line, but it moves the starting point on the $y$axis.
    - This vertical shift means that every point $(x, y)$ on the line is moved up or down by $b$ units.
2. **Impact on Transformation**:
    - When $b>0$, the line shifts up by $b$ units.
    - When $b<0$, the line shifts down by $b$ units.
    - For any $x$, the $y$ coordinate is adjusted by adding $b$.
### Linear Functions in the Context of Secant Lines in Calculus
#### [[Secant Line#Secant Line is a Linear Functions Linear Function|Secant Lines]]
A secant line intersects a curve at two or more points and can be used to approximate the slope of the curve between those points.
	For a function $f(x)$, the slope of the secant line between $(x_1, f(x_1))$ and $(x_2, f(x_2))$ is given by:$$\LARGE m_{\text{sec}} = \frac{f(x_2) - f(x_1)}{x_2 - x_1}$$
#### Relationship to Linear Functions
For a linear function $f(x) = mx + b$:
- Any secant line between two points on this function is identical to the line itself.
- This is because the slope $m$ is constant for all $x$.
### Linear Functions and Derivatives
#### Derivative of a Linear Function
The derivative of a function represents the slope of the tangent line to the curve at any point.
	For a linear function $y = mx + b$, the derivative is:
$$\LARGE f'(x) = m$$

This means that the rate of change of $y$ with respect to $x$ is constant and equal to $m$.
#### Connection with Secant Lines
In calculus, the concept of secant lines leads to the derivative. 
	The slope of the secant line between $x$ and $x + h$ is:
$$\LARGE m_{\text{sec}} = \frac{f(x + h) - f(x)}{h}$$

For a linear function $f(x) = mx + b$, this becomes:
$$\LARGE m_{\text{sec}} = \frac{m(x + h) + b - (mx + b)}{h} = \frac{mx + mh + b - mx - b}{h} = \frac{mh}{h} = m$$

As $h$ approaches 0, the secant line approaches the tangent line, and the slope of the secant line approaches the derivative. 
	For linear functions, the slope of the secant line is always $m$, the same as the slope of the tangent line.