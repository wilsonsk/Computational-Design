---
up:
  - "[[Analysis]]"
related: 
date created: 2024-05-06
---
# Integrals
Integration is a fundamental concept that can be thought of as the reverse process of differentiation.
	When you see the integral sign ∫, it signifies that we are performing an operation called integration on a function.
## Derivatives Vs. Integrals
![[Pasted image 20240602190201.png]]
## Working Backwards from the Derivative.
Where instead of starting with the knowns being the position and time, we only have the graph of the derivative. 

#### Starting Point:
![[Pasted image 20240602153215.png]]

To get to the end point, we calculate the sum of the area under the graph.
#### $\LARGE x(t) = \sum_{i=0}^{t} v(t_{i}) \triangle t_{i}$
In this case, the sum of velocities for each time, $t_{i}$, scaled by the interval of time, $\triangle t_{i}$, which would produce a rectangle under the each velocity at time, $v(t_{i})$, with an area of such.
	Where $v(t_{i})$ is the "height" and $\triangle t$ is the "width".
		Where the times, $t_{i}$, goes from $t_{0}$ until at specific time t. 

When we add up the area of each rectangle, then we arrive at the approximate **coordinate**, $x$ at a specific time, $t$. 
	I.e. We produce, $x(t)$. 
	
#### End Point:
![[Pasted image 20240602153227.png]]

When we take the **[[Limits|limit]]** of the $\triangle t$ - i.e. $\LARGE \lim\limits_{\triangle t \rightarrow 0}$ we then make the rectangles themselves smaller and smaller, and thus the "graining" of the curve, finer and finer.
	And therefore, makes the approximation of the area under the function/curve/graph more accurate.

