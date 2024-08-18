---
up:
  - "[[Dynamics Analysis]]"
related:
  - "[[Data Operations]]"
  - "[[SubD Surface Patterns]]"
  - "[[Curves]]"
  - "[[Notion of Surface Curvature]]"
  - "[[Numbers]]"
  - "[[Points]]"
  - "[[Data Relationships]]"
date created: 2024-04-10
---
*Refer to this Map for a detailed map of the relational structure:* [[A Map of Change as Rates to Limits of those Rates to Differentials to Derivatives]]
##### *A Note on [[Mapping#A Function as a Subset of Mappings ($1 1$, $m 1$)|Functions]]*
Derivatives ***themselves*** are a type of function that measure the rate at which ***another*** function's output changes with respect to its input.
	These "**input functions**" of Derivative functions, can be any [[Mapping#Output Types of Functions|type]], from Scalar Functions, to Vector-Valued, Matrix-Valued, Complex-Valued Functions, etc.
# Derivatives
The Rate of Change of a Function's Output Value, as one Input Variable Changes.

The **derivative** of a function, $f(x)$, measures the rate at which the function's output value changes as its input changes. 
	It is a fundamental concept in calculus, representing an instantaneous rate of change.

For a function $f(x)$, the derivative at a point $x$ is defined as the limit of the average rate of change of the function as the interval $\Delta x$ approaches zero.

Mathematically, the derivative of $f$ at $x$, denoted $f'(x)$ or $\frac{df}{dx}$, is given by:
$$f'(x) = \lim_{\Delta x \to 0} \frac{f(x + \Delta x) - f(x)}{\Delta x}$$
#### Interpretation
- **Rate of Change**: The derivative represents the rate at which $f(x)$ changes with respect to $x$.
- **Slope of the Tangent Line**: Geometrically, $f'(x)$ is the slope of the tangent line to the graph of $f$ at the point $(x, f(x))$.
## Notation
The derivative can be notated in various ways, including:
## $\LARGE f'(x)$
## $D_x f(x)$
# $\LARGE \frac{d}{dx}$
The notation $\LARGE \frac{d}{dx}$​ is an operator, specifically the differentiation operator with respect to the variable $x$.
	It requires a function to act upon.
It does not specify any particular function, it just indicates the operation of taking a derivative with respect to $x$.
	When you see $\LARGE \frac{d}{dx}$​ by itself, it means "take the derivative with respect to $x$."
		It is not complete by itself and needs a function or expression to operate on.
*For example*, $\LARGE \frac{d}{dx}(x^2)$ means to take the derivative of $x^2$ with respect to $x$.
	It is an instruction to differentiate
# $\LARGE \frac{df}{dx}$ 
This generally means the derivative of some function $f$ with respect to $x$.
Here, $f$ is an unspecified function of $x$.
	The exact form of $f(x)$ is not specified when you just write $\LARGE \frac{df}{dx}$.
It is the result of applying the operator $\LARGE \frac{d}{dx}$​ to a specific function $f(x)$.
This represents the derivative of a specific function $f(x)$ with respect to $x$. 
	It is the result of applying $\LARGE \frac{d}{dx}$​ to $f(x)$.
		It is the actual derivative of a specific function $f(x)$.
##### $$\LARGE \frac{df}{dx}x^2 \text{ vs. } \frac{d}{dx}x^2$$
$$\LARGE \frac{d}{dx}x^2 $$
This notation is used to specify that you are taking the derivative of the specific function $\LARGE f(x)=x^2$ with respect to $x$.
	Here, $\LARGE \frac{d}{dx}$​ is the differentiation operator, and $x^2$ is the function being differentiated.
		It specifically means "differentiate $x^2$ with respect to $x$".

$$\LARGE \frac{df}{dx}x^2$$
This notation is more ambiguous and typically incorrect in this context unless it has a very specific meaning defined in a particular problem or scenario. 
	It can be broken down as follows:
	$\LARGE \frac{df}{dx}$ This generally means the derivative of some function $f$ with respect to $x$.
	$\LARGE x^2$ This is just a multiplication with $\LARGE x^2$.

However, when combined as $\LARGE\frac{df}{dx} x^2$, it suggests that the derivative of $f$ with respect to $x$ is being multiplied by $x^2$. 
	This is not the same as taking the derivative of $x^2$ with respect to $x$.
		This would mean "multiply the derivative of $f$ with respect to $x$ by $x^2$".
##### But if $\LARGE f(x)=x^2$ then $\LARGE \frac{df}{dx} == \frac{d}{dx}x^2 == \frac{d}{dx}f(x)$
When Defining the Derivative by Rules of Differentiation, each term is differentiated (i.e. the Derivative for each term is obtained).
	Therefore, you will see a lot of the $\LARGE \frac{d}{dx}x^2$ form.
- - -
## Derivative as a Name
Refers to a seemingly "instantaneous" rate of change. 

First used by mathematician Lagrange in the late 18th century.
	Derived from the Latin word "derivare", which means:
		"To draw off" or "to take from".
			The idea was to take the original function and draw from it a new function.
				This new function would describe how original function changes.
				
The derivative is the result of an operation that takes a function and produces another function.
	Then new function (the derivative) provides information on the slope or rate of change of the original function at any given point. 
	
It is a conceptual representation of the slope over an interval that is infinitesimally small.
	So small that it's effectively a point. 

- - -
### Rate of Change
##### The [[Ratio#Rate (of change)|Rate]] 
Refers to the ***comparison*** of two quantities.
##### The Change 
Refers to the ***two quantities***.
	Specifically the **differences** of the two quantities.
		In this specific case, one quantity is dependent on the other. 
	 
The difference quotient is a formula used to calculate the average rate of change of a function over a specified interval. 
	This Differential Ratio is a type of Difference Quotient, the key characteristic is that the Numerator and Denominator are both Differentials.

The ratio of the Function Output Value and the Change in the Input Variable Value, is the Differential Ratio, where both are themselves Differentials. 
		And this Differential Ratio is the Derivative.
##### The [[Ratio#Average Rate (of change)|Average Rate of Change]]
$$\LARGE \text{Given an interval } [x_1, x_2]$$
$$\LARGE \text{Average Rate of Change } = \frac{(f(x_2) - f(x_1))}{x_2 - x_1}$$
Is represented by a [[Secant Line#The Average Rate of Change|Secant Line]].
	The Secant Line connects two points on a curve.
		The Slope of the Secant Line gives an average rate of change between those two points.

It is the Rate of Change over a defined interval, where one quantity is dependent on the other.
#### The [[Ratio#Instantaneous Rate (of change)|Instantaneous Rate of Change]]
$$\LARGE f'(x) = \lim_{h \to 0}\frac{f(x + h) - f(x)}{h}$$
As the two points get closer to each other, the secant line approaches the [[Tangent Line#The Slope of a Secant Line|Tangent Line]] at a single point on the curve.
	The Slope of the Tangent Line represents the Instantaneous Rate of Change.

This Instantaneous Rate of Change *is* the Derivative. 
### *Note on "With Respect to..."*
In terms of differentials, this phrasing refers to the variable that is changing or the variable with respect to which we are measuring the rate of change. 
	When taking the derivative of a function, we are interested in how the function changes as one specific variable changes, while keeping other variables constant..

- - -
## The Average Rate of Change is the [[A Map of Change as Rates to Limits of those Rates to Differentials to Derivatives#Difference Quotient|Difference Quotient]]
$$\LARGE \text{Average Rate of Change } = \frac{\Delta f(x)}{\Delta x}$$
$$\LARGE \frac{\Delta f(x)}{\Delta x} = \frac{(f(x_2) - f(x_1))}{x_2 - x_1} = \text{Difference Quotient}$$

The difference quotient $\LARGE \frac{f(x+h) - f(x)}{h}$ gives the slope of the secant line between the points $(x, f(x))$ and $(x+h, f(x+h))$ on the curve of the function $f(x)$.
	This secant line approximates the behavior of the function over the interval $[x, x+h]$.
		*Note: The interval is **NOT* infinitesimally small.**
##### Difference
The numerator $f(x+h)−f(x)$ represents the [[Kinematics Analysis#Displacement (Δx,Δy,Δz)|displacement]] or the change in the function's output value as the input changes from $x$ to $x+h$.
##### Quotient
Dividing by $h$ (i.e. the interval between input changes) scales (i.e. [[Division#Contracting|contracts]]) this change by the size of the increment $h$, giving the average rate of change over the interval from $x$ to $x+h$.
## The Difference Quotient *is* the Slope of the Secant Line
Geometrically, the difference quotient $\LARGE {f(x+h)−f(x)​ \over h}$ represents the [[Secant Line#The Average Rate of Change|slope of the secant line]] that passes through the points $(x,f(x))$ and $(x+h,f(x+h))$ on the graph of the function.

The ratio $\frac{f(x+h) - f(x)}{h}$ represents the average rate of change.
	The difference quotient or ratio $\frac{f(x+h) - f(x)}{h}$ is indeed interpreted as a "[[Slope|slope]]".
		Here, $f(x+h) - f(x)$ represents the vertical change (rise), and $h$ represents the horizontal change (run).
		
The difference quotient $\frac{f(x+h) - f(x)}{h}$ gives the slope of the secant line between the points $(x, f(x))$ and $(x+h, f(x+h))$ on the curve of the function $f(x)$.
	This secant line approximates the behavior of the function over the interval $[x, x+h]$.

- - -
## Differentiation
Differentiation is the process of finding the derivative of a function. 
	The derivative represents the rate at which a function is changing at any given point.

Differentiation is used to determine the slope of a function at any point, find the rate of change, and solve problems involving motion, optimization, and other applications where rates of change are important.
### To Differentiate
**Differentiation** is a process (finding the derivative).
	To "Differentiate" a function, means to compute its derivative.

*For example: Differentiating of some function $f(x)$ is to find that function's Derivative,* $\LARGE \frac{df}{dx}$

**Mathematical Representation**
If you have a function $f(x)$, its derivative is denoted as
$$\LARGE f'(x) \text{ or }\frac{df(x)}{dx}$$
### Differential
$$\LARGE \frac{\text{Infinitesmal } \Delta f}{\text{Infinitesmal } \Delta x} = \frac{df}{dx}$$
$$\LARGE \text{The Differential of the function } f(x) \text{ is } df.$$
$$\LARGE \text{The Differential of } x \text{ is } dx.$$
The term "differential" comes from the concept of differences.
	**Differential** refers to an infinitesimal change in a function's Output Value resulting from a small change in the input value. 
		It is used in various contexts, including differentials in calculus and differential equations.

**Differential** is a quantity (an infinitesimal change).
	**Differentials** provide a way to approximate changes in functions.
		Differentials imply a variable approaching zero.
			Differentials are infinitesimally small changes or intervals.
#### Linear Approximation
The differential $dy$ provides a linear approximation to the change in $y$ for a small change in $x$.
	It’s a way to approximate $\Delta y$ when $\Delta x$ is small:
$$\Delta y \approx dy = f'(x) \, dx$$

- - -
## [[A Map of Change as Rates to Limits of those Rates to Differentials to Derivatives|The Relationship Between the Ave. Rate of Change (i.e. Difference Quotient), the Limit of the Difference Quotient (i.e. Differential Ratio) and the Instantaneous Rate of Change (i.e. Derivative)]]
### The Differential of a Function (i.e. a Differential Ratio)
#### When the Difference Quotient Contains Differentials

#### Differential Ratio
$$\LARGE \frac{\text{Infinitesmal } \Delta f}{\text{Infinitesmal } \Delta x} = \frac{df}{dx}$$
A differential ratio, often just referred to as a ratio of differentials, is an expression involving differentials. 
	For instance, $\LARGE \frac{df}{dx}$ is a differential ratio representing the derivative of $y$ with respect to $x$. 
		This ratio indicates how a small change in $x$ (denoted by $dx$) relates to a small change in $f(x)$ (denoted by $dy$).
			*Note: A Differential Ratio is **not** equal to the Differential Equation.*

For a function $f(x)$, the differential $df$ is defined in terms of the derivative $f′(x)$ and the differential $dx$.\
	The differential $df$ represents the change in $f(x)$ for a small change in $x$, denoted by $dx$, which is also a differential.
		This shows that the differential $df$ is the product of the derivative $f′(x)$ and the differential $dx$.
$$\LARGE f'(x) = \frac{df}{dx}$$
$$\LARGE df=f′(x) dx = \frac{df}{dx}dx$$
Here:
- $df$ is the differential of the function $f$(x).
- $\frac{df}{dx}$ is the derivative of $f$ with respect to $x$, which tells us the rate of change of $f$ as $x$ changes.
- $dx$ is the differential of $x$, representing a small change in $x$.
### The Ratio of Differentials *is* the Derivative
The derivative $f′(x)$ can be interpreted as the ratio of the differential of the function $dy$ to the differential of the variable $dx$:
$$\LARGE f'(x) = \frac{dy}{dx} \quad \text{and} \quad dy = f'(x) \, dx$$
This relationship shows that the derivative is the ratio of the differential change in the function to the differential change in the input variable, and differentials provide a linear approximation of the function's change based on its derivative.
    This equation signifies that the derivative is the rate at which $y$ changes with respect to $x$.
	    I.e. The Derivative is the ratio of the differential $dy$ to the differential $dx$.
##### Differentials in Linear Approximation
Differentials are used to linearly approximate changes in the function.
	For a small change $dx$ in the input, the corresponding change in the output $dy$ can be approximated using the derivative:
$$dy≈f′(x)dx$$
### Differential Ratio *is* a Limit
$$\LARGE \frac{\text{Infinitesmal } \Delta f}{\text{Infinitesmal } \Delta x} = \frac{df}{dx} = f'(x) = \lim_{h \to 0} = \frac{f(x+h) - f(x)}{h}$$
Remember, the Differentials, $df$ and $dx$ represent infinitesimal changes in their values. 
	That when the change of $x$ is infinitesimal, there is an infinitesimal change in $f(x)$.

Differentials imply a variable approaching zero.
Differentials are infinitesimally small changes or intervals.
	Therefore, Differential Ratios imply the Limit of a ratio. 
#### This is the **Equivalent** of the Following
As $h$ approaches zero, this ratio becomes $\frac{dy}{dx}$, representing the instantaneous rate of change.
$$\LARGE f'(x) = \frac{df}{dx} = \lim_{h \to 0} = \frac{f(x+h) - f(x)}{h}$$
$$\LARGE h \text{ is equivalent to } dx \text{ and } f(x + h) - (fx) \text{ is equivalent to } df$$
##### Numerator ($f(x+h) - f(x)$):
Is the differential of the function, $f(x)$, that is $\LARGE df$
	This represents the infinitesimally small change in the dependent variable (output of the function) over the interval $h$.
		It shows how much the function's output changes as the input changes by $h$.

The numerator $f(x+h) - f(x)$ is equivalent to/becomes the differential $dy$.
	In differential terms, as $h$ approaches zero, this change is represented by $dy$ (the differential of the dependent variable).
##### Denominator ($h$):
Is the Differential of $x$.
	This represents the infinitesimal small change in the independent variable over the interval $h$.
		Which is the interval over which we are measuring the change in the function's value.

The denominator $h$ is equivalent to/becomes the differential $dx$.
	In differential terms, as $h$ approaches zero, this change is represented by $dx$ (the differential of the independent variable).

- - -
### The Differential (i.e. a Limit) is the Instantaneous Rate of Change
#### Think About it...
When the change becomes infinitesimal, the interval between the two points approaches $0$.
	Therefore, the rate of change between these two points, begins to represent the smallest interval of change.
		This smallest interval of change between two points, represents the **"Instantaneous" Rate of Change.**
$$\LARGE \text{If } dx \text{ (i.e. } h \text{)} = 0$$
$$\LARGE \frac{df}{dx} = \frac{0}{0} = \lim_{h \to 0} = \frac{f(x+0) - f(x)}{0}$$
### The Instantaneous Rate of Change (i.e the Limit of the Slope of the Secant Line) is the Slope of the Tangent Line
Remember that the Slope of a Secant Line represents the Average Rate of Change.
$$\LARGE \text{Ave. Rate of Change} = {f(x-2)−f(x_1)​ \over x_2 - x_1} = \text{Slope of the Secant Line}$$
This ratio is the slope of a linear function.
	Aka the [[Slope|Slope]] of the [[Secant Line|Secant Line]]. 
#### As the Average Rate of Change Approaches the Instant Rate of Change
##### The Secant Line Approaches the Tangent Line
![[Pasted image 20240410153825.png|400]]
**When the *change* becomes infinitesimally small**, that is, as the $\LARGE \Delta x$ (i.e. $\LARGE h$) approaches $0$, the secant line approaches the tangent line to the curve at the point $\LARGE x$.
$$\LARGE f'(x) = \frac{df}{dx} = \lim_{h \to 0} = \frac{f(x+h) - f(x)}{h}$$
As $h$ approaches zero, this average slope becomes the instantaneous slope, which is the Tangent Line.
![[Pasted image 20240422232308.png]]
## The Differential Ratio *is* the Slope of the Tangent Line
![[Pasted image 20240422233019.png]]
The Limit of the slope of this tangent line is the derivative of the function at that point, $f'(x)$.
#### Which is the Derivative
A derivative (of a function $f(x)$) at a single point $f'(x)$, is itself a function that maps that single point (as an input) to the **value** of the **limit** of the **average rate of change** (i.e. limit of $\Delta y / \Delta x$) of that input.

The differential of the function is represented/expressed in the fact that the derivative is defined as the **limit of the Differential Ratio**. 
	This ratio is called the **derivative**.
		The derivative (i.e. the ratio of the change in output values to the change in the input values) represents how a small change in the input (independent variable) results in a change in the output (dependent variable).

- - -
## Derivative Is 
### 1. [[#The Ratio of Differentials *is* the Derivative|A Ratio of Differentials]]
Ratios are a fundamental to the concept of the derivative.
It [[Data/Abstract Mathematical Spaces/Abstract Mathematical Objects/Measurement|measures]] the output ($\Delta y$) (i.e. the differential $dy$) of a function $f(x)$ is proportioned to the input ($\Delta x$) (i.e. the differential $dx$) at an infinitesimally small scale.

$$\LARGE f'(x) = \frac{\Delta y}{\Delta x}$$

The derivative is the ratio of the change in the output to the change in the input as the change in the input approaches zero.
### 2. [[#The Differential (i.e. the Limit) is the Instantaneous Rate of Change|The Instantaneous Rate of Change of a Function]]
A derivative (of a function $f(x)$) at a single point $f'(x)$, is itself a function that maps that single point (as an input) to the **value** of the **limit** of the **average rate of change** (i.e. limit of $\Delta y / \Delta x$) of that input.
### 3. [[#The Differential Ratio *is* the Limit *of* the Slope of the Tangent Line|The Limit of the Slope of the Secant Line as h Approaches Infinity]] (i.e. the [[Straight Lines#The Derivative as the Derivatives Is the Tangent Line The Slope of a Tangent Line Slope (i.e. a proportion/rate/ratio between $ Delta y / Delta x$) of the Tangent Line Tangent Line Slope of a Tangent Line|Slope of the Tangent Line]])
A **derivative** of a **function** at a point **provides the slope of the [[Secant Line|Secant]] line to the function at that specific point**.^calculus-derivatives
The **derivative** (which only exists for a given point) is itself is a **value** that represents the **exact slope** of the **tangent vector** at that **point** it is associated with (on the curve).
	I.e. The **derivative** ***is*** the **slope of the tangent line**.
		![[Pasted image 20240410150406.png]]
##### The [[Data/Abstract Mathematical Spaces/Physics/Analysis/Tangent Line|Tangent Line]]
 The **Tangent line (or vector)** at a single point, represents the **"instantaneous" rate of change** of the curve (i.e. function) at that point. ^f2b939
	The slope of this tangent line/vector is given by the **derivative** of the curve/function at this point. ^1f0a97
	The derivative at any point, gives the direction of the tangent vector at that point.
		For surfaces, taking partial derivatives provides the tangent planes.
###### [[Data/Abstract Mathematical Spaces/Physics/Analysis/Tangent Line|Tangent Line Through a Point (a, f'(a))]] 
$$\LARGE y = f(a) + f'(a)(x-a)$$
Formally, the derivative at a point $a$, is **defined** as the [[Limits|limit]] of the slope of the Secant Line (i.e. **instantaneous rate of change**)
![[Pasted image 20240422232308.png]]
![[Pasted image 20240727142926.png]]
![[Pasted image 20240422233019.png]]
As the **interval or distance** over which the change is measured (between point $a$ and another determined point), **approaches zero**. ^c2858f
	If this limit exists, then the function is **[[#Differentiability|differentiable]]** at that point, and the slope of the tangent line at this point is precisely the value of this limit itself - which is the derivative of that point.

**The equation to determine the derivative is:**
	The limit of the average rate of change as the interval (between two points) approaches zero.
		Where the **average rate of change** over an interval of distance between two points is:
			The **slope** of the **secant line** that connects those two points. 

The **[[Limits|limit]]** is the **means** of **transitioning** between the **average rate of change** to the **instantaneous rate of change**. ^limit-as-a-transition
![[Pasted image 20240410153825.png|400]] ^d8b06d
### 4. Is the Unit Tangent Vector
That is, the vector contains the coordinates of a slope of a line that is tangent to the point. 
	The tangent vector $T(\Delta x)$ visually and mathematically represents the instantaneous rate of change of the function $f$ at a point $x$.
		The components of the vector capture the differential changes in the input and output, providing a linear approximation of the function's behavior near that point.

In the context of single-variable calculus, the derivative $f'(x)$ gives the slope of the tangent line to the curve $y=f(x)$ at the point $x$. If we interpret this geometrically:

The tangent vector to the curve at point $(x, f(x))$ can be thought of as having components that describe its direction and magnitude.
#### Components of a Tangent Vector
For a [[Abstract Mathematical Spaces#Scalar Functions|scalar function]] $y=f(x)$
##### Point on the Curve
Consider the point $P=(x, f(x))$ on the curve.
##### Tangent Vector
The tangent vector at $P$ can be described in terms of its components along the x-axis and y-axis.
	The change in $x$ is typically considered as $\Delta x$, and the change in $y$ is $\Delta y=f'(x) \Delta x$.
##### Tangent Vector Components
Let $\Delta x$  be a small change in $x$. The corresponding change in $y$, denoted $\Delta y$, can be approximated using the derivative $f'(x)$. 
	This represents the corresponding change in the $y$-direction based on the slope of the function at the point $x$. 
		The derivative $f'(x)$ gives the rate of change of $y$ with respect to $x$.
			This represents the corresponding change in $y$ based on the slope of the function at that point.
$$\LARGE y = f'(x) \Delta x $$
$$\LARGE \text{Which itself is the Slope of the Tangent Vector}$$
$$\LARGE \text{And is a component of the Tangent Vector}$$
The components of the tangent vector are given by the changes in $x$ and $y$:
$$\LARGE \mathbf{T} = \mathbf{T}(\Delta x) \begin{pmatrix} \Delta x \\ \Delta y \end{pmatrix} = \begin{pmatrix} \Delta x \\ f'(x) \Delta x \end{pmatrix}$$
##### Unit Tangent Vector
The direction of the tangent vector is given by the slope $f'(x)$.
	If $\Delta x = 1$ then $f'(x)\Delta x == f'(x)$
A unit tangent vector can be [[Static Equilibrium#Normalizing Vectors (i.e. unit vectors)|normalized]] and expressed as:
$$\LARGE \mathbf{T} = \frac{1}{\sqrt{1 + (f'(x))^2}} \begin{pmatrix} 1 \\ f'(x) \end{pmatrix}$$
###### To find the unit tangent vector, normalize the tangent vector $\mathbf{T}$. 
###### 1. First, calculate the magnitude of $\mathbf{T}$:
$$\LARGE |\mathbf{T}| = \sqrt{(\Delta x)^2 + (f'(x) \Delta x)^2} = \Delta x \sqrt{1 + (f'(x))^2}$$
##### 2. Then, divide the components of $\mathbf{T}$ by this magnitude
$$\LARGE \mathbf{T}_{\text{unit}} = \frac{1}{|\mathbf{T}|} \mathbf{T} = \frac{1}{\Delta x \sqrt{1 + (f'(x))^2}} \begin{pmatrix} \Delta x \\ f'(x) \Delta x \end{pmatrix}$$
###### 3. Simplify
$$\LARGE \mathbf{T} = \frac{1}{\sqrt{1 + (f'(x))^2}} \begin{pmatrix} 1 \\ f'(x) \end{pmatrix}$$

- - -
## Calculating the Derivative 
### Defining the Derivative at a Point vs. as a Function
##### Defined for a Specific Point
The primary difference between finding the [[Limits#Limit as a Derivative at a Specific Point|derivative at a specific point]] and finding the general derivative function lies in whether or not you plug in a specific value for the variable.
##### Defining as a Function (i.e. for a set of points)
When represented as functions, describe the rate of change of a function at any point in its domain. 
	This is known as the derivative function or simply the derivative of the function.
		This derivative function provides a formula that can be used to find the slope of the tangent line to the function at any point in its domain.

The derivative function $f'(x)$ represents the rate of change of $f(x)$ at any point $x$ in its domain. 
	It is defined using the same [[Limits|limit]] process, but we do not fix $x$ at a specific value. 
		Instead, we keep $x$ as a variable.
			If $f(x)$ is a differentiable function, its derivative function, denoted $f′(x)$ or $\frac{d}{dx}$, is defined as:
$$\LARGE f'(x) = \lim_{{h \to 0}} \frac{f(x+h) - f(x)}{h}$$
This derivative function $f′(x)$ gives the slope of the tangent line to the curve at any point $x$.
### 1. Using Limits to Define the Derivative
The limit definition of the derivative fundamentally captures the idea of **how the output of a function changes with respect to changes in the input variable**. 
	This approach involves a detailed process that directly examines the rate of change of the function's output as the input changes by a small amount.
#### For a Specific Point
The derivative of a function $f(x)$ at a point $x$ is fundamentally defined using limits. 
	This definition captures the rate of change of $f(x)$ with respect to $x$:

$$\LARGE f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$
This limit definition can be broken down as follows:
1. **Increment the Input:** Consider a small increment $h$ added to the input $x$, so you evaluate the function at $x + h$.
2. **Change in Output:** Compute the change in the function's output, $f(x + h) - f(x)$.
3. **Rate of Change:** Divide the change in output by the change in input $h$.
4. **Limit:** Take the limit as $h$ approaches zero to find the instantaneous rate of change.
##### General Steps
$$\LARGE \text{1. Substitute } x + h \text{ into the function:}$$
$$\text{Calculate } f(x + h) \text{ by substituting } x + h \text{ for every } x \text{ in the function } f(x).$$
$$\LARGE \text{2. Form the difference quotient:}$$
$$\LARGE \text{3. Calculate the difference (i.e. Simplify) } f(x + h) - f(x)$$
$$\LARGE \text{4. Divide by } h:$$
$$\LARGE \text{Form the quotient } \frac{f(x + h) - f(x)}{h}$$
$$\LARGE \text{5. Take the limit as } h \text{ approaches 0:}$$
$$\LARGE \text{Evaluate the limit } \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$
$$\text{This limit, if it exists, is the definition of the derivative of } f \text{ at } x, \text{ denoted }$$
$$\LARGE f'(x) \text{ or } \frac{d}{dx} f(x)$$
$$\LARGE \text{ Mathematically, it is expressed as:}$$
$$\LARGE f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$
### 2. Using the [[#Rules of Differentiation|Rules of Differentiation]]
###### *Important*: You only ever apply the Differentiating Rules to the terms associated with the independent variable.
#### This is Because...
Differential rules, such as the power rule, product rule, and chain rule, provide straightforward methods for finding derivatives of functions.
	These rules are used to differentiate terms with the $x$ variable with respect to $x$.

Differential rules provide a set of formulas and shortcuts to efficiently find derivatives without explicitly computing the limit every time. 
	These rules **apply directly to differentiating the variable with respect to itself** and are derived from the fundamental limit definition of the derivative.
#### General Differentiation Process
in general, when differentiating a function with respect to a variable, you apply differentiation rules (such as the power rule, product rule, quotient rule, and chain rule) **to each term that contains the variable**. 
	This is how you obtain the derivative of the entire function. 
###### 1. Identify the Function and Variable
Determine the function you need to differentiate and the variable with respect to which you are differentiating.
###### 2. Differentiate Each Term
Apply the appropriate differentiation rule to each term containing the variable.
###### 3. Combine the Results
Sum the derivatives of each term to obtain the derivative of the entire function.
- - -
## Derivatives of a Constant
When you differentiate a function, any constant term disappears because the derivative of a constant (i.e. constant function) is zero. 

A **constant function** is a function that always returns the same value, **regardless of the input**.
	It does not depend on any variable and is represented mathematically as:
	$$\LARGE f(x)=C, \text{where C is a constant}$$
Here, $C$ is a fixed value and does not change with $x$.

If $f(x) = c$, where $c$ is a constant, then the derivative of $f$ with respect to $x$ is zero:
$$\LARGE \frac{d}{dx} c = 0$$
### Think About it...
Remember the Derivative measures the **rate of change** as a ratio. 
	A constant implies no change. 
	
If say the velocity is constant, then the rate of change of velocity - that is acceleration, is zero.
	Because velocity is constant and thus does not have a rate of change, because it does not change.
		And therefore, the derivative of velocity, that is, acceleration (i.e. the rate of change of velocity), does not exist.
### Derivative of a Constant is Zero
$$\LARGE f′(x)=\lim\limits_{​\triangle x \rightarrow 0} {f(x+\triangle x) - f(x) \over \triangle x}​$$
##### 1. Constant Function
A constant function $\LARGE f(x)=c$ means that the function's value does not change no matter what the input x is.
		 *For Example:* if we know that the velocity is constant, then we know that the derivative which is acceleration, will be zero- as a constant velocity means to no change in velocity and thus no acceleration (i.e. rate of change of velocity).
    - A constant function $\LARGE f(x)=c$ means that the function's value does not change no matter what the input x is.
    - For example, $f(x)=5$ means the function always outputs 5, regardless of the value of x.
##### 2. Rate of Change of a Constant Function
Since the value of a constant function does not change, the rate of change (or the slope) is zero.
	Using the definition of the derivative: 
$$\LARGE f′(x)=\lim\limits_{​\triangle x \rightarrow 0} {f(x+\triangle x) - f(x) \over \triangle x}​$$
For a constant function $f(x)=c$: 
$$\LARGE f'(x) = \lim\limits_{\triangle x \rightarrow 0} {c -c\over \triangle x} = \lim\limits_{\triangle x \rightarrow 0} {0\over \triangle x} = 0$$
#### Visualizing the Derivative of a Constant
Imagine a flat horizontal line on a graph, like 𝑦=5y=5. This line has no slope; it does not rise or fall as you move along the 𝑥x-axis. The rate of change of this line is zero everywhere because it is perfectly flat.

When you differentiate a function that includes a constant, the constant term "disappears" in the sense that its derivative is zero, which is why the constant does not affect the derivative of the rest of the function.

- - -
## Rules of Differentiation
### Derivative of a Linear Term, ($\LARGE ax$)
Aka Differentiating $x$ with Respect to Itself "*Directly*"
The "derivative of a linear term" rule refers to the differentiation of a term of the form $ax$, where $a$ is a constant and $x$ is the variable. 
	The rule states that the derivative of such a term with respect to $x$ is simply the constant coefficient $a$.
$$\LARGE f(x)=ax == \text{A Linear Term}$$

To find the derivative of $f(x)$ with respect to $x$, denoted as $\frac{d}{dx}(ax)$, we use the [[#Power Rule|Power Rule]]. 

In the case of $\LARGE ax$, we can rewrite it as $\LARGE ax^1$. 

Applying the power rule:
$$\LARGE \frac{df}{dx}(ax^1) = a \cdot \frac{df}{dx} \cdot x^{1-1} = a \cdot 1x^0 = a \cdot 1 = a$$

Therefore, the derivative of $ax$ with respect to $x$ is $a$.
###### Rate of Change of $t$ with Respect to Itself "*Directly*"
When we say "with respect to itself," we mean that we are differentiating a variable with respect to that same variable.
	In this case, where f(x) = x, the derivative is always 1.
		Where $f(x) = x^2 ,etc....$ it is still considered differentiating x with respect to x, but it is not a direct differentiation. 

*For Example*:
The derivative of $t$ is simply 1. 
![[Pasted image 20240604144939.png]]
![[Pasted image 20240604144946.png]]
![[Pasted image 20240604144953.png]]
![[Pasted image 20240604145001.png]]
![[Pasted image 20240604145006.png]]

- - -
### Constant Scalar Rule, ($\LARGE af(x)$)
The constant scalar rule states that when you take the derivative of a constant multiplied by a function, the constant can be factored out of the differentiation process.
	I.e. Allows factoring out the constant **before** differentiating the function.

If $f(x) = c \cdot g(x)$, where $c$ is a constant scalar, and $g(x)$ is a differentiable **function**, then the derivative of $f$ with respect to $x$ is:
#### $\LARGE \frac{d}{dx} \left( c \cdot g(x) \right) = c \cdot \frac{d}{dx} g(x)$
###### Example
#### $\LARGE \frac{d}{dx} (3x^3) = 3 \cdot \frac{d}{dx} (x^3) = 3 \cdot 3x^2 = 9x^2$

- - -
### Power Rule
If $f(x) = x^n$, where $n$ is a constant, then the derivative of $f$ with respect to $x$ is given by:
	Basically just decrease the exponent by 1, then place the original value of the exponent as a coefficient in front of the term. 
#### $\LARGE \frac{d}{dx} x^n = n x^{n-1}$ 

###### Example
$\LARGE \frac{d}{dx} x^5 = 5x^4$ 
##### Derivation of the Power Rule
1. **Start with the Limit Definition:**
$$\LARGE \frac{d}{dx}(x^n) = \lim_{h \to 0} \frac{(x + h)^n - x^n}{h}$$​
2. **Expand Using the Binomial Theorem:**
$$\LARGE (x + h)^n = x^n + nx^{n-1}h + \frac{n(n-1)}{2}x^{n-2}h^2 + \cdots + h^n$$
3. **Subtract $\LARGE x^n$ and Simplify:**
$$\LARGE \frac{(x + h)^n - x^n}{h} = \frac{nx^{n-1}h + \frac{n(n-1)}{2}x^{n-2}h^2 + \cdots + h^n}{h}$$
$$\LARGE nx^{n-1} + \frac{n(n-1)}{2}x^{n-2}h + \cdots + h^{n-1}$$
4. **Take the Limit as $\LARGE h \to 0$:**
$$\LARGE \lim_{h \to 0} \left(nx^{n-1} + \frac{n(n-1)}{2}x^{n-2}h + \cdots + h^{n-1}\right) = nx^{n-1}$$
This shows that the derivative of $x^n$ with respect to $x$ is $nx^{n-1}$.

##### Example of Power Rule via Limit Definition of a Derivative
###### 1. Apply the Limit Definition:
$$ \LARGE f'(x) = \frac{df}{dx}(x^2) = \lim_{h \to 0} \frac{(x + h)^2 - x^2}{h}$$
###### 2. Expand and Simplify:
$$ \LARGE f'(x) = \lim_{h \to 0} \frac{(x^2 + 2xh + h^2 - x^2)}{h} =  \lim_{h \to 0}\frac{(2xh + h^2)}{h} =  \lim_{h \to 0}(2x+h)$$
###### 3. Take the Limit
$$\LARGE \text{Where } h \text{ is } 0.$$
$$\LARGE f'(x) = \lim_{h \to 0}(2x+h) = 2x$$

- - -

### Sum Rule
If $f(x) = g(x) + h(x)$, where $g(x)$ and $h(x)$ are differentiable functions, then the derivative of $f$ with respect to $x$ is:
$\LARGE \frac{d}{dx} \left( g(x) + h(x) \right) = \frac{d}{dx} g(x) + \frac{d}{dx} h(x)$
###### Example
#### $\LARGE \frac{d}{dx} (x^2 + x^3) = \frac{d}{dx} (x^2) + \frac{d}{dx} (x^3) = 2x + 3x^2$


- - -

### Difference Rule
If $f(x) = g(x) - h(x)$, where $g(x)$ and $h(x)$ are differentiable functions, then the derivative of $f$ with respect to $x$ is:
#### $\LARGE \frac{d}{dx} \left( g(x) - h(x) \right) = \frac{d}{dx} g(x) - \frac{d}{dx} h(x)$

- - -

### Product Rule
If $f(x) = g(x) \cdot h(x)$, where $g(x)$ and $h(x)$ are differentiable functions, then the derivative of $f$ with respect to $x$ is:
#### $\LARGE \frac{d}{dx} \left( g(x) \cdot h(x) \right) = g(x) \cdot \frac{d}{dx} h(x) + h(x) \cdot \frac{d}{dx} g(x)$

###### Example
#### $\LARGE \frac{d}{dx} (x^2 \cdot \sin(x)) = x^2 \cdot \cos(x) + \sin(x) \cdot 2x = x^2 \cos(x) + 2x \sin(x)$
- - -

### Quotient Rule
If $f(x) = \frac{g(x)}{h(x)}$, where $g(x)$ and $h(x)$ are differentiable functions and $h(x) \neq 0$, then the derivative of $f$ with respect to $x$ is:
#### $\LARGE \frac{d}{dx} \left( \frac{g(x)}{h(x)} \right) = \frac{h(x) \cdot \frac{d}{dx} g(x) - g(x) \cdot \frac{d}{dx} h(x)}{(h(x))^2}$
###### Example
#### $\LARGE \frac{d}{dx} \left( \frac{x^2}{\sin(x)} \right) = \frac{\sin(x) \cdot 2x - x^2 \cdot \cos(x)}{(\sin(x))^2}$


- - -
### [[Chain Rule|Chain Rule]]
The chain rule is a formula for computing the derivative of the composition (i.e. composite functions) of two or more functions.
	If you have a function $f(x)$ that is composed of two functions $g$ and $h$, such that:
	$$\LARGE f(x) = g(h(x))$$
Then the Chain Rule helps you find the derivative of $f(x)$ with respect to $x$. 

Then the Chain Rule states that:
$$\LARGE f(x) = g(u) \text{, and } u = h(x)$$
$$\LARGE \frac{df(g(h(x)))}{dx} = \frac{df(g(h(x)))}{dh(x)} \cdot \frac{dh(x)}{dx}$$
$$\LARGE f'(g(h(x)) = \frac{df(g(h(x)))}{dx}= \text{Derivative of }f(g(h(x))) \text{ with respect to }x$$
$$\LARGE g'(h(x)) = \frac{dg(x)}{dx}= \text{Derivative of }g(h(x)) \text{ with respech respect to }h(x)$$
$$\LARGE h'(x) = \frac{dh(x)}{dx}= \text{Derivative of }h(x) \text{ with respech respect to }x$$
where:
###### $g()$ is a [[#Differentiable Function|Differentiable Function]] of $h(x)$
This means that $g$ is a function that can be differentiated with respect to its argument, which is $h(x)$.
	In other words, if you treat the output value of $h(x)$ as a single variable, the function $g$ has a well-defined derivative at every point where $h(x)$ is defined.
###### $h(x)$ is a Differentiable Function of $x$
This means that $h$ is a function of $x$ that can be differentiated with respect to $x$.
	In other words, $h$ has a well-defined derivative at every point in its domain.

If $f(x) = g(h(x))$, where $g$ is a [[#Differentiable Function|differentiable function]] of $h(x)$ and $h(x)$ is a differentiable function of $x$, then the derivative of $f$ with respect to $x$ is:
$$\LARGE \frac{d}{dx} g(h(x)) = g'(h(x)) \cdot h'(x)$$
#### Step by Step Process
###### Example
$$\LARGE g(u) = u^2 + 3 \text{ and } h(x) = \sin(x)$$
##### 1. Identify the Inner and Outer Functions
###### Outer Function
$$\LARGE \text{Outer Function}= g(u) = u^3 + 3u \text{, where } u = h(x)$$
###### Inner Function
$$\LARGE \text{Inner Function} = h(x) = \sin(x)$$
##### 2. Differentiate the Outer Function
###### 1. Find the Derivative the Outer Function $g(x)$ as $u$ changes.
$$\LARGE g(u) = u^2 + 3u$$
$$\LARGE g'(u) = \frac{dg}{du} = 2u + 3$$
###### 2. Find the Derivative of the Inner Function $h(x)$ as $u$ changes.
$$\LARGE h(x) = \sin(x)$$
$$\LARGE h'(x) = \frac{dh(x)}{dx} = \cos(x)$$
###### 3. Apply the Chain Rule
- According to the Chain Rule:
$$\LARGE \frac{df(g(h(x)))}{dx} = \frac{df(g(h(x)))}{dh(x)} \cdot \frac{dh(x)}{dx}$$
1. Multiply the Derivatives from Steps 1 and 2 to get the Derivative of the Composite Function.

2. Substitute the the Inner and Outer differentials obtained from Steps 1 and 2 for $\LARGE g'(x) = \frac{df(g(x)))}{dh(x)}$ and $\LARGE h'(x) = \frac{dg(h(x))}{dx}$
$$\LARGE \frac{df(g(x))}{dx} = (2u+3) \cdot \cos(x)$$
3. Substitute Back the Intermediate Variable, $\LARGE u$
	Since $\LARGE u = h(x) = \sin(x)$, substitute $u$ back into the expression. 
$$\LARGE \frac{df(g(x))}{dx} = (2(\sin(x))+3) \cdot \cos(x)$$
###### 4. The Derivative
$$\LARGE \boxed{\frac{df}{dx} = (2\sin(x) + 3) \cdot \cos(x)}$$


- - -
## Example: Using the Rules of Differentiation to find the  Derivative

#### Given Position Function:

![[Pasted image 20240602234115.png]]
#### Find the Derivative:

To find the derivative x′(t), we'll differentiate x(t) with respect to t.

1. **Write the position function:** 
	![[Pasted image 20240602234124.png]]
2. **Differentiate each term:**
	Differentiating each term in the function $x(t) = t^2 + 3t +2$ involves applying basic [[#Rules of Differentiation|rules of differentiation]]. 
![[Pasted image 20240604144556.png]]

![[Pasted image 20240602234407.png]]
 ![[Pasted image 20240602234152.png]]
3. **Combine the results:** 
	![[Pasted image 20240602234201.png]]
### Interpretation
![[Pasted image 20240602234215.png]]

- - -
## Differentiability
### Differentiable Function
A **differentiable function** is a function that has a derivative at every point in its domain.
	In other words, a function $f(x)$ is differentiable at a point $x = a$ if the derivative $f'(a)$ exists. 
		More generally, a function is differentiable on an interval if it has a derivative at every point in that interval.

When we say that a function is "differentiable," it means that the function has a derivative.
	In other words, at each point in its domain, the function has a well-defined rate of change.

**In calculus**, it refers a **curve** that has, at a **point** in a **function**, a **derivative** **existing**. 
###### Key Characteristics of a Differentiable Function
1. **Continuity**:
    - A differentiable function must be continuous. This means that the function does not have any jumps, breaks, or holes. If $f(x)$ is differentiable at $x = a$, then it must be continuous at $x = a$.
    - Formally: If $f$ is differentiable at $x = a$, then $\lim_{{x \to a}} f(x) = f(a)$.
2. **Existence of the Derivative**:
    - A function $f$ is differentiable at $x = a$ if the limit that defines the derivative exists:
    $$\LARGE f'(a) = \lim_{{h \to 0}} \frac{f(a+h) - f(a)}{h}$$​
3. **Smoothness**:
    - Differentiable functions are "smooth" in the sense that they do not have any sharp corners or cusps. The graph of a differentiable function has a well-defined tangent line at every point in its domain.
###### As Differentiability relates to [[Limits#Limits Define Continuity or Discontinuities Discontinuity|Continuity]]:
Differentiability implies Continuity but not every continuous function is differentiable. 
###### Continuity
A function can be continuous without being differentiable.
A function fff is continuous at a point p\mathbf{p}p if, for every ϵ>0\epsilon > 0ϵ>0, there exists a δ>0\delta > 0δ>0 such that for all points q\mathbf{q}q within a distance δ\deltaδ of p\mathbf{p}p, the value of f(q)f(\mathbf{q})f(q) is within ϵ\epsilonϵ of f(p)f(\mathbf{p})f(p). In simpler terms, small changes in the input lead to small changes in the output.
An example of this is the absolute value function f(x)=∣x∣f(x) = |x|f(x)=∣x∣, which is continuous everywhere but not differentiable at x=0x = 0x=0.
- **Differentiability**: If a function is differentiable at a point, it must be continuous at that point. However, the reverse is not necessarily true.

**For a function to be differentiable at a point**, it **must** be **continuous at that point**, and the **derivative** at that point must also exist.
	Solutions to differential equations are often smooth and continuous (i.e. differentiable).
		This is because most physical process **behave** as though they are continuous (i.e. smooth) over time and space.
			Making differentiable functions suitable models for such processes.
			
For a curve (i.e. function) to be differentiable **everywhere** it must be smooth without any [[Discontinuities|discontinuities]] for the entirety of its length. 
	And would therefore, have tangent vectors for every point on its curve.
	
**In computational geometry**, it refers to the curve being smooth enough at a point that you can define a tangent line at every point along the curve. 
	**I.e. A curve is differentiable if it has a derivative at every point along the curve.**
		In which case it would be smooth enough that a tangent vector could be defined at every point along the curve.
			A curve that is not differentiable at a point might have a discontinuity (like a cusp) there instead.
### Conditions for Differentiability
##### [[Continuities|Continuity]]
A function $f(x)$ must be continuous at the point $x=a$. 
    $$\LARGE \lim_{{x \to a}} f(x) = f(a)$$
If a function is not continuous at a point, it cannot be differentiable there.
##### Existence of the Limit
The limit that defines the derivative must exist. Specifically:
    $$\LARGE f'(x)=\lim_{{h \to 0}} \frac{f(a+h) - f(a)}{h}$$
This limit must exist and be finite for the function to be differentiable at $x=a$.
##### Graphical Interpretation
Graphically, a function is differentiable at a point if the graph of the function has a well-defined tangent line at that point. 
	This means the function does not have any sharp corners or cusps at the point, and the tangent line does not become vertical.

- - -
## Derivatives and [[Continuities|Continuity]]
Refers to the concept where [[Notion of Surface Curvature|curvature]] and [[Continuities|continuity]] relate to derivatives and matching derivatives ensures 
	Specifically, it is often discussed under the terms $G$ continuity and $C$ continuity.
### Geometric Continuity ($G$ Continuity)
Focuses on the geometric smoothness of curves and surfaces. 
It is less strict than $C$ Continuity because it allows [[Transformations/Transformations|transformations]] like scaling and rotation that preserve geometric properties but not necessarily the strict derivative values.
##### $G0$ Continuity
Positional continuity.
	The functions have the same position at the joining point.
**Meaning**: The curves or surfaces meet at a point, but there may be a sharp corner.
$$\LARGE f_1(c) = f_2(c)$$
##### $G1$ Continuity
Tangential continuity.
The functions have the same position and first derivative (slope) at the joining point.
**Meaning**: The curves or surfaces meet smoothly without a sharp corner, and the direction of travel is continuous.
$$\LARGE f_1(c) = f_2(c) \quad \text{and} \quad f_1'(c) = f_2'(c)\quad \text{and} \quad \mathbf{T}_1(c) = \mathbf{T}_2(c)$$
Where $T1$​ and $T2$ are the unit tangent vectors.
##### G2 Continuity
Curvature continuity.
The functions have the same position, first derivative, and second derivative (curvature) at the joining point.
**Meaning**: The curves or surfaces meet very smoothly, with no abrupt changes in the curvature.
$$ f_1(c) = f_2(c) \quad \text{and} \quad f_1'(c) = f_2'(c) \quad \text{and} \quad f_1''(c) = f_2''(c)\quad \text{and} \quad \mathbf{T}_1(c) = \mathbf{T}_2(c) \quad \text{and} \quad \kappa_1(c) = \kappa_2(c)$$
Where $κ1$​ and $\kappa_2​$ are the curvatures.
### Differential Continuity ($C$ Continuity)
Focuses on the mathematical smoothness of the functions, ensuring that derivatives up to a certain order are continuous.
	It is commonly used in mathematical and engineering analyses.
##### C0 Continuity
Positional continuity. The functions are continuous at the joining point.
**Meaning**: There is no break or jump in the value of the function at the joining point.
$$\LARGE f_1(c) = f_2(c)$$
##### $C1$ Continuity 
Tangential continuity.
The functions and their first derivatives are continuous at the joining point.
**Meaning**: The function is smooth, and there is no break or jump in the slope at the joining point.
$$\LARGE f_1(c) = f_2(c) \quad \text{and} \quad f_1'(c) = f_2'(c)$$
##### $C2$ Continuity
Curvature continuity.
The functions and their first and second derivatives are continuous at the joining point.
**Meaning**: The function is very smooth, with no break or jump in the curvature at the joining point.  
$$\LARGE f_1(c) = f_2(c) \quad \text{and} \quad f_1'(c) = f_2'(c) \quad \text{and} \quad f_1''(c) = f_2''(c)$$

- - -
## [[Discontinuities|Discontinuities]] Prevents Derivatives

### Why [[Discontinuities|Discontinuities]] (i.e. disruptions in smoothness) Prevent the Existence of a Derivative
Discontinuities prevent the existence of derivatives because the derivative is defined as the limit of the slope of secant lines as the points used to create them get infinitely close. 
- This definition **presupposes** that the **function is continuous** at the point where the derivative is being calculated.
- **Impact on Derivatives**: ^discontinuities-prevent-limits-which-prevent-deriviatives
	- Also, in actuality it is that [[Limits#Why Discontinuities Discontinuities (i.e. disruptions in smoothness) Prevent the Existence of a Limits|Discontinuities can prevent the existence of limits, which in turn means that derivatives at those points cannot be defined.]] 
		- Without a limit, there is no way to talk about the slope of the function at the point of discontinuity. 
			- You cannot have an instantaneous rate of change (derivative) where there is no consistent value for the function at that point.

When a function is discontinuous at a point, there's a break in the curve at that point. 
- Since the **derivative is the slope of the tangent line** to the curve **at a point**;
	- And a **tangent line requires a smooth passage through the point**;
		- A discontinuity creates a situation where there's no single, well-defined tangent line.

**Cusps**:
- A sudden change in direction (i.e. a sharp corner) of the curve $f(x)$ at point $a$.
	- Even though this function might be continuous:
		- The slopes of the **secant lines** from the **left and right** differ.
			- Thus the limits from the left and right are not equal.
				- Thus no unique slope (i.e. derivative) of the tangent at point $a$ exists.
- Since the [[#^c2858f|derivative is defined in terms of the limit]]:
			- If the limit does not exist for a given point, then the [[#^277add|derivative also does not exist]] for that same given point.
- If $f(x)$ is continuous without discontinuities like cusps:
	- The limits from left and right at any point, are equal.
		- Thus a derivative exists for that point, having a well defined tangent line with a slope. 
- **[[#Discontinuities|Discontinuity]]**:
	- Discontinuities in a curve are positions where the curve "jumps" from one value to another without any connecting points in between.
		- Without a continuous path:
			- There is not "approaching" the point from either side in a meaningful way.
				- Which means there's no slope of the secant to speak of.	
- **How This Affects Tangent Vector Direction:**
	- **Indeterminacy at Sharp Points**: 
		- At points where the curve has a sharp change in direction (non-differentiable points), the concept of a single, well-defined tangent line breaks down. 
			- If you tried to draw a tangent, you would find an infinite number of lines that could arguably be tangents, depending on the approach angle. 
				- This indeterminacy means there's no unique tangent vector direction at such points.
	- **Visualization with Secant Lines**: 
		- Imagine drawing secant lines (lines connecting two nearby points on the curve) and then moving these points closer together towards the point of interest. 
			- For smooth parts of the curve, as the points get infinitely close, the secant line approaches a unique position — the tangent line. 
				- However, at a sharp corner or discontinuity, the limit of the secant line's position oscillates or becomes undefined as the points get closer, indicating the absence of a well-defined tangent line and thus a tangent vector.

- - - 

## Critical Points
**Critical points** of a function are points in the domain of the function **where the first derivative is either zero or undefined**.
	These points are significant because they are potential locations where the function has local maxima, local minima, or points of inflection.
### Formal Definition
A point $x=c$ is called a **critical point** of a function $f(x)$ if one of the following conditions holds:
1. $\LARGE f'(c) = 0$
2. $\LARGE f′(c)$ does not exist
### Importance of Critical Points
#### Derivative and Critical Points
To find the turning points of a polynomial function, we take its first derivative $f'(x)$ and set it to zero to find the critical points.
	The critical points are where the slope of the function is zero, i.e., where the function could potentially change direction.
#### Degree of the Derivative
The degree of the first derivative $f'(x)$ of a polynomial function $f(x)$ of degree nnn is $n-1$.
	This means that the first derivative f'(x) is a polynomial of degree $n-1$.
#### Roots of the Derivative
A polynomial of degree $n-1$ can have at most $n-1$ real roots.
	Each real root of the first derivative corresponds to a critical point of the original function, which can be a turning point.
#### Second Derivative Test
To confirm whether a critical point is a turning point (and not a saddle point), we can use the second derivative test.
	If the second derivative $f′′(x)$ at a critical point is positive, the function has a local minimum there.
		If $f′′(x)$ at a critical point is negative, the function has a local maximum there.

- - -
#### Local Maxima and Minima
Critical points are candidates for local extrema (maxima and minima).
	By evaluating the first and second derivatives at these points, we can determine whether they are local maxima, local minima, or neither.

**Local maxima** and **local minima** are points on a function where the function reaches its highest or lowest value, respectively, within a small neighborhood around these points.
	They are important for understanding the behavior of functions and optimizing real-world problems.
##### Local Maximum
A function $f(x)$ has a **local maximum** at $x=c$ if there exists an interval $(a, b)$ containing $c$ such that:
$$\LARGE f(c) \geq f(x) \quad \text{for all} \quad x \in (a, b)$$
In other words, $f(c)$ is greater than or equal to the function values at nearby points.
##### Local Minimum
A function $f(x)$ has a **local minimum** at $x=c$ if there exists an interval $(a, b)$ containing $c$ such that:
$$\LARGE f(c) \leq f(x) \quad \text{for all} \quad x \in (a, b)$$
##### Finding Local Maxima and Minima
###### Identify Critical Points
Find the points where the first derivative $f′(x)$ is zero or undefined.
###### Second Derivative Test
Use the second derivative $f''(x)$ to determine the nature of the critical points.
    - If $f''(c) > 0$, the function has a local minimum at $x=c$.
    - If $f''(c) < 0$,, the function has a local maximum at $x=c$.
    - If $f''(c) = 0$, the test is inconclusive.

- - -
#### [[#Inflection Points|Inflection Points]] (*also see* [[Curves#Inflection Point|Inflection Points]] in Curves)
**Inflection points** are points on a function where the concavity changes.
	These points are not necessarily where the first derivative is zero but are significant in understanding the behavior and shape of the function.

***Important***: Although not all inflection points are critical points, analyzing the behavior of the function around critical points can sometimes help identify points where the concavity of the function changes.

A function $f(x)$ has an **inflection point** at $x=c$ if the concavity of the function changes at that point.
	This means the function changes from being concave up (convex) to concave down (concave) or vice versa.
	
Inflection Points indicate the **change** from **concave** to **convex** or vice versa.
	If you imagine this triangle "traveling" the length of the curve:
		The way the **orientation** of $T_2$ changes relative to $T_1$ can indicate the **concavity** of the curve.
	An [[Curves#Inflection Point|Inflection]] point is suggested if $T_2$ **rotates** from one side of $T_1$ to the other as $P_1$ and $P_2$ "travel" along the curve.

An inflection point is typically a smooth, continuous transition or change in the curvature of a function.
	![[Pasted image 20240410143446.png|500]]
	Take some $P_1 =C(s_1)$ on a curve $C$.
		$T_1$ = the **unit tangent vector** at this point $P_1$.
	$P_2$ is a point on $C$ that represents "a small movement" relative to $P_1$.
		$T_2$ = the **unit tangent vector** at this point $P_2$.
	Vector $V =T_2 - T_1$
		Notice that they combine to "make" a **triangle**.
			It represents the **rate of change** between the two points on the curve (in the function) $T_1$ and $T_2$.
				That is the approximation of the curve between $P_1$ and $P_2$.
					As the distances between $P_1$ and $P_2$ decrease, the **secant line** becomes a better approximation of the **tangent** $T_1$ at point $P_1$.
			The triangle visually describes the "smoothness" or **continuity** of a function.
				If the curve is smooth and function is differentiable at the measured points, then the tangent vectors will change gradually and not "jump".
	If $P_1$ and $P_2$ are very "close" together distance wise:
		$T_1$ and $T_2$ will be almost equal.
			Therefore, $V$ will be almost **perpendicular** (i.e. normal, orthogonal) to both $T_1$ and $T_2$.

- - -
### Identifying Critical Points
###### Identifying Inflection Points
To find inflection points of a function $f(x)$:
1. **Find the second derivative** $\LARGE f′′(x)$.
2. **Set the second derivative equal to $0$ and solve for $x$**:
    $$\LARGE f''(x) = 0$$
3. **Determine if the concavity changes around those points**:
    - If $\LARGE f′′(x)$ changes sign as $x$ passes through $c$, then $x=c$ is an inflection point.
#### Steps to Determine the Nature of Critical Points:
##### First Derivative Test:
- **Find the first derivative** of the function $f'(x)$.
- **Set the first derivative to zero** to find the critical points: $f'(x) = 0$.
- Solve for $x$ to find the critical points.
##### Second Derivative Test (if applicable):
- **Find the second derivative** of the function $f''(x)$.
- **Evaluate the second derivative at the critical points**:
	- If $f''(x) > 0$ at a critical point, the function has a **local minimum** at that point.
	- If $f''(x) < 0$ at a critical point, the function has a **local maximum** at that point.
	- If $f''(x) = 0$, the second derivative test is inconclusive; further analysis is needed.
##### Alternative Analysis (if the second derivative test is inconclusive):
- **Analyze the sign of the first derivative** on intervals around the critical points to determine whether the function is increasing or decreasing.
- **Consider higher-order derivatives** or other methods, such as the first derivative test, to determine the behavior of the function.
### Example:
Let's illustrate with a simple example:
Given the function $$\LARGE f(x) = x^3 - 3x^2 + 2$$
1. **Find the first derivative**:
    $$\LARGE f'(x) = 3x^2 - 6x$$
2. **Set the first derivative to zero and solve for $x$**:
    $$\LARGE 3x^2 - 6x = 0$$
    
    $$\LARGE 3x(x - 2) = 0$$
    
    $$\LARGE x = 0 \quad \text{or} \quad x = 2$$
    
    The critical points are $x = 0$ and $x = 2$.
    
3. **Find the second derivative**:
    $$\LARGE f''(x) = 6x - 6$$
4. **Evaluate the second derivative at the critical points**:
    - At $x = 0$:
        $$\LARGE f''(0) = 6(0) - 6 = -6 \quad (\text{negative, so } x = 0 \text{ is a local maximum})$$
    - At $x = 2$:
		$$\LARGE f''(2) = 6(2) - 6 = 6 \quad (\text{positive, so } x = 2 \text{ is a local minimum})$$

- - -
## Differential Equations
A differential equation is a mathematical equation that relates a function to its derivatives. It describes how a certain quantity changes with respect to one or more variables.

**Differential equations** are equations that involve the differentials of functions.
	They express relationships between functions and their rates of change.

**Differential Equation**: An equation involving derivatives of a function.
##### Ordinary Differential Equations (ODEs)
Involve functions of a single variable and their derivatives. For example:
    $$\frac{dy}{dx} = ky$$
This is a first-order differential equation.
    
##### Partial Differential Equations (PDEs)
Involve partial derivatives of functions of multiple variables. For example:
    $$\frac{\partial u}{\partial t} = \alpha \frac{\partial^2 u}{\partial x^2}$$
This is the heat equation, a second-order PDE.