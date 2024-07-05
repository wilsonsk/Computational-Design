# A Map of Change as Rates to Limits of those Rates to Differentials to Derivatives

- - -
### I.e. The Relationship Between the Ave. Rate of Change (i.e. Difference Quotient), the Limit of the Difference Quotient (i.e Differential Ratio) and the Instantaneous Rate of Change (i.e. Derivative)
- - - 
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
### [[Ratio#From Ratio to Rate of Change|From a Ratio to a Rate of Change]]
##### [[Ratio|A Ratio]]
##### [[Ratio#Rate|A Rate (of Change)]]
##### [[Ratio#Average Rate (of change)|An Average Rate (of Change)]]
##### [[Ratio#Instantaneous Rate (of change)|An Instantaneous Rate (of change)]]
 - - - 

## The [[Secant Line|Secant Line]] as a Linear Function Describing the Rate of Change
A secant line is a straight line that intersects a curve (i.e. a non-linear function) at two distinct points. 
	It serves as a linear approximation to the curve over the interval between these two points and provides a geometric way to understand the average rate of change of the function over that interval.

A secant line to the curve $y = f(x)$ at points $x$ and $x+h$ is a line that passes through the points $(x, f(x))$ and $(x+h, f(x+h))$.
## Two Forms of the Secant Line Equation
### 1. Slope-intercept Form (form for all points)
This is the standard linear equation form.
	This form is useful when you know the slope of the line and the y-intercept.
		It directly shows the relationship between $x$ and $y$ for **all points on the line**.
$$\LARGE y = mx+b$$
- m is the slope of the line.
- $b$ is the y-intercept, (i.e. the value of $y$ (i.e. $f(x_0)$) when $x=0$).
- $x$ is the independent input variable value.
### 2. Point-Slope Form (form for a specific point)
This equation represents the linear relationship between the intervals of the independent ($x$ - $x_0$) and dependent ($y$ - $y_0$) variables.
	This form expresses the equation of a line passing through a **specific point** $(x_0, f(x_0))$ with a slope $m$.
$$\LARGE f(x) - f(x_0) = m(x - x_0)$$
- m is the slope of the line.
- $f(x_0)$ is the output value of the function, when $x= x_0$
	- I.e. It is the y-intercept, $b$, the initial value of $y_0$ aka $f(x_0)$ 
- $x$ is the independent input variable value.
### Converting Between the Forms
$$\LARGE f(x) - f(x_0) = m(x - x_0)$$
$$\LARGE = f(x) = m(x - x_0) + f(x_0)$$

- - - 
## Slope, $m$, *of* the Secant Line is the Ratio or Average Rate of Change
### The Slope, $m$
The slope $m$ of a line is defined as the ratio of the vertical change ($\Delta y$) to the horizontal change ($\Delta x$) between any two points on the line.

$$\LARGE m = \frac{\Delta y}{\Delta x}$$

The rate at which the dependent variable changes "with respect to" the independent variable (i.e. how $y$ changes **as** x changes).
	This rate is the average rate of change.
### The [[Ratio|Ratio]]
###### If $\Delta y$ is greater than $\Delta x$
Meaning $y$ changes more rapidly than $x$.
###### If $0<m<1$ , $\Delta y$ is less than $\Delta x$
Meaning $y$ changes less rapidly than $x$.
###### If $m<0$, $\Delta y$ is in the opposite direction to $\Delta x$
Meaning $y$ decreases as $x$ increases.
### [[Derivatives#Difference Quotient I.e. The (Average/Instantaneous) Rate of Change|Average Rate of Change]]
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
#### [[Division#Ratio|Rate]] of Change Example
If a car travels 100 miles in 2 hours, the average speed is: 
$$\LARGE \text{Average Speed} = \frac{100 \text{ miles}}{2 \text{ hours}} = 50 \text{ miles per hour}$$
###### Numerator of the Ratio, $\LARGE \Delta y$
Where $100$ miles is a distance, that is an **interval** between "starting" and "ending" positions.  
	This change in position can be denoted as $\Delta s$, where $s$ represents the position.

