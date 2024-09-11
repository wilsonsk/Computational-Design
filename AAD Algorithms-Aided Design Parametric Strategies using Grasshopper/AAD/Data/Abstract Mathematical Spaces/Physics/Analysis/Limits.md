---
up:
  - "[[Dynamics Analysis]]"
related:
  - "[[Curves]]"
  - "[[Data Operations]]"
  - "[[Notion of Surface Curvature]]"
  - "[[Numbers]]"
  - "[[Points]]"
  - "[[SubD Surface Patterns]]"
  - "[[Data Relationships]]"
  - "[[Derivatives]]"
date created: 2024-04-10
---
# Limits
![[Pasted image 20240909160502.png]]
## Limit i.e. *limes*
*See [[Linear Motion#Average Velocity|Linear Motion]] for more specific application of Limits.* 
### Limit as a Derivative at a Specific Point
They represent the rate of change of a function at a specific point. 
	Average Rate of Change (i.e. Slope of the Secant Line).
	Instantaneous Rate of Change (i.e. Slope of the Tangent Line).

The derivative of a function $f(x)$ at a specific point $x = a$ is defined using the limit: 
$$\LARGE f'(a) = \lim_{{h \to 0}} \frac{f(a+h) - f(a)}{h}$$​
This expression represents the instantaneous rate of change of the function at the specific point $x = a$. 
	It tells us the slope of the tangent line to the function at that point.
### Vs. [[Derivatives#Derivative as a Function|Derivative as a Function]]
The primary difference between finding the derivative at a specific point and finding the general derivative function lies in whether or not you plug in a specific value for the variable.

The derivative function $f'(x)$ represents the rate of change of $f(x)$ at any point $x$ in its domain. 
	It is defined using the same limit process, but we do not fix $x$ at a specific value. 
		Instead, we keep $x$ as a variable.
		
The derivative function $f'(x)$ represents the rate of change of $f(x)$ at any point $x$ in its domain. 
	It is defined using the same limit process, but we do not fix $x$ at a specific value. 
		Instead, we keep $x$ as a variable.
$$\LARGE f'(x) = \lim_{{h \to 0}} \frac{f(x+h) - f(x)}{h}$$
This derivative function provides a formula that can be used to find the slope of the tangent line to the function at any point in its domain.
### The Limit of a function, $f(x)$ is  $lim_{x→a​}f(x)$
A limit describes the behavior of a function as its input value (i.e. argument) approaches a particular point, or as it goes to infinity. 
Meaning the boundary or threshold.
- The mathematical concept that describes the behavior of a function (i.e. a curve) as its independent variable approaches some boundary value.
	- I.e. as one value (or point) gets closer to another point. 
![[Pasted image 20240422232308.png]]
A Limit refers to the **value** of a **function's output** as that **function's input** (i.e. a point on the function curve) approaches or gets infinitely close to some point.
	By looking at the position "now", the position slightly "later" and taking the ratio and bringing "later" as close as possible to right" now", we define a quantity that we can say is the velocity at this "instant".
	![[Pasted image 20240410151035.png]]
	![[Pasted image 20240606134026.png]]
#### *$f(a)$ is a function that maps every $x$ (i.e. point) to an $f(a)$ on a 2D graph.*
More generally a function called $f(x)$
##### *$f'(a)$ is the **[[Derivatives|derivative]]** (i.e. the [[Tangent Line#The Derivatives Is the Tangent Line The Slope of a Tangent Line Slope (i.e. a proportion/rate/ratio between $ Delta y / Delta x$) of the Tangent Line Tangent Line Slope of a Tangent Line|slope]] of the [[Tangent Line|tangent line]]) at a point where $x=a$.*
#### *$h$ (i.e. the independent variable) represents the increment or distance or interval from the point $a$ along the $x-axis$.*
- *It is used to measure how far away a point on the curve is from point $a$ when calculating the slope of the secant line.*
#### *$f(a + h) == f(\Delta a)$*
##### $f(a+h) - f(a)$ is the "rise" i.e. the Sine or the "opposite side" of the [[Secant Line#As the Proportion Visually it is the Hypotenuse of a Right Triangle Hypotenuse of the Triangle Representing the Derivatives Formally, the derivative at a point $a$, is **defined** as the Limits limit of the slope of the Secant Line secant line (i.e. **average rate of change**) Average Rate of Change|Right Triangle]] that Represents the [[Secant Line#The Average Rate of Change|Slope of the Average Rate of Change]] (i.e. the Secant Line)
Is equivalent to $\Delta f(a) == \Delta y$
$[f(a), f(a+h)]$ are the **[[Domain|bounds]]** **of** an **interval**. 
	Where $h$ is the value between the bounds.
##### $(a + h) - a$ is the "run" i.e. the Cosine or the "adjacent side" of the [[Secant Line#As the Proportion Visually it is the Hypotenuse of a Right Triangle Hypotenuse of the Triangle Representing the Derivatives Formally, the derivative at a point $a$, is **defined** as the Limits limit of the slope of the Secant Line secant line (i.e. **average rate of change**) Average Rate of Change|Right Triangle]] that Represents the [[Secant Line#The Average Rate of Change|Slope of the Average Rate of Change]] (i.e. the Secant Line) 
Is equivalent to $\Delta a == \Delta x$
$[a, a+h]$ are the **[[Domain|bounds]]** **of** an **interval**. 
	Where $h$ is the value between the bounds.

![[Pasted image 20240422232413.png]]
##### Local Behavior at a Single Point
$$\lim_{h\to 0}$$
- *As $h$ approaches zero (i.e. zero distance between a point and point $a$), the secant line approaches the tangent line $T_a$ for point $a$*.
	- This is considered **local behavior at a point**.
##### Global Behavior of a Function
 $$\lim_{h\to \infty}$$
	- *Can also approach infinity, but the secant line does not to converge to a single point like when h approaches zero.*
		- *Instead as h grows, the secant line continues to connect increasingly distant points, spanning a large interval.*
		- This is considered **global behavior of a function**.
## The Limit as a Means of [[Derivatives^limits-as-a-transitions|Transition]]
Between the **average rate of change** to the **instantaneous rate of change**. 
- Mathematically, the [[Derivatives^limits-as-a-transitions|derivative]] at a point is defined as the **limit** of the **difference quotient** (the slope of the secant line) as the interval (distance between two values/points) **approaches zero**.
	- Therefore, if this limit exists at this point, then the function is **differentiable** at that point.
		- And the slope of the tangent line at this point is precisely the value of this limit itself - which is the derivative of that point.
## Limits and Derivatives
**Limits** are foundational to the concept of derivatives. 
##### Limit
Defines the concept of instantaneous change.
##### [[Derivatives|Derivative]]
Uses the limit to define the rate of change of the function.
##### [[Derivatives#Differentiation|Differential]]
Applies the derivative to approximate changes in the function values.
##### [[Integrals|Integral]]
Summarizes or accumulates the infinitesimal changes, essentially performing the inverse operation of differentiation.
#### The Concept of the Derivative
The derivative of a function $f$ at a point $x$ how $f(x)$ changes as $x$ changes. 
	This is essentially the slope of the tangent line to the function at that point.
##### Secant Line
The [[Secant Line|Secant Line]] is a [[Linear Functions|Linear Function]] that connects two points on a curve.
$$\LARGE y=mx+b$$
The [[Linear Functions#Slope as a Rate of Change|Slope]] of the Secant Line, $\LARGE m$ gives an average rate of change between those two points.
	The slope $m$ represents the rate of change of $y$ with respect to $x$.
		This means that for each unit increase in $x$, the value of $y$ changes by $m$ units.
###### Average Rate of Change (i.e. Slope of the Secant Line)
For a small increment $\Delta x$, the average rate of change of $f$ over the interval from $x$ to $x+ \Delta x$ is:
$$\LARGE \frac{f(x + \Delta x) - f(x)}{\Delta x}​$$

This represents the slope of the secant line connecting the points:
##### Using the Limit to Define the Derivative
The derivative of a function at a point is defined as the limit of the average rate of change (slope of the secant line) as the interval approaches zero.


As the two points get closer to each other, the secant line approaches the [[Tangent Line|tangent line]] at a single point on the curve.
###### Instantaneous Rate of Change (i.e. Slope of the Tangent Line)
The derivative focuses on the instantaneous rate of change. 
	To find this, we consider what happens as $\Delta x$ becomes infinitesimally small.

The Limit Process converts the Secant Line into a Tangent Line.
	That is, by taking the Limit of the Slope of the Secant line as $\Delta x$ approaches $0$, it produces the Slope of the Tangent Line, which is the Derivative, $f'(x)$, of the function, $f(x)$.
		Mathematically, the derivative, $f'(x)$ of a function $f(x)$ at a point $x$ is given by:

$$\LARGE f′(x)= \lim_{\Delta x \to 0} \frac{f(x + \Delta x) - f(x)}{\Delta x}$$

Here, the limit captures the idea of an instantaneous rate of change.

When $x_2$​ approaches $x_1$​, this slope approaches the derivative of $f$ at $x_1$, which is the slope of the tangent line at that point.
	In the limit as $x_2$ approaches $x_1$​, the secant line becomes the tangent line. 
		This is represented as:
			$$\LARGE \lim_{x_2 \to x_1} \frac{f(x_2) - f(x_1)}{x_2 - x_1} = f'(x_1)$$
## Limits Define Continuity or [[Discontinuities|Discontinuity]]
### [[Continuities|Continuity]]
Continuity at a point means that there is **no** interruption in the curve (i.e. function) at that point. 
- For a function to be continuous at a point $a$, three conditions must be met:
	1. **The function $f(x)$ is defined at point $a$.**
		- I.e. There exists an output value $f(a)$.
	2. **The limit exists at point $a$.**
		![[Pasted image 20240410233411.png]]
		- I.e. The left-hand limit (as $x$ approaches $a$ from the left) and the right-hand limit (as $x$ approaches $a$ from the right) both exist and are equal.
			- Here, $h$ (i.e. the independent variable representing distance or interval between $x$ and $a$) can approach zero from negative values (left-hand limit) or from the positive values (right-hand limit).
				- This means that as you get closer to $a$ from either side, the function's output values approach the same number.
	1. **The function's output value at $a$ equals the limit at $a$**.
		- I.e. The **value** $f(a)$ is **equal** to the **limit** of $f(x)$ as **$x$ approaches $a$**.
#### Non-Differentiability Without Discontinuity
A function can be continuous but not [[Derivatives#Differentiability|differentiable]] at a point. 
- This happens when the function's graph has a sharp turn or cusp at that point. 
	- Even though the function does not break or jump, the direction of the graph changes so abruptly that there is no single tangent line that can be drawn at that point. 
##### How [[Derivatives#Differentiability|differentiability]] relates to the rate of change:
- **Average Rate of Change (i.e. slope of the [[Secant Line|secant line]]): 
	- **If we look at the slopes of secant lines near a point of interest on the curve, the average rate of change is represented by these slopes.** 
		- **If the slopes of the secant lines from either side of the point do not converge to the same value as they get infinitely close to the point (i.e. as $h$ gets smaller, this suggests that the derivative (instantaneous rate of change) at the point does not exist**.		
- I.e. If the limit doesn't exist for a point, it means:
	- The function's (i.e. curve's) behavior is **too erratic** at that point to be **captured by a single number** (i.e. the slope of the tangent- the derivative).
		- Therefore, the function is not [[Derivatives#Differentiability|differentiable]] at that point.
			- Meaning no well defined instantaneous rate of change at that point.
### [[Discontinuities|Discontinuity]]
Discontinuity at a point means there is a **sudden change in direction**, an **interruption in the smoothness**, or a **break** in the curve itself. 
- When the left-hand and right-hand limits are not equal, it means there's a jump in the function at point $a$ (i.e. where $x=a$.) 
	- The function is approaching different values from the left and right as you get closer to $a$.
		- So there is no single value that $f(x)$ is approaching. 
			- As a result, the overall limit at $a$ does not exist.
				- And **for a derivative to exist at point $a$, this limit must exist** for that point (and be the **same value** **irrespective of the direction** from which **$h$ approaches zero)**.
#### Why [[Discontinuities|Discontinuities]] (i.e. disruptions in smoothness) Prevent the Existence of a Limits
Discontinuities create a break in the function that disrupts the foundational requirement for limits, and since derivatives are defined in terms of limits, a discontinuity at a point means you cannot have a derivative at that point. 
- The prevention of derivatives due to discontinuities is a direct consequence of the definition of a derivative requiring a well-defined limit.

**Limits Require Consistency**: 
- For a limit to exist at a certain point, the function must approach the same value from both the left and the right of that point. 
	- This is the concept of the limit being 'well-defined'.

**Discontinuities Break Consistency**: 
- A discontinuity at a point means that there is a break in this consistency.
	- There could be a jump in the function values ([[Discontinuities#Jump Discontinuity|jump discontinuity]]), or the function could go off to infinity ([[Discontinuities#Infinite Discontinuity|infinite discontinuity]]), or the function could simply not be defined at the point ([[Discontinuities#Removable Discontinuity|removable discontinuity]]).

**[[Derivatives|Derivatives]] Rely on Limits**: 
- The derivative at a point is defined as the limit of the slope of the secant lines as the interval between the points on the lines approaches zero. 
	- [[Derivatives#^discontinuities-prevent-limits-which-prevent-deriviatives|If the limit doesn't exist because the function isn't approaching the same value from both sides, then the derivative cannot be defined.]]

**Impact on Derivatives**: 
- Without a limit, there is no way to talk about the slope of the function at the point of discontinuity. 
	- You cannot have an instantaneous rate of change (derivative) where there is no consistent value for the function at that point.
#### Both Non-Differentiability and Discontinuities "Break Consistency of a Limit at a Point"
But they do so in **different ways**.
##### Discontinuity:
- **Definition**: 
	- A discontinuity at a point $x=a$ occurs when a function does not have a well-defined limit at that point, or the limit exists but does not equal the function's value at $a$ (if it's defined at all).
- **Detection**:
    - **Graphical Method**: Look for breaks, jumps, or holes in the graph at $x=a$.
    - **Limit Analysis**: Check if the left-hand limit and the right-hand limit are equal. 
	    - If they are not, or if one or both do not exist, $f(x)$ is discontinuous at $a$. 
		    - Also, if the limits are equal but not equal to $f(a)$ (the actual function value at $a$, if defined), then $f(x)$ has a [[Discontinuities#Removable Discontinuity|removable discontinuity]] there.
##### Non-Differentiability:
- **Definition**: 
	- A point of non-differentiability on a curve is a point where the function is continuous (no breaks, jumps, or holes) but does not have a well-defined tangent line (and hence, no derivative) at that point. 
		- This usually happens at sharp corners or [[Discontinuities#^2b891a|cusps]].
- **Detection**:
    - **Graphical Method**: Look for sharp corners or cusps in the graph where the direction of the curve changes abruptly, but there is no break in the graph.
    - **Derivative Analysis**: If the function is continuous at $x=a$ but the limit defining the derivative, does not exist due to a change in the slope of secant lines that does not stabilize as $h$ approaches zero, the function is non-differentiable at $a$.
##### Key Distinctions:
- **Continuity First**: 
	- To be non-differentiable at a point, a function must first be continuous at that point. 
		- If it's discontinuous, questions of differentiability at that point don't apply.
- **Behavior of Limits**: 
	- For discontinuities, the issue is with the function's limit(s) not matching the function's value or not existing. 
		- For non-differentiability, the limit defining the derivative does not exist due to the slope changing abruptly, even though the function itself smoothly passes through the point.
## Limit of the Average Rate of Change
###### Velocity
The rate of change of the **position** of some object.
### Average Velocity
#### Average Velocity = $\bar V = dx/dt$
$dx$ is $\Delta x$ Delta $x$ - i.e. the change in the $x$ value.

$\Delta x$ is also $\Delta f(t)$ which is the change of the output of the function $f(t)$ as $t$ value changes. 

In the most general, $\Delta x = \Delta f(t) = \Delta f(x) = y$  
	So $\bar V = dx/dt = \Delta x / \Delta t = \Delta f(x) / \Delta t = \Delta y / \Delta x$

$dt$ is $\Delta t$ Delta $t$ - i.e. the change in the $t$ (**time**) value.
	$dx$, $dt$ imply velocity, which is a function $v(t)$.

![[Pasted image 20240422144312.png|400]]

$\Delta x / \Delta t$ is the **slope** a straight line that connects the two points.
	As these two points get "closer", the straight line connecting them, would become **[[Tangent Line|tangent]]** to the curve. 
	Therefore, the **direction** of the **velocity vector** at **[[Derivatives|any point]]** in the curve, is **[[Tangent Line|tangent]]** to the curve at that point. 
	The Tangent of this angle (the angle formed by the line from the "initial" point to the "changed point" and the line parallel to the $x-axis$, is $\Delta y / \Delta x$ i.e. $dx/dt$.
	
The **Limit** of the **average rate (i.e. average velocity)** is
$v(t) = \Delta x / \Delta t = dx/dt=$ $$\lim_{\Delta t\to 0}\Delta x / \Delta t$$
	"As $t$ approaches 0" means:
		 The [[#*$h$ (i.e. the independent variable) represents the **increment or distance** from the point $a$ along the $x-axis$.*|increment]] between two $t$ values on the $x-axis$ gets infinitely smaller, i.e. approaches zero distance between them. 

## Limit Definition of a Derivative (i.e. Calculating Derivatives via Limits) 
Plug in $(f(x + h))$ for every $x$ variable, then simplify $f(x + h) - f(x)$ then solve $\lim\limits_{h \to 0}\frac{f(x + h) - f(x)}{h}$
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
### Two Approaches
Limits or [[Derivatives#Rules of Differentiation|Rules of Differentiation]]
### Using Limits vs. Differentiation Rules
- **Using Limits**: When you first learn about derivatives, you start by using the limit definition to understand the fundamental concept. 
- **Using [[Derivatives#Rules of Differentiation|Differentiation Rules]]**: Once the differentiation rules are understood, you apply them directly without computing limits each time. 
### Basic Steps to Calculate Limits
1. **Direct Substitution**:
    - The simplest method is to substitute the value of the variable directly into the function. If $f(x)$ is continuous at $x = a$, then $\lim_{x \to a} f(x) = f(a)$.
2. **Factoring**:
    - If direct substitution results in an indeterminate form (like $\frac{0}{0}$), factor the function and simplify. This can often resolve the indeterminate form.
    - $\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{(x-a)h(x)}{(x-a)k(x)} = \lim_{x \to a} \frac{h(x)}{k(x)}$
    - if $(x-a)$ cancels out.
3. **Rationalizing**:
    - For functions involving square roots or other roots, multiply the numerator and denominator by the conjugate to rationalize.
    - $\lim_{x \to a} \frac{\sqrt{f(x)} - \sqrt{g(x)}}{h(x)} \text{ multiply by } \frac{\sqrt{f(x)} + \sqrt{g(x)}}{\sqrt{f(x)} + \sqrt{g(x)}}$
4. **L'Hôpital's Rule**:
    - If a limit results in an indeterminate form like $\frac{0}{0}$ or $\frac{\infty}{\infty}$, use L'Hôpital's Rule, which involves differentiating the numerator and the denominator.
    - $\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)}$
5. **Squeeze Theorem**:
    - If you can bound $f(x)$ between two other functions $g(x)$ and $h(x)$ that have the same limit at $a$, then $f(x)$ also approaches that limit.
    - $g(x) \leq f(x) \leq h(x) \text{ and } \lim_{x \to a} g(x) = \lim_{x \to a} h(x) = L \implies \lim_{x \to a} f(x) = L$
### Examples
1. **Direct Substitution**:
    - $\lim_{x \to 2} (3x + 4) = 3(2) + 4 = 10$
2. **Factoring**:
    - $\lim_{x \to 1} \frac{x^2 - 1}{x - 1} = \lim_{x \to 1} \frac{(x - 1)(x + 1)}{x - 1} = \lim_{x \to 1} (x + 1) = 2$
3. **Rationalizing**:
    - $\lim_{x \to 4} \frac{\sqrt{x} - 2}{x - 4} \text{ multiply by } \frac{\sqrt{x} + 2}{\sqrt{x} + 2} = \lim_{x \to 4} \frac{(\sqrt{x} - 2)(\sqrt{x} + 2)}{(x - 4)(\sqrt{x} + 2)} = \lim_{x \to 4} \frac{x - 4}{(x - 4)(\sqrt{x} + 2)} = \lim_{x \to 4} \frac{1}{\sqrt{x} + 2} = \frac{1}{4}$
4. **Using L'Hôpital's Rule**:
    - $\lim_{x \to 0} \frac{\sin x}{x} = \lim_{x \to 0} \frac{\cos x}{1} = 1$
5. **Squeeze Theorem**:
    - $\lim_{x \to 0} x^2 \sin \left(\frac{1}{x}\right) = 0$
    - because $-x^2 \leq x^2 \sin \left(\frac{1}{x}\right) \leq x^2$ and $\lim_{x \to 0} -x^2 = \lim_{x \to 0} x^2 = 0$.