This alternate form:
#### $\LARGE \int_{t_{0}}^{t} v(\tilde{t}) d\tilde{t}$
Where $dt$ means $\triangle t$.
	Therefore, The equation states that we are integrating the velocity function (i.e. summing the function's output values) according to some displacement interval of the independent variable. 

## The Integral
The Integral itself represents the accumulation of quantities.
	It can be thought of as the reverse process of differentiation
![[Pasted image 20240602154331.png|500]]
*Note: Any area under **above** the curve, is negative and thus subtracted from the sum.*

Now each $x(t_{i})$ is the area under the graph up to that specific point. 

Therefore, integrating the derivative function up to a point and then producing the output value of the function that produced that initial derivative. 
### What "Integrate" Means
The $\int$ sign means, we are integrating the function $v(t)$ with respect to time.
	I.e. Means calculating the accumulated value (like displacement) that results from the continuous sum of the function's values over time.
		The integral sign ∫ tells us to sum up the values of the function over an interval of the variable, which in this case is time t.
			Which gives us the displacement s(t) (or position), assuming the initial position is zero.
#### Integral Sign (∫)
This indicates that we are summing up values of the function over a continuous range of 𝑡~t~.
#### Function v($\tilde{t}$)
This is the function we are integrating.
	The use of $\tilde{t}$ inside the function $v(\tilde{t})$ and the differential $d\tilde{t}$ specifies that $\tilde{t}$ is the variable of integration.
		 It differentiates the variable of integration from the limits of integration or any other variable in the problem.
#### Limits of Integration
The integration is performed from t0​ to t.
	These are the bounds between which the function $v(\tilde{t})$ is being integrated.
		 The lower limit is t0​, and the upper limit is t.

### Two Main Types of Integrals
###### 1. Indefinite Integral
The indefinite integral of a function $f(t)$ is a function $F(t)$ whose derivative is $f(t)$.
	$\LARGE ∫f(t)dt=F(t)+C$

#### The Constant of Integration
###### Integral Constant
If you write down an Integral, you will always write down an Integral Constant.

Also known as the Constant of Integration.
	It is produced as a by product of finding the indefinite integral (i.e. [[#Antiderivative|antiderivative]]) of a function.
###### Antiderivative
Refers to the inverse derivative, primitive function, primitive integral or indefinite integral of a function f.
	It is a differentiable function F whose derivative is equal to the original function f.
###### Indefinite Integral
The indefinite integral of a function f(x) is a family of functions F(x) such that F′(x)=f(x). 
	It is denoted by:
	    $f(x)dx=F(x)+C$
		    Here, C is the constant of integration.
###### Why the Constant of Integration?
When you take the derivative of a constant, it becomes zero, and is therefore not unique. 
	$\LARGE {d \over dt​}(c)=0$, where $c$ is any constant.
		Therefore, when integrating, there could be an infinite number of functions that differ only by a constant whose derivative is the same.
			 To account for all these possibilities, we include the constant C.
##### Example
Consider the function f(x)=2x. To find its indefinite integral:
1. **Set Up the Integral**:
	$∫2xdx$
2. **Find the Antiderivative**: We know that the antiderivative of 2x is x^2 (since ${dx\over d​}x^2=2x$).
	However, any function of the form $x^2+C$ where C is a constant will also have a derivative of 2x.
3. **Include the Constant of Integration**:
    $∫2xdx=x^2+C$
##### Why It Matters
The integral constant C is essential in the context of indefinite integrals because it represents the family of all possible antiderivatives of a function. 
	It ensures that the integration process accounts for all potential vertical shifts of the antiderivative function, reflecting the fact that differentiation loses this information.

- **General Solution**: The constant of integration allows us to express the general solution to an indefinite integral. Without C, we would only have a particular solution.
    
- **Initial Conditions**: In many practical problems, an initial condition or boundary condition is provided. The constant of integration is determined using this condition. For example, if you know 𝐹(0)=3F(0)=3, then you can solve for 𝐶C by substituting into 𝐹(𝑥)=𝑥2+𝐶F(x)=x2+C.


## Power Rule for Integration
One of the fundamental techniques for finding the antiderivative (or integral) of a power function. 
	It is essentially the reverse process of the power rule for differentiation.
#### $\int t^n dt = \frac{t^{n+1}}{n+1} + C$

Where C is the constant of integration. 
	This rule helps us find the antiderivative of functions of the form tn.
### Understanding the Notation
###### Function $t^n$
$t^n$ represents a power function where t is raised to the power of n.
	In integration, this is the function we are interested in integrating.
###### Differential $dt$
The $dt$ part of the integral indicates that $t$ is the variable of integration.
	It tells us that we are summing up infinitesimally small changes in the function $t^n$ over the variable $t$.
### Understanding the Rule
For a function $t^n$, where 𝑛≠−1
#### $\int t^n dt = \frac{t^{n+1}}{n+1} + C$

#### Why the Rule Works
###### [[#Antiderivative|Antiderivative]]
The integral of a function is another function whose derivative is the original function. So, if we have $\frac{t^{n+1}}{n+1}$, its derivative should give us back 𝑡𝑛tn.
#### Differentiation Check
Differentiate $\LARGE \frac{t^{n+1}}{n+1}$:

#### $\LARGE \frac{d}{dt}\left( \frac{t^{n+1}}{n+1} \right) = \frac{d}{dt}\left( \frac{1}{n+1} \cdot t^{n+1} \right)$

Using the power rule for differentiation $\left( \frac{d}{dt}(t^m) = m \cdot t^{m-1} \right)$:

$= \frac{1}{n+1} \cdot (n+1) \cdot t^{(n+1)-1} = t^n$

So, integrating 𝑡𝑛tn results in $\frac{t^{n+1}}{n+1} + C$, where 𝐶C is the constant of integration that accounts for any constant term that would disappear when differentiating.

### Example

#### Example 1: Simple Power Function

Find the integral of $t^3$.

$\int t^3 , dt$

Using the power rule:

$\int t^3 , dt = \frac{t^{3+1}}{3+1} + C = \frac{t^4}{4} + C$

#### Example 2: Another Power Function

Find the integral of 𝑡−2t−2.

$\int t^{-2} , dt$

Using the power rule:

$\int t^{-2} , dt = \frac{t^{-2+1}}{-2+1} + C = \frac{t^{-1}}{-1} + C = -\frac{1}{t} + C$

### Special Case: 𝑛=−1n=−1

For 𝑛=−1n=−1, the power rule does not apply directly because the denominator would be zero. Instead, we use a specific integral result:

$\int t^{-1} , dt = \int \frac{1}{t} , dt = \ln|t| + C$

### Summary

The power rule for integration is a straightforward method for finding the antiderivative of functions of the form 𝑡𝑛tn:

$\int t^n , dt = \frac{t^{n+1}}{n+1} + C \quad \text{for} \quad n \neq -1$

- **For 𝑛=−1n=−1**: Use $\int \frac{1}{t} , dt = \ln|t| + C$.
- **Integration** involves finding a function whose derivative gives the original function.
- **The constant 𝐶C** represents any constant value that would disappear during differentiation.

This rule is fundamental in calculus and helps solve many problems involving finding areas under curves and solving differential equations.
### Step-by-Step Solution

1. **Given Data:**
    - Initial position: x0​
    - Initial time: t0​
    - Velocity function: v(t)
    - Time of interest: t
2. **Position Function:** The position x(t) is found by integrating the velocity function
#### Example
Let's consider a specific example where the velocity function is $v(t)=3t^2$.
**Given:**
- Initial position $x_0​=0$ meters
- Initial time $t_0​=0$ seconds
- Velocity function $v(t)=3t^2$
- Time of interest t=2 seconds
![[Pasted image 20240602162742.png]]

