# Functions and Motion
### How Different Types of Functions Affect the Trajectory of Moving Objects

The type of function that describes the position of a moving object over time influences the object's trajectory. 

Each type of function provides a different model of motion, resulting in distinct paths and behaviors.
### How Scaling the Input Variable Affects the Output Values and Creates Specific Patterns
The nature of the function used to describe the relationship between the input variable $x$ and the output $y$ determines the pattern of the output values.
	This is because different functions scale the input variable in different ways, affecting the growth rate and curvature of the output.
#### Fundamental Theorem of Algebra
The Fundamental Theorem of Algebra states that a polynomial of degree $n$ has exactly $n$ roots (solutions) in the complex number system, counting multiplicity.
    Therefore, a polynomial of degree $n−1$ (the derivative of the original polynomial) can have at most $n−1$ real roots.
#### Inflection Point
An inflection point of a function is a point where the concavity of the function changes.
	This means the function changes from being concave up (convex) to concave down (concave) or vice versa.
###### Mathematical Condition
At an inflection point, the second derivative $f′′(x) =0$ changes sign around that point.
###### Behavior
The concavity of the function changes, but it does not necessarily involve a change from increasing to decreasing or vice versa.

For a polynomial of degree $n$:
- The maximum number of inflection points is $n−2$.