The numerator is a [[#Differentials|differential]] of the dependent variable ($f(x)$).
###### Denominator of the Ratio, $\LARGE \Delta x$
Where $2$ hours, is the interval of time, $t$, between "starting" and "ending" time values.
	This change in time can be denoted as $\Delta t$, where $t$ represents time.

The numerator is a [[Derivatives#Differential|differential]] of the independent variable ($x$).

- - -

## [[Division#A Ratio as a Scalar|What it Means to Scale a Constant by a Rate]]


- - - 

## Slope of the Secant Line, $m$ as a Scalar
The slope $m$ can be thought of as a scalar that scales the input variable $x$ to produce the output $y$.
	Depending on the magnitude and sign of $m$, it either scales up (amplifies) or scales down ([[Division#Contracting|contracts]]) the input $x$.
$$\LARGE f(x) = mx +b$$
$$\LARGE m = \frac{\Delta y}{\Delta x}$$
$$\LARGE y = \frac{\Delta y}{\Delta x} \cdot x$$
### If $|\Delta y| > |\Delta x|$, Then $f(x) > x$
###### When the Change in $y$ is Greater than the Change in $x$
$$m = \frac{\Delta y}{\Delta x} > 1$$
This means the output $y$ (or $f(x)$) increases more than the input $x$ when $x$ changes.
	In this case, the slope $m$ scales up the input $x$.

The notion is that the change in $x$ is a fraction of the change in $y$.
### If $|\Delta y| > |\Delta x|$, Then $f(x) < x$
###### When the Change in $y$ is Less than the Change in $x$
$$m = \frac{\Delta y}{\Delta x} < 1$$
This means the output $y$ (or $f(x)$) increases less than the input $x$ when $x$ changes.
	In this case, the slope $m$ scales down (i.e. contracts) the input $x$.

The notion is that the change in $y$ is a fraction of the change in $x$.
## Why Scale the Rate with the Input Variable, $\LARGE x$?
What does this scalar relationship express or represent?
#### An Intuitive Notion: Scaling Relationship the Rate of Change with the Input Value, and its Effect on the Output Value 
$$y = \frac{\Delta y}{\Delta x} \cdot x$$
This "slope" or "ratio" and its relationship as a scalar to the input $x$ and its output product $y$, is just a way of expressing that if...
	Change in $y$ is more then change in $x$, then output $y$ will always be larger than input $x$.
		Or that if a change in $y$ is less then change in $x$, then output $y$ will always be smaller than input $x$.
#### Think About It...
If the change in $y$ is more than the change in $x$, then of course f(x) would be larger relative to the input $x$.
	And this is expressed as the **scaling** effect of $\LARGE \frac{\Delta y}{\Delta x}\cdot x$, where $\Delta y > \Delta x$ and thus $\frac {\Delta y}{\Delta x} > 1$.
	
And if the change in $x$ is more than the change in $y$, then of course f(x) would be smaller relative to the input $x$.
	And this is expressed as the **scaling** effect of $\LARGE \frac{\Delta y}{\Delta x}\cdot x$, where $\Delta y < \Delta x$ and thus $\frac {\Delta y}{\Delta x} < 1$.

- - - 
## Normalizing the Independent Variable, $\LARGE x$ by $\LARGE \Delta x$
Focusing on how $x$ is scaled by the slope of the Secant Line, $m$.
$$\LARGE y = \frac{\Delta y}{\Delta x} \cdot x$$

The process of scaling $x$ by this ratio, involves dividing $\LARGE x$ by the $\LARGE \Delta x$.
	And then subsequently multiplying this quotient, $\LARGE \frac{x}{\Delta x}$ by $\LARGE \Delta y$.
### Normalizing 
Normalization is the process of adjusting values measured on different scales to a common scale, often to make comparisons or computations easier.
	In the context of the ratio $\frac{x}{\Delta x}$​, normalization involves expressing $x$ in terms of the unit change $\Delta x$.

This ratio, $\LARGE \frac{x}{\Delta x}$, (dividing the input value $x$ by the change in $x$), can be interpreted as the number of times the unit change $\Delta x$ fits into the value $x$.
### How $\LARGE \Delta x$ Affects $\LARGE x$ and Therefore, $\LARGE f(x)$
##### If $\LARGE \Delta x = 1$
$$\LARGE \frac{x}{\Delta x} = \frac{x}{1} = x$$
$$\LARGE \text{Normalizing $x$ by $\Delta x = 1$ does not change the value of $x$.}$$
$$\LARGE \text{The output $\LARGE f(x)$ is directly proportional to the slope.}$$
#### If $\LARGE \Delta x > x$
$$\LARGE \text{Then} \space \frac{x}{\Delta x} < 1 \space \text{and that scaling} \space $$
$$\LARGE \text{The value of x is contracted}$$
$$\text{The output f(x) will be reduced relative to x, depending on the slope} \frac{\Delta y}{\Delta x}$$
#### If $\LARGE \Delta x < x$ 
$$\LARGE \text{Then} \space \frac{x}{\Delta x} > 1$$
$$\LARGE \text{The value of x is scaled}$$
$$\text{The output f(x) will be increased relative to x, depending on the slope} \frac{\Delta y}{\Delta x}$$


- - - 

## Slope of the Secant Line, $m$ is the [[Derivatives#Difference Quotient I.e. The (Average/Instantaneous) Rate of Change|Difference Quotient]]
### Difference Quotient
The difference quotient is a formula used to calculate the average rate of change of a function over a specified interval. 
	I.e. The difference quotient measures the average rate of change of a function, $f(x)$ over an interval, $h$.

For a function $f(x)$, the difference quotient between two points $(x, f(x))$ and $(x+h,f(x+h))$ is given by the slope of the secant line. 
		$$\LARGE m = \frac{\Delta f(x)}{\Delta x} = \text{Difference Quotient} = \frac{f(x+h) - f(x)}{h}$$
		$$\LARGE \Delta y = f(x + h) - f(x)$$
		$$\LARGE \Delta x = h$$
- $f(x)$ is the value of the function at point $x$.
- $f(x+h)$ is the value of the function at point $x+h$.
- $h$ is the change in the independent variable $x$.​

- - -

## Finite vs. Infinitesimal Changes
#### Finite Changes
$\Delta x$ and $\Delta y$
Refer to measurable, non-zero changes in the value of a variable over a specific interval.

**Example**: 
$$\LARGE m = \frac{\Delta y}{\Delta x}$$$$\LARGE \Delta y = f(x + h) - f(x)$$
$$\LARGE \Delta x = h$$
#### Infinitesimally Small Changes
$\LARGE dx$ and $\LARGE dy$
Are changes that are so small they approach zero but are not exactly zero. 
	These are used in the context of calculus to understand the behavior of functions at an extremely small scale.

For infinitesimal changes, as $h$ approaches zero, $\Delta y$ becomes $dy$ and $\Delta x$ becomes $dx$.
$$\LARGE \text{Limit Definition} = dy = \lim_{h \to 0}​(f(x+h)−f(x))$$
$$\LARGE \text{Limit Definition} = dx = \lim_{h \to 0}h$$
**Example**: 
For a function $y=f(x)$, the differential $dx$ represents an infinitesimally small change in $x$, and $dy$ represents the corresponding infinitesimally small change in $y$.
## Differentials
Differentials are infinitesimally small changes in variables.
	In calculus, differentials help us understand how small changes in one variable affect another variable.

The differential of $x$ is denoted as $dx$.
The differential of $y$, when $y=f(x)$, is denoted as $dy$.

They are not called differentials unless we are considering the limit as these changes become infinitesimally small.
#### Differential Form
The differential form is a mathematical representation that describes how small changes in an independent variable result in changes in a dependent variable. 

For a function $y=f(x$), the differential form is given by:
$$\LARGE dy = f'(x) \, dx \space \text{and} \space dx = \frac{dy}{f'(x)}$$
Where $f′(x)$ is the derivative of $f(x)$ with respect to $x$ (i.e. as $x$ changes).

---

## The *Limit* of the Difference Quotient as the Differential Ratio (i.e. the Derivative)
### [[Limits|Limits]]
A limit examines the behavior of a function as the input approaches a certain value.

$$\LARGE \lim_{h \to 0} f(x+h)$$
### Limit of the Difference Quotient is the Differential Ratio aka the [[Derivatives|Derivative]]
$$\LARGE f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$
Where $h$ is a small increment in $x$.​

As $h$ approaches zero, the secant line approaches the tangent line at $x$, and the difference quotient becomes the instantaneous rate of change, or the derivative.
### The Limit of the Difference Quotient is the Derivative Which is Itself the Ratio of Differentials
$$\LARGE \lim_{h \to 0} \frac{f(x+h) - f(x)}{h} = f'(x) =\frac{dy}{dx}$$
##### Limit Form
$$\LARGE \text{Differential y} =  dy = \lim_{h \to 0}​(f(x+h)−f(x))$$
$$\LARGE \text{Differential x} = dx = \lim_{h \to 0}h$$
##### Differential Form
$$\LARGE dy = \frac{dy}{dx}$$
$$\text{And}$$
$$\LARGE dx = \frac{dy}{(\frac{dy}{dx})}$$
$$\LARGE == dy = f'(x) \, dx \space \text{and} \space dx = \frac{dy}{f'(x)}$$
*This is similar to the Slope, $m$ of the Secant Line*
$$\LARGE m = \frac{\Delta y}{\Delta x}$$
$$\LARGE y = mx$$

---

## [[Derivatives]]


---

## [[Partial Derivatives|Partial Derivatives]]