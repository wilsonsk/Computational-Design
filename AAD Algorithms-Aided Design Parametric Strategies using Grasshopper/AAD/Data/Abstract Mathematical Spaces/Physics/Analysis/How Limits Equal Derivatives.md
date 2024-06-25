# Understanding the Relationship Between Limits, Difference Quotients, Derivatives, and Differentials
##### [[Division#Ratio|Rate]] of Change Example
If a car travels 100 miles in 2 hours, the average speed is: 
$$\LARGE \text{Average Speed} = \frac{100 \text{ miles}}{2 \text{ hours}} = 50 \text{ miles per hour}$$
###### Numerator of the Ratio
Where $100$ miles is a distance, that is an **interval** between "starting" and "ending" positions.  
	This change in position can be denoted as $\Delta s$, where $s$ represents the position.

The numerator is a [[Derivatives#Differential|differential]] of the dependent variable ($f(x)$).
###### Denominator of the Ratio
Where $2$ hours, is the interval of time, $t$, between "starting" and "ending" time values.
	This change in time can be denoted as $\Delta t$, where $t$ represents time.

The numerator is a [[Derivatives#Differential|differential]] of the independent variable ($x$).

---
## The Concept of Change
Change refers to the variation in the value of a quantity over time, space, or any other dimension. 
	It is a fundamental aspect of understanding dynamic systems.
### Functions as Descriptions of Change
Functions are mathematical models that describe how one quantity changes with respect to another.
	$f(x) = x^2$ describes how the output $f(x)$ changes as the input $x$ changes.

In the context of a function $f(x)$, for each input $x$, the function produces an output $f(x)$.
	The coordinates $(x,y)$ can be represented as $(x,f(x))$ where $y=f(x)$.

**Independent Variable**: $x$
    - The input value to the function.
    - It is plotted on the horizontal axis of a graph.
**Dependent Variable**: $y$ or $f(x)$
    - The output value of the function, which depends on the input $x$.
    - It is plotted on the vertical axis of a graph.
### The [[Secant Line|Secant Line]] as a Linear Function Describing the Rate of Change
A secant line is a straight line that intersects a curve (i.e. a non-linear function) at two distinct points. 
	It serves as a linear approximation to the curve over the interval between these two points and provides a geometric way to understand the average rate of change of the function over that interval.

A secant line to the curve $y = f(x)$ at points $x$ and $x+h$ is a line that passes through the points $(x, f(x))$ and $(x+h, f(x+h))$.
#### Two Forms of the Secant Line Equation
###### 1. Slope-intercept Form (form for all points)
This is the standard linear equation form.
	This form is useful when you know the slope of the line and the y-intercept.
		It directly shows the relationship between $x$ and $y$ for **all points on the line**.
$$\LARGE y = mx+b$$
- m is the slope of the line.
- $b$ is the y-intercept, (i.e. the value of $y$ (i.e. $f(x)$) when $x=0$).
- $x$ is the independent input variable value.
###### 2. Point-Slope Form (form for a specific point)
This equation represents the linear relationship between the intervals of the independent ($x$ - $x_0$) and dependent ($y$ - $y_0$) variables.
	This form expresses the equation of a line passing through a **specific point** $(x_0, f(x_0))$ with a slope $m$.
$$\LARGE f(x) - f(x_0) = m(x - x_0)$$
##### Converting Between the Forms
$$\LARGE f(x) - f(x_0) = m(x - x_0)$$
$$\LARGE = f(x) = m(x - x_0) + f(x_0)$$
### Slope, $m$, *of* the Secant Line is the Ratio or Average Rate of Change
#### The Slope, $m$
The slope $m$ of a line is defined as the ratio of the vertical change ($\Delta y$) to the horizontal change ($\Delta x$) between any two points on the line.

$$\LARGE m = \frac{\Delta y}{\Delta x}$$

The rate at which the dependent variable changes "with respect to" the independent variable (i.e. how $y$ changes **as** x changes).
	This rate is the average rate of change.
##### [[Derivatives#Difference Quotient I.e. The (Average/Instantaneous) Rate of Change|Average Rate of Change]]
The average rate of change of a function between two points provides a measure of how the function's output (the dependent variable) changes on average for each unit change in the input (the independent variable).
	I.e. Measures how much the output of a function changes on average for a given change in the input.

*Remember*: 
$$ \text{Average}= \frac{\text{Sum of Values}}{\text{Total Number of Values}}$$
###### $\LARGE \Delta y$ ("sum of values")
Is similar to the sum of the changes in $y$ values.

It represents the total change in the function's value over the interval $[x,x+h]$. 
	This is analogous to the "sum of values" because it represents the overall change in $y$.
###### $\LARGE \Delta x$ ("total number of values")
Is similar to the total number of intervals or units over which the change is averaged.

It represents the interval length over which the change occurs. 
	This is analogous to the "total number of values" because it is the span over which the change in $y$ is averaged.
### Slope of the Secant Line is the [[Derivatives#Difference Quotient I.e. The (Average/Instantaneous) Rate of Change|Difference Quotient]]
##### Difference Quotient
The difference quotient is a formula used to calculate the average rate of change of a function over a specified interval. 
	I.e. The difference quotient measures the average rate of change of a function over an interval.

For a function $f(x)$, the difference quotient between two points $x$ and $x+h$ is given by
The slope of the secant line is given by the difference quotient: 
		$$\LARGE m = \text{Difference Quotient} = \frac{f(x+h) - f(x)}{h}$$
- $f(x)$ is the value of the function at point $x$.
- $f(x+h)$ is the value of the function at point $x+h$.
- $h$ is the change in the independent variable $x$.​
### Differentials
##### Finite vs. Infinitesimal Changes
###### Finite Changes
$\Delta x$ and $\Delta y$
Refer to measurable, non-zero changes in the value of a variable over a specific interval.
**Example**: 
If $x$ changes from $x_1$​ to $x_2$​.
Then: $\Delta x = x_2 - x_1$
###### Infinitesimally Small Changes
$dx$ and $dy$
Are changes that are so small they approach zero but are not exactly zero. 
	These are used in the context of calculus to understand the behavior of functions at an extremely small scale.
**Example**: 
For a function $y=f(x)$, the differential $dx$ represents an infinitesimally small change in $x$, and $dy$ represents the corresponding infinitesimally small change in $y$.
##### Differentials
Differentials are infinitesimally small changes in variables.
	In calculus, differentials help us understand how small changes in one variable affect another variable.

The differential of $x$ is denoted as $dx$.
The differential of $y$, when $y=f(x)$, is denoted as $dy$.

They are not called differentials unless we are considering the limit as these changes become infinitesimally small.
### Difference Quotients vs. Derivatives

---

#### Section 3: Limits and the Transition to the Derivative

- **Objective**: To explore the concept of limits and how the difference quotient leads to the derivative.

##### 3.1 Introduction to Limits

- **Definition**: A limit examines the behavior of a function as the input approaches a certain value.
- **Example**: lim⁡h→0f(x+h)\lim_{h \to 0} f(x+h)h→0lim​f(x+h)

##### 3.2 Connecting Limits to the Difference Quotient

- **Limit of the Difference Quotient**: f′(x)=lim⁡h→0f(x+h)−f(x)hf'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}f′(x)=h→0lim​hf(x+h)−f(x)​
- **Interpretation**: As $h$ approaches zero, the secant line approaches the tangent line at $x$, and the difference quotient becomes the instantaneous rate of change, or the derivative.

---

#### Section 4: The Derivative

- **Objective**: To understand the derivative as the limit of the difference quotient and its geometric and practical significance.

##### 4.1 Definition and Notation

- **Derivative**: The instantaneous rate of change of a function at a point.
- **Formula**: f′(x)=lim⁡h→0f(x+h)−f(x)hf'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}f′(x)=h→0lim​hf(x+h)−f(x)​

##### 4.2 Geometric Interpretation

- **Tangent Line**: The line that just touches the curve at a point and has the same slope as the curve at that point.
- **Slope of the Tangent Line**: The derivative $f'(x)$ represents the slope of the tangent line to the curve at $x$.

---

#### Section 5: Differentials

- **Objective**: To introduce differentials and their relationship to derivatives and the difference quotient.

##### 5.1 Understanding Differentials

- **Differential Notation**:
    - **$dx$**: Infinitesimally small change in the independent variable.
    - **$dy$**: Infinitesimally small change in the dependent variable.

##### 5.2 Connecting Differentials to the Difference Quotient

- **As $h$ Approaches Zero**:
    - **Numerator ($f(x+h) - f(x)$)** becomes $dy$, the differential of the dependent variable.
    - **Denominator ($h$)** becomes $dx$, the differential of the independent variable.
- **Derivative in Differential Form**: f′(x)=dydxf'(x) = \frac{dy}{dx}f′(x)=dxdy​

---

#### Section 6: Summary and Intuitive Understanding

- **Objective**: To consolidate understanding and highlight the intuitive connections between the key concepts.

##### 6.1 Summary

- **Difference Quotient**: Measures the average rate of change (slope of the secant line).
- **Limit**: Process of making the interval $h$ approach zero.
- **Derivative**: Instantaneous rate of change (slope of the tangent line).
- **Differentials**: Infinitesimally small changes in the independent and dependent variables.

##### 6.2 Intuitive Understanding

- **Average vs. Instantaneous Rate of Change**: The difference quotient gives the average rate of change, while the derivative gives the instantaneous rate of change as the interval shrinks to zero.
- **Geometric Connection**: The transition from secant line to tangent line through the limit process.