This means:
- A linear function ($n=1$) has no inflection points.
- A quadratic function ($n=2$) has no inflection points.
- A cubic function ($n=3$) can have at most 1 inflection point.
- A quartic function ($n=4$) can have at most 2 inflection points.
#### Turning Point
A turning point of a function is a point where the function changes direction from increasing to decreasing or vice versa.
	It is also referred to as a [[Derivatives#Local Maximum|local maximum]] or [[Derivatives#Local Minimum|local minimum]].
##### Increasing and Decreasing Functions
###### Increasing Function
A function $\LARGE f(x)$ is said to be increasing on an interval if, as $x$ moves from left to right (i.e., as $x$ increases), the $y$-values $(f(x)$) also increase. 
	I.e. The function's graph goes up as $x$ increases.

Mathematically, $f(x)$ is increasing on an interval if for any two points $x_1$​ and $x_2$​ within the interval, $x_1 < x_2$ implies $f(x_1) < f(x_2)$.
###### Decreasing Function
A function $f(x)$ is said to be decreasing on an interval if, as $x$ moves from left to right, the $y$-values ($f(x)$) decrease. 
	I.e. The function's graph goes down as $x$ increases.

Mathematically, $f(x)$ is decreasing on an interval if for any two points $x_1$​ and $x_2$​ within the interval, $x_1 < x_2$​ implies $f(x_1) > f(x_2)$.
###### Mathematical Condition
At a turning point, the first derivative $f′(x)= 0$.
##### Behavior
The function changes from increasing to decreasing (local maximum) or from decreasing to increasing (local minimum).

For a polynomial of degree $\LARGE n$:
- The maximum number of turning points is $\LARGE n−1$.
##### Polynomial Functions and Turning Points
The degree of a polynomial function is the highest power of the variable $x$ in the polynomial.
###### The Order (i.e. highest power) of a Function Determines the Number of Curves
This means:
- A linear function ($n=1$) has no turning points.
- A quadratic function ($n=2$) can have at most 1 turning point.
- A cubic function ($n=3$) can have at most 2 turning points.
- A quartic function ($n=4$) can have at most 3 turning points.
### 1. Linear Functions
A linear function is of the form:
$$\LARGE x(t) = at + b$$

where $a$ and $b$ are constants.

**Scaling**: The output $y$ changes linearly with $x$. 
	For each unit increase in $x$, $y$ increases by a constant amount $a$.

**Pattern**: The graph is a straight line, reflecting a constant rate of change.

- **Trajectory**: The trajectory is a straight line because the function increases or decreases at a constant rate.
- **Maximum Number of Turning Points:** $\LARGE n-1$
	$$n = 1 \quad ; \text{max number of turning points} = \quad 1-1 = 1$$
- **Maximum Number of Inflection Points**: $\LARGE n-2$
	$$n = 1 \quad ; \text{max number of inflection points} = 1-2 = N/A$$
- **Velocity**: Constant $v(t) = a$
- **Acceleration**: Zero $a(t) = 0$
- **Example**: A car moving at a constant speed on a straight road.
### 2. Quadratic Functions
A quadratic function is of the form:
$$\LARGE x(t) = at^2 + bt + c$$
where $a$, $b$, and $c$ are constants.

**Scaling**: The output $y$ changes quadratically with $x$.
	As $x$ increases, $y$ increases by an amount proportional to x2x^2x2. 
		This means that small changes in $x$ can produce larger changes in $y$ as $x$ grows.

**Pattern**: The graph is a parabola, reflecting a rate of change that increases or decreases depending on the value of $x$.

- **Trajectory**: The trajectory is parabolic because the position changes at a rate that itself changes linearly (velocity).
- **Maximum Number of Turning Points:** $\LARGE n-1$
	$$n = 2 \quad ; \text{max number of turning points} = \quad 2-1 = 1$$
- **Maximum Number of Inflection Points**: $\LARGE n-2$
	$$n = 2 \quad ; \text{max number of inflection points} = \quad 2-2 = 0$$
- **Velocity**: Linearly increasing or decreasing $v(t) = 2at + b$
- **Acceleration**: Constant $a(t) = 2a$
- **Example**: A projectile under the influence of gravity (ignoring air resistance).
### 3. Cubic Functions
A cubic function is of the form:
$$\LARGE x(t) = at^3 + bt^2 + ct + d$$

where $a$, $b$, $c$, and $d$ are constants.

**Scaling**: The output $y$ changes cubically with $x$. 
	As $x$ increases, $y$ increases by an amount proportional to x3x^3x3. 
		This introduces more complexity, with the output values changing at varying rates depending on $x$.

**Pattern**: The graph can have inflection points and multiple curves, reflecting a more complex relationship between $x$ and $y$.

- **Trajectory**: The trajectory is more complex with potential inflection points where the curvature changes direction.
- **Maximum Number of Turning Points:** $\LARGE n-1$
	$$n = 1 \quad ; \text{max number of turning points} = \quad 3-1 = 2$$
- **Maximum Number of Inflection Points**: $\LARGE n-2$
	$$n = 1 \quad ; \text{max number of inflection points} = 3-2 = 1$$
- **Velocity**: Quadratic $v(t) = 3at^2 + 2bt + c$
- **Acceleration**: Linearly changing $a(t) = 6at + 2b$
- **Example**: More complex mechanical systems with varying forces.
### 4. Higher-Order Polynomials
Higher-order polynomial functions are of the form:
$$\LARGE x(t) = a_n t^n + a_{n-1} t^{n-1} + \cdots + a_1 t + a_0$$

**Scaling**: The output $y$ changes according to the highest power of $x$ present in the function. 
	Higher powers of $x$ lead to more dramatic changes in $y$ as $x$ grows, with increasing complexity in the graph's shape.

**Pattern**: The graph has multiple points of inflection and curvature changes, reflecting the polynomial's degree.

- **Trajectory**: The object's path becomes increasingly complex with more [[Derivatives#Inflection Points|points of inflection]] and changes in curvature as the degree of the polynomial increases.
- **Maximum Number of Turning Points:** $\LARGE n-1$
- **Maximum Number of Inflection Points**: $\LARGE n-2$
- **Velocity**: The derivative of the polynomial, resulting in a polynomial of one degree lower.
- **Acceleration**: The second derivative of the polynomial, resulting in a polynomial of two degrees lower.
- **Example**: Complicated systems with multiple forces acting in various ways.
### 5. Exponential Functions
An exponential function is of the form:
$$\LARGE f(x) = a e^{bx}$$

where $a$ and $b$ are constants.

**Scaling**: The output $y$ changes exponentially with $x$. 
	For each unit increase in $x$, $y$ increases by a factor of $e^b$.
		This leads to rapid growth or decay.

**Pattern**: The graph shows exponential growth or decay, with $y$ increasing or decreasing rapidly as $x$ changes.

- **Trajectory**: The object’s position changes exponentially, either increasing or decreasing rapidly.
- **Example**: Population growth, radioactive decay, or charging of a capacitor.
- **Velocity**: Exponential $v(t) = ab e^{bt}$
- **Acceleration**: Exponential $a(t) = ab^2 e^{bt}$
## Curve Fitting 
If you have a curve (a set of data points or a graphical representation of a trajectory), you can find a function that fits it.
	This process is known as **curve fitting**. 
		There are several methods and tools available for this purpose, depending on the nature of your data and the type of function you wish to fit.
### Methods of Curve Fitting

1. **Polynomial Regression**:
    - Fits a polynomial function to the data points.
    - Useful for curves that can be approximated by polynomials.
2. **Least Squares Method**:
    - Minimizes the sum of the squares of the differences between the observed and predicted values.
    - Can be applied to linear and nonlinear functions.
3. **Spline Interpolation**:
    - Fits piecewise polynomials (splines) to the data.
    - Useful for fitting curves that need to pass through all data points smoothly.
4. **Exponential and Logarithmic Regression**:
    - Fits exponential or logarithmic functions to the data.
    - Useful for data that grows or decays exponentially.
5. **Fourier Transform**:
    - Decomposes a function into its constituent sine and cosine waves.
    - Useful for periodic data.
6. **Nonlinear Regression**:
    - Fits more complex, non-linear models to the data.
    - Can handle a wide variety of functions, including those not easily represented by polynomials.
#### Steps to Find a Function that Fits a Curve

1. **Collect Data Points**:
    - Gather the (x,y)(x, y)(x,y) coordinates of the curve.
2. **Choose a Model**:
    - Decide on the type of function (linear, polynomial, exponential, etc.) that you believe best fits the data.
3. **Apply a Fitting Method**:
    - Use a fitting method (e.g., least squares) to find the coefficients of the function.
4. **Evaluate the Fit**:
    - Assess the goodness of fit using metrics such as R2R^2R2 (coefficient of determination), residuals, or root mean square error (RMSE).