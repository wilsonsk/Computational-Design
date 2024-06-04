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
#### The Constant of Integration
##### What is the Constant of Integration?
When you find the antiderivative (or indefinite integral) of a function, you are essentially reversing the process of differentiation. 
	However, when you differentiate a function, any constant term disappears because the [[Derivatives#Derivative of a Constant is Zero|derivative of a constant is zero]]. 
		This means that when you find the antiderivative, there could be any constant value added to it, and it would still be valid.
##### What Does the Constant of Integration Do?
###### Represents All Possible Shifts
The constant C represents any vertical shift of the function.
	So, $x^2+5$, $x^2$, and $x^{2}−3$ all have the same slope (rate of change) at any point because they all have the same derivative2x.
###### Adjusts to Initial Conditions
If you know a specific point on the function, like $f(0)=3$, you can use this to find the exact value of C.
##### Visual Example
Imagine you have a curve representing the function $x^{2}+C$. 
	The constant C can shift this curve up or down on the graph, but the shape of the curve remains the same because the rate of change (slope) at any point is still determined by the derivative 2x.
##### Why Do We Add the Constant of Integration?
###### Reversing Differentiation
When you differentiate $x^2+5$ and $x^2−3$, both give you $2x$. 
	So, when you integrate $2x$, you need to account for all possible constants that could have been there before differentiation. 
		This is why we add a constant C.
###### Family of Functions
The antiderivative represents a family of functions, all differing by a constant. 
	Adding the constant C ensures we include all possible functions that could have been differentiated to give the original function.
###### Integral Constant
If you write down an Integral, you will always write down an Integral Constant.

Also known as the Constant of Integration.
	It is produced as a by product of finding the indefinite integral (i.e. [[#1. Indefinite Integral aka the Antiderivative]]) of a function.
###### [[#1. Indefinite Integral aka the Antiderivative|Antiderivative]]
Refers to the inverse derivative, primitive function, primitive integral or indefinite integral of a function f.
	It is a differentiable function F whose derivative is equal to the original function f.
###### [[#1. Indefinite Integral|Indefinite Integral]]
The indefinite integral of a function f(x) is a family of functions F(x) such that F′(x)=f(x). 
	It is denoted by:
	    $f(x)dx=F(x)+C$
		    Here, C is the constant of integration.
###### Why the Constant of Integration?
When you take the derivative of a constant, it becomes zero, and is therefore not unique. 
	$\LARGE {d \over dt​}(c)=0$, where $c$ is any constant.
		Therefore, when integrating, there could be an infinite number of functions that differ only by a constant whose derivative is the same.
			 To account for all these possibilities, we include the constant C.
##### Steps to Determine the Constant of Integration
1. **Integrate the given function to find the general antiderivative.**
2. **Use the initial or boundary condition to solve for the constant of integration.**
###### Example of Calculating the Constant of Integration
Suppose the acceleration function is $\LARGE a(t)=6t$ and we know the initial velocity $\LARGE v(0)=4$.
1. **Integrate the acceleration function to find the velocity function:**
	
	$\LARGE v(t) = \int 6t \, dt$
	
1. Using the [[#Power Rule for Integration|power rule for integration]]:
	
	$\LARGE \int 6t \, dt = 6 \cdot \frac{t^{1+1}}{1+1} = 6 \cdot \frac{t^2}{2} = 3t^2$
	
	So, the general antiderivative is:

		$\LARGE v(t) = 3t^2 + C$
		
1. **Use the initial condition to solve for C:**
	Given 𝑣(0)=4v(0)=4
	
		$\LARGE 4 = 3(0)^2 + C \implies C = 4$
	
	Therefore, the specific velocity function is:

		$\LARGE v(t) = 3t^2 + 4$

##### Why It Matters
The integral constant C is essential in the context of indefinite integrals because it represents the family of all possible antiderivatives of a function. 
	It ensures that the integration process accounts for all potential vertical shifts of the antiderivative function, reflecting the fact that differentiation loses this information.

- **General Solution**: The constant of integration allows us to express the general solution to an indefinite integral. Without C, we would only have a particular solution.
    
- **Initial Conditions**: In many practical problems, an initial condition or boundary condition is provided. The constant of integration is determined using this condition. For example, if you know 𝐹(0)=3F(0)=3, then you can solve for 𝐶C by substituting into 𝐹(𝑥)=𝑥2+𝐶F(x)=x2+C.
### Two Main Types of Integrals
##### 1. Indefinite Integral aka the Antiderivative 
The indefinite integral (i.e. the antiderivative) of a function $f(t)$ is a function $F(t)$ whose derivative is $f(t)$.
	This means that F(t) is a function whose rate of change at any point t is given by f(t). The process of finding an antiderivative is called integration.
		*For example, velocity is the antiderivative of acceleration.*

$\LARGE ∫f(t)dt=F(t)+C$

Where:
- ∫ is the integral sign.
- f(t) is the integrand, the function being integrated.
- dt indicates that t is the variable of integration.
- F(t) is the antiderivative or the integral of f(t).
- C is the constant of integration, representing an arbitrary constant since the differentiation of a constant is zero.
###### Example of Finding the Antiderivative
Consider the function f(x)=2x. To find its indefinite integral:
1. **Set Up the Integral**:
	$∫2xdx$
2. **Find the Antiderivative**: We know (via [[#Power Rule for Integration|the Power Rule For Integration]]) that the antiderivative of 2x is x^2 (since ${dx\over d​}x^2=2x$).
	However, any function of the form $x^2+C$ where C is a constant will also have a derivative of 2x.
3. **Include the Constant of Integration**:
    $∫2xdx=x^2+C$
###### Antiderivative and the [[#The Constant of Integration|Constant of Integration]]
When finding an antiderivative, we include an arbitrary constant C because the derivative of a constant is zero. 
	This means there are infinitely many antiderivatives for a given function, each differing by a constant. 
###### Properties of Antiderivatives
1. **Linearity**:
    - The antiderivative of a sum is the sum of the antiderivatives:
        $\LARGE ∫[f(t)+g(t)]dt=∫f(t)dt+∫g(t)dt$
    - The antiderivative of a constant multiple is the constant multiple of the antiderivative:
        $\LARGE ∫c⋅f(t)dt=c⋅∫f(t)dt$
2. **Basic Antiderivatives**:
    - Power Rule:
        $\LARGE ∫t^{n}dt={t^{n+1}\over n+1} + C$ for $n\neq -1$
    - Exponential Rule:
        $\LARGE ∫e^{t}dt=e^{t}+C$
    - Constant Rule:
        $\LARGE ∫cdt=ct+C$
###### Antiderivative Example 1: Simple Power Function

Consider the function $\LARGE f(t)=2t$:

1. **Find the Antiderivative**:
	$\LARGE F(t) = \int 2t \, dt$
1. **Apply the Power Rule for Integration**:
    $\LARGE \int 2t \, dt = 2 \cdot \frac{t^{1+1}}{1+1} = 2 \cdot \frac{t^2}{2} = t^2$
3. **Include the Constant of Integration**:
    $\LARGE \int 2t \, dt = t^2 + C$

So,  $\LARGE F(t)=t^{2}+C$ is an antiderivative of $\LARGE f(t)=2t$.

###### Antiderivative Example 2: Exponential Function

Consider the function $f(t)=e^t$:

1. **Find the Antiderivative**:
	 $\LARGE F(t) = \int e^t \, dt$

3. **Use the Fact that the Derivative of $e^t$ is $e^{t}$**:
	$\LARGE \int e^t \, dt = e^t + C$


So, $\LARGE F(t)=e^{t}+C$ is an antiderivative of $\LARGE f(t)=e^{t}$.

###### Antiderivative Example: Velocity as the Antiderivative of Acceleration
###### Mathematical Explanation
**Acceleration**:
- Acceleration a(t) is the rate of change of velocity with respect to time.
- Mathematically, this is expressed as: $\LARGE a(t)={dv(t)\over dt}​$
**Velocity**:
- Velocity v(t) is the antiderivative of acceleration.
- To find v(t), you integrate a(t): $\LARGE v(t)=∫a(t)dt+C$
- Here, C is the constant of integration, which can be determined if you have an initial condition, such as the initial velocity.

Suppose the acceleration function is $\LARGE 𝑡a(t)=6t$:
1. **Find the velocity function**:

	$\LARGE v(t) = \int 6t \, dt$

2. **Integrate using the power rule**:
    
	$\LARGE \int 6t \, dt = 6 \cdot \frac{t^{1+1}}{1+1} = 6 \cdot \frac{t^2}{2} = 3t^2$

3. **Include the constant of integration**:
    
	$\LARGE v(t) = 3t^2 + C$

###### Determining the Constant of Integration

To find the constant C, you need an initial condition, such as the initial velocity v(0):

- Suppose the initial velocity is $\LARGE v(0)=4$. 

So, the velocity function is:

	$\LARGE 4 = 3(0)^2 + C \implies C = 4$
##### 2. Definite Integral
The definite integral of a function f(t) from a to b is the total accumulation of the function's values over the interval [𝑎,𝑏][a,b].

$\LARGE \int_{a}^b​ f(t)dt$

Where:
- a and b are the [[#Limits of Integration|limits of integration]].
- The definite integral gives a single numerical value, representing the net area under the curve of f(t) from t=a to t=b.
	- I.e. It represents the accumulated values (sum) of each function output value scaled by a factor of the interval between output values. 
###### Example 1: Indefinite Integral

Find the indefinite integral of 2t.

$∫2tdt$

Using the power rule for integration:

$∫2tdt=2∫tdt=2⋅1+1t1+1​=2⋅2t2​=t2+C$

So,

∫2tdt=t2+C
###### Example 2: Definite Integral

Find the definite integral of t^2 from 1 to 3.

$\LARGE \int_{1}^3​ t^2dt$

First, find the antiderivative of t2:

$\int t^2dt={t^3\over 3}​+C$

Then, evaluate it from 1 to 3:

$\LARGE {t^3\over 3}_{​​1}^3​={3^3\over 3}​−{1^3\over 3}​={27\over 3}​−{1\over 3}​=9−{1\over 3}​=8.67$
### Fundamental Theorem of Calculus

The Fundamental Theorem of Calculus links the concept of differentiation and integration, and it has two parts:
##### Part 1: The Connection Between Differentiation and Integration
This part states that if F is an [[#Antiderivative|antiderivative]] of f on an interval [𝑎,𝑏][a,b], then the integral of f over [𝑎,𝑏][a,b] is given by:
	$\LARGE \int_{a}^b ​f(t)dt=F(b)−F(a)$

- **Interpretation**: This part tells us that the definite integral of a function f from a to b can be found by evaluating its antiderivative F at the endpoints and taking the difference.
- **Implication**: It provides a powerful way to compute definite integrals using antiderivatives, simplifying the process of finding areas under curves.
##### Part 2: The Existence of Antiderivatives
This part states that if f is a continuous function on [𝑎,𝑏][a,b], then the function F defined by:

	$\LARGE F(t)=\int_{a}^t ​f(x)dx$

That function F is differentiable on $(a,b)$, and $F′(t)=f(t)$.

- **Interpretation**: This part tells us that if f is continuous on [𝑎,𝑏][a,b], then the function F defined by the integral of f from a to t is differentiable, and its derivative is f.
- **Implication**: It guarantees that continuous functions have antiderivatives, establishing the foundation for solving differential equations and understanding the accumulation of quantities.
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
	We simple "add" 1 to the exponent and we divide the result by that same summed exponent.
#### $\int t^n dt = \frac{t^{n+1}}{n+1} + C$

#### Why the Rule Works
###### [[#Antiderivative|Antiderivative]]
The integral of a function is another function whose derivative is the original function. So, if we have $\frac{t^{n+1}}{n+1}$, its derivative should give us back 𝑡𝑛tn.
#### Differentiation Check
Differentiate $\LARGE \frac{t^{n+1}}{n+1}$:

#### $\LARGE \frac{d}{dt}\left( \frac{t^{n+1}}{n+1} \right) = \frac{d}{dt}\left( \frac{1}{n+1} \cdot t^{n+1} \right)$

Using the power rule for differentiation $\left( \frac{d}{dt}(t^m) = m \cdot t^{m-1} \right)$:

$= \frac{1}{n+1} \cdot (n+1) \cdot t^{(n+1)-1} = t^n$

So, integrating $t^n$ results in $\frac{t^{n+1}}{n+1} + C$, where C is the constant of integration that accounts for any constant term that would disappear when differentiating.

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

#### Example of a Special Case: 𝑛=−1n=−1

For 𝑛=−1n=−1, the power rule does not apply directly because the denominator would be zero. Instead, we use a specific integral result:

$\int t^{-1} , dt = \int \frac{1}{t} , dt = \ln|t| + C$
##### Summary of Power Rule of Integration

The power rule for integration is a straightforward method for finding the antiderivative of functions of the form 𝑡𝑛tn:

$\int t^n , dt = \frac{t^{n+1}}{n+1} + C \quad \text{for} \quad n \neq -1$

- **For n=−1**: Use $\int \frac{1}{t} , dt = \ln|t| + C$.
- **Integration** involves finding a function whose derivative gives the original function.
- **The constant C** represents any constant value that would disappear during differentiation.

This rule is fundamental in calculus and helps solve many problems involving finding areas under curves and solving differential equations.
### Step-by-Step Solution Using the Power Rule of Integration

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

