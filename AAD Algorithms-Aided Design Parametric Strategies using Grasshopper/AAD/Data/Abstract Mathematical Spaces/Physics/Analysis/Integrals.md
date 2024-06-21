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
## The Integral
The Integral itself represents the accumulation of quantities.
	It can be thought of as the reverse process of differentiation
![[Pasted image 20240602154331.png|500]]
*Note: Any area under **above** the curve, is negative and thus subtracted from the sum.*
### An Alternate Form:
#### $\LARGE \int_{t_{0}}^{t} v(\tilde{t}) d\tilde{t}$
Where $dt$ means $\triangle t$.
	Therefore, The equation states that we are integrating the velocity function (i.e. summing the function's output values) according to some displacement interval of the independent variable. 
Remember 
### Integral as Accumulated Area
**Integrals** can be thought of as the accumulation of quantities. 
	Now each $x(t_{i})$ is the area under the graph up to that specific point. 

*Remember*: the sum of velocities for each time, $t_{i}$, scaled by the interval of time, $dt$ (i.e. $\triangle t_{i}$), which would produce a rectangle under the each velocity at time, $v(t_{i})$, with an area of such.
	Where $v(t_{i})$ is the "height" and $dt$ (i.e. $\triangle t$) is the "width".
		Where the times, $t_{i}$, goes from $t_{0}$ until at specific time t. 

Therefore, integrating the derivative function up to a point and then producing the output value of the function that produced that initial derivative. 

The integral of a function $f(x)$ over an interval sums the values of $f(x)$ over that interval, scaled by the interval length. 
	This process can be seen as reversing differentiation.

For example, consider the integral:
$$\LARGE \int f(x) \, dx$$

If $f(x)=x$, the integral is:
$$\LARGE \int x \, dx = \frac{x^2}{2} + C$$

Here, the result is a quadratic expression. 
	This arises because integration is the inverse process of differentiation. 
		Differentiating $\LARGE \frac{x^2}{2}$ gives $x$, thus integrating $x$ gives $\LARGE \frac{x^2}{2}$
### Understanding Integral as Scaling
The integral $dt\int f(x)$ represents the sum of the values of $f(x)$ over small intervals $dt$. 
	When $f(x)=x$, summing $x$ over $dt$ leads to a quadratic function because the area under the curve $y=x$ from 0 to $x$ forms a triangle with area $\frac{1}{2} x^2$, which matches the integral result.
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
#### Variable of Integration
The variable of integration is the variable in the differential coefficient with respect to which integration is evaluated. 

It is the input variable, that is, the independent variable of a function.
	*For example, $t$ or $x$.*

The variable of integration is the variable in the Integrand, that is, the function $f(x)$, which is called the integrand.
#### Integrand
The integrand is the function or expression inside the integral that is being integrated with respect to the variable of integration.
	The integrand is the function that is being integrated in an integral.

In the expression:
#### $\LARGE \int f(x)dx$

The function $f(x)$ is the **integrand**.
The $dx$ indicates the **variable of integration**.
##### Understanding the Integrand
- **In a Definite Integral**: For a definite integral, such as
    
    $\int_{a}^{b} f(x) , dx$
    
    $f(x)$ is the integrand, and it is integrated over the interval from $x = a$ to $x = b$.
    
- **In an Indefinite Integral**: For an indefinite integral, such as
    
    $\int f(x) , dx$
    
    $f(x)$ is the integrand, and the result is a family of functions that differ by a constant of integration.
##### Integrand Example
Let's use a specific example to illustrate:

1. **Simple Function**:
    
    Consider the integral:
    
    $\int 2x , dx$
    
	 **Integrand**
		Here, the integrand is $2x$. 
			This is the function that you are integrating with respect to $x$.
	**Integrating**
		To integrate $2x$ with respect to $x$, we use the power rule for integration.
			 The [[#Power Rule for Integration|power rule]] states that:
				$\LARGE \int t^n dt = \frac{t^{n+1}}{n+1} + C for \space n \neq -1$
		 In this case, $2x$ can be written as $2 \cdot x^1$. 
			 Applying the power rule:
				1. Increase the exponent by 1: $1 + 1 = 2$
				2. Divide by the new exponent: $\frac{x^2}{2}$
	    So, integrating $2x$:
		    $\LARGE \int 2xdx = 2 \cdot {x^{2} \over 2} + C$
		Simplifying:
		    $\LARGE \int 2xdx = x^{2} + C$
			where $C$ is the [[#The Constant of Integration|constant of integration]].
	
1. **Constant Function**:
    
    For the integral:
    
    $\int -g , dt$
    
    The integrand is $-g$. In this case, $-g$ is a constant, and the variable of integration is $t$.
3. **Integrand**: 

	In this integral, $-g$ is the integrand.
		It is a constant function with respect to $t$.
    
4. **[[#Factoring Out the Constant|Factoring Constants]]**:
    
    When we factor out a constant, the integrand becomes more apparent. 
	    For example:
    
		    $\int -g , dt = -g \int 1 , dt$
    
    Here, the integrand is $1$ after factoring out the constant $-g$. 
	    This shows the linearity property of integration, where constants can be factored out of the integrand.

5. **[[#Integrating 1 with Respect to $t$|Integrating 1]] with Respect to $t$**: 

	The integral of $1$ with respect to $t$ is $t$:
	
	    $\int 1dt = t$

1. **Combining the Results**:
	
	Now, multiply the result of the integral by the constant $-g$:

		$\int 1 \, dt = -g(t + C) = -gt+ C$

Here, $C$ is the constant of integration.
#### A Constant
A constant is a fixed value that does not change with respect to the variable of integration. 
	For example, $g$ (acceleration due to gravity) is a constant with respect to time $t$.

When we [[#Constant Rule|integrate a constant]], we are essentially integrating a constant value with respect to a variable.

When you integrate a constant, the constant itself is part of the integrand. 
	Thus, in the context of the integral $\int -g , dt$, $-g$ is both a constant and the integrand.
		It is the constant value being integrated with respect to $t$.
#### The Constant of Integration
The integration constant in the context of kinematic equations is not necessarily the reference point, but it often represents initial conditions, such as initial velocity or initial position.
##### What is the Constant of Integration?
When you find the antiderivative (or indefinite integral) of a function, you are essentially reversing the process of differentiation. 
	However, when you differentiate a function, any constant term disappears because the [[Derivatives#Derivative of a Constant is Zero|derivative of a constant is zero]]. 
		This means that when you find the antiderivative, there could be any constant value added to it, and it would still be valid.
##### What Does the Constant of Integration Do?
The Constant of Integrations sets the initial state of the system at the start of the observation.
###### Represents All Possible Shifts
The constant C represents any vertical shift of the function.
	So, $x^2+5$, $x^2$, and $x^{2}−3$ all have the same slope (rate of change) at any point because they all have the same derivative2x.
###### Adjusts to Initial Conditions
If you know a specific point on the function, like $f(0)=3$, you can use this to find the exact value of C.
###### Visual Example
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
###### [[#1. Indefinite Integral aka the Antiderivative|Antiderivative]]
Refers to the inverse derivative, primitive function, primitive integral or indefinite integral of a function f.
	It is a differentiable function F whose derivative is equal to the original function f.
The Constant of Integration is produced as a by product of finding the indefinite integral (i.e. [[#1. Indefinite Integral aka the Antiderivative]]) of a function.
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
### Relationship Between Differentials and Integrals
###### [[Derivatives#Differentiation|Differentials]]
Represent infinitesimal changes in a function's variable.
###### Integrals
Sum up these infinitesimal changes to compute the total change or accumulated quantity.
##### Differentials in Integration
In the context of integration, differentials represent infinitesimal changes in the variable of integration. 
	When we write an integral, the differential indicates the variable with respect to which we are integrating. 
		For example, in the integral:
$$\int f(x) \, dx$$
The differential $dx$ signifies that we are summing up infinitesimal changes in $x$.
##### Fundamental Theorem of Calculus
This theorem bridges the concepts of differentiation and integration.
	It states that integration and differentiation are inverse processes:
###### First Fundamental Theorem:
If $F(x)$ is an antiderivative of $f(x)$, then:
$$\int_a^b f(x) \, dx = F(b) - F(a)$$
###### Second Fundamental Theorem
If $F(x)$ is an antiderivative of $f(x)$, then:
$$\frac{d}{dx} \left( \int_a^x f(t) \, dt \right) = f(x)$$
This indicates that differentiating an integral returns the original function.
###### Indefinite Integrals and Differentials
The indefinite integral (antiderivative) of a function $f(x)$ with respect to $x$ is a function $F(x)$ such that:
$$\frac{dF(x)}{dx} = f(x)$$
In terms of differentials, this can be written as:
$$dF = f(x) \, dx$$
Thus, integrating $f(x)$ with respect to $x$ can be seen as summing up the infinitesimal quantities $f(x) , dx$.
##### Example
Consider the function $f(x) = 2x$:
1. **Find the Indefinite Integral**:
$$\int 2x \, dx$$
To find the antiderivative, we look for a function $F(x)$ such that $\frac{dF(x)}{dx} = 2x$.
2. **Compute the Antiderivative**:
$$F(x) = x^2 + C$$
    Here, $x^2$ is an antiderivative of $2x$, and $C$ is the constant of integration.
3. **Differential Form**:
$$dF = 2x \, dx$$
    This shows that the differential of $F(x)$ corresponds to $f(x) , dx$.
#### Integration Constant in Kinematic Equations
When we derive the kinematic equations from the basic principles of motion, we integrate acceleration to find velocity and then integrate velocity to find displacement.

In both cases, the integration constants are determined by the initial conditions of the motion. 
	They set the initial state of the system at the start of the observation.
##### From Acceleration to Velocity:
Given constant acceleration $a$,
#### $\LARGE a=\frac{dv}{dt}$

Integrating **both sides** with respect to time $t$,
#### $\LARGE \int a \, dt=\int \frac{dv}{dt} \, dt$`

#### $\LARGE at+C_1=v(t)$

Here, $C_1$ is the integration constant, which represents the initial velocity $v_0$. 
	So, the velocity equation becomes:
#### $\LARGE v(t)=v_0+at$

$C_1$ represents the initial velocity $v_0$, which is the velocity at $t=0$.
##### From Velocity to Displacement:
Given the velocity function $v(t)=v_0+at$,
#### $\LARGE v(t)=\frac{dx}{dt}$

Integrating both sides with respect to time $t$,
#### $\LARGE \int (v_0+at) \, dt=\int \frac{dx}{dt} \, dt$
#### $\LARGE v_0 t+\frac{1}{2}at^2+C_2=x(t)$

Here, $C_2$ is the integration constant, which represents the initial position $x_0$. 
	So, the displacement equation becomes:
#### $\LARGE x(t)=x_0+v_0 t+\frac{1}{2}at^2$

$C_2$ represents the initial position $x_0$, which is the position at $t=0$.
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
And [[#Factoring Out the Constant|factoring out the constant]] $2$:

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
#### $\LARGE \int t^n dt = \frac{t^{n+1}}{n+1} + C$

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
## Other Rules of Integration
### Linearity Property of Integration
The **Linearity Property of Integration** is a fundamental property that allows us to break down integrals involving sums and constants.
	This property is crucial for simplifying and solving complex integrals.
#### Linearity Property
The linearity property of integration states that for any constants $a$ and $b$, and functions $f(x)$ and $g(x)$, the integral of a linear combination of functions is equal to the same linear combination of the integrals of those functions.
##### Rule Statement
The linearity property can be written as:
$$\LARGE \int (a f(x) + b g(x)) \, dx = a \int f(x) \, dx + b \int g(x) \, dx $$

This property shows that we can distribute the integral across terms and factor out constants.
##### Explanation and Derivation
Let's break down the linearity property step-by-step.
###### Given Integral
Consider the integral of a linear combination of functions:
$$\LARGE \int (a f(x) + b g(x)) \, dx $$

###### Distributing the Integral
According to the linearity property, we can distribute the integral across the sum:
$$\LARGE \int (a f(x) + b g(x)) \, dx = \int a f(x) \, dx + \int b g(x) \, dx $$
###### Factoring Out Constants
We can factor out the constants $a$ and $b$ from their respective integrals:
$$\LARGE \int a f(x) \, dx + \int b g(x) \, dx = a \int f(x) \, dx + b \int g(x) \, dx $$
### Examples
#### Example 1: Simple Linear Combination

Consider the integral:
$$\LARGE \int (3x^2 + 4x) \, dx $$

Here, $a=3, f(x) = x^2, b = 4, and g(x)=xg$.

1. **Distribute the Integral**:
    $$ \int (3x^2 + 4x) \, dx = \int 3x^2 \, dx + \int 4x \, dx $$
2. **Factor Out the Constants**:
    $$ \int 3x^2 \, dx + \int 4x \, dx = 3 \int x^2 \, dx + 4 \int x \, dx $$
3. **Integrate Each Term**: Using the power rule:
    $$ \int x^2 \, dx = \frac{x^3}{3} + C_1 $$$$ \int x \, dx = \frac{x^2}{2} + C_2 $$
4. **Combine the Results**:
    $$ 3 \int x^2 \, dx + 4 \int x \, dx = 3 \left( \frac{x^3}{3} + C_1 \right) + 4 \left( \frac{x^2}{2} + C_2 \right) $$
    
    Simplify:
    $$ 3 \left( \frac{x^3}{3} \right) + 4 \left( \frac{x^2}{2} \right) + 3C_1 + 4C_2 = x^3 + 2x^2 + C $$
    
    Here, $C = 3C_1 + 4C_2$ represents a combined constant of integration.

Thus:
$$ \int (3x^2 + 4x) \, dx = x^3 + 2x^2 + C $$
#### Example 2: Integral with Constants

Consider the integral:
$$ \int (5 \sin(x) - 2 \cos(x)) \, dx $$

Here, $a=5, f(x)=sin⁡(x), b=−2, and g(x)=\cos⁡(x)$

1. **Distribute the Integral**:
    $$ \int (5 \sin(x) - 2 \cos(x)) \, dx = \int 5 \sin(x) \, dx - \int 2 \cos(x) \, dx $$
    
2. **Factor Out the Constants**:
    $$ \int 5 \sin(x) \, dx - \int 2 \cos(x) \, dx = 5 \int \sin(x) \, dx - 2 \int \cos(x) \, dx $$
3. **Integrate Each Term**:
    $$ \int \sin(x) \, dx = -\cos(x) + C_1 $$$$ \int \cos(x) \, dx = \sin(x) + C_2 $$
4. **Combine the Results**:
    $$ 5 \int \sin(x) \, dx - 2 \int \cos(x) \, dx = 5 \left( -\cos(x) + C_1 \right) - 2 \left( \sin(x) + C_2 \right) $$
    Simplify:
    $$ -5 \cos(x) + 5C_1 - 2 \sin(x) - 2C_2 = -5 \cos(x) - 2 \sin(x) + C $$
    Here, $C = 5C_1 - 2C_2$​ represents a combined constant of integration.

Thus:
$$ \int (5 \sin(x) - 2 \cos(x)) \, dx = -5 \cos(x) - 2 \sin(x) + C $$
### Constant Rule
The rule of integration for constants states that the integral of a [[#A Constant|constant function]] $c$ with respect to a variable $x$ is equal to the constant multiplied by the [[#Variable of Integration|variable of integration]], plus an arbitrary [[#The Constant of Integration|constant of integration]] $C$.
###### I.e. The integral of a constant is a linear function.
Think about this...
	If say velocity is constant, then thus does not have a rate of change, because it does not change.
		Therefore, the integral of velocity, that is, position, changes linearly, that is to say, without a change in velocity.
			This is why we arrive at a linear function. 
###### Given the Integral
#### $\LARGE \int cdx$

If $f(x) = c$, where $c$ is a constant, then the integral of $f$ with respect to $x$ is:
#### $\LARGE \int c \, dx = c x + C$
##### Integrand
Here, the integrand is $c$. 
	This is a constant function with respect to $x$.
###### Integrating
To integrate a constant $c$ with respect to $x$, we use the basic rule of integration for constants. 
	The rule states that the integral of a constant $c$ with respect to $x$ is:
#### $\LARGE \int c \, dx = c \cdot x + C$
Where $C$ is the constant of integration.
- The constant $c$ is multiplied by the variable of integration $x$.
- The constant of integration $C$ is added to account for any constant that could have been present before differentiation.
#### Factoring Out the Constant 
Factoring out constants in integrals leverages the linearity property of integration, which simplifies the integration process.

When we integrate a constant, we can think of it as factoring out the constant from the integral. Here’s how it works step-by-step:
1. **Integral with Constant**:
    $\LARGE \int cdx$
2. **Factoring Out the Constant**: The constant $−g$ can be factored out of the integral.
	This is because integration is a linear operation, meaning we can factor out constants just as we do in differentiation. 
		So, we rewrite the integral as:
		    $\LARGE \int cdx = c \int 1 \, dx$
3. **[[#Integrating 1 with Respect to $t$|Integral of 1 with Respect to x]]**:
	$\LARGE \int 1dx = {x^{0+1} \over 0 + 1} + C = x + C$
4. Reintroduce the Constant $c$ and Combine Like Terms
	$\LARGE \int c \, dx  = cx + C$
##### Where the 1 (in $1dx$) Comes From
The $1$ inside the integral represents the integrand when we factor out the constant $-g$.
	In the original integral $\int c \, dx$ $c$ is the integrand. 
		When we factor $c$ out, we are left with the integral of $1$ with respect to $x$:
			$\LARGE c \int 1 \, dx$
This is because multiplying $1$ by any constant still gives the constant. 
	Therefore, we can think of the integral as integrating $1$ and then multiplying the result by $c$.
##### Why Do We Factor Out the Constant 
- **Simplification**: Factoring out constants simplifies the integrand, making the integration process easier. When a constant is factored out, the remaining integrand is often simpler to integrate.

- **Clarity**: Factoring out constants provides a clear separation between the constant multiplier and the function being integrated, which can make the integral easier to understand and solve.
###### Example
##### $\LARGE \int 5 \, dx = 5x + C$
$=5\int dx = x + C = {x^{0+1}\over 0+1} = x + C = 5x+ C$
### Constant Multiple Rule
The **Constant Multiple Rule** applies when a constant multiplies a function. 
	This rule states that if you have a constant $c$ multiplied by a function $f(x)$ inside an integral, you can factor out the constant and then integrate the function.

The Constant Multiple Rule is a property of integrals that allows you to factor out a constant from an integrand, and then integrate the remaining function.

Given $f(x) = c \cdot g(x)$, where $c$ is a constant and $g(x)$ is an integral function, then the integral of $f$ with respect to $x$ is:
#### $\LARGE \int c \cdot g(x) \, dx = c \int g(x) \, dx$
#### Factoring Out the Constant
Since $c$ is a constant, it can be factored out of the integral. This leverages the linearity property of integration:

Then the integral of $g(x)$ is calculated using the power rule.
##### Example Integral
Consider the integral:
$$\LARGE \int 3x^2 \, dx$$
##### Here, $c = 3$ is a constant and $f(x) = x^2$.
###### Step-by-Step Solution
1. **Factor Out the Constant**:
    $$\LARGE \int 3x^2 \, dx = 3 \int x^2 \, dx$$
    
2. **Integrate the Remaining Function**: Now, integrate $x^2$ with respect to $x$ using the power rule for integration. The power rule states:
    $$\LARGE \int x^n \, dx = \frac{x^{n+1}}{n+1} + C \quad \text{for} \, n \neq -1$$
    
    Applying the power rule:
    $$\LARGE \int x^2 \, dx = \frac{x^{2+1}}{2+1} + C = \frac{x^3}{3} + C$$
    
3. **Reintroduce the Constant and Combine the Results**: Multiply the result of the integral by the constant $3$:
    $$\LARGE 3 \int x^2 \, dx = 3 \left( \frac{x^3}{3} + C \right)$$
    
    Simplify:
    $$\LARGE 3 \left( \frac{x^3}{3} + C \right) = x^3 + 3C$$

    Since $3C$ is just another constant, we can write it as $C'$ or simply $C$ (since it still represents an arbitrary constant):
    $$\LARGE x^3 + C$$
$$\LARGE \int 3x^2 \, dx = 3 \int x^2 \, dx = 3 \cdot \frac{x^3}{3} + C = x^3 + C$$

### Sum Rule
If $f(x) = g(x) + h(x)$, where $g(x)$ and $h(x)$ are integral functions, then the integral of $f$ with respect to $x$ is:
#### $\LARGE \int (g(x) + h(x)) \, dx = \int g(x) \, dx + \int h(x) \, dx$
###### Example
#### $\LARGE \int (x^2 + x) \, dx = \int x^2 \, dx + \int x \, dx = \frac{x^3}{3} + \frac{x^2}{2} + C$
### Difference Rule
If $f(x) = g(x) - h(x)$, where $g(x)$ and $h(x)$ are integrable functions, then the integral of $f$ with respect to $x$ is:
#### $\LARGE \int (g(x) - h(x)) \, dx = \int g(x) \, dx - \int h(x) \, dx$
### Integration by Parts
If $f(x) = u(x) \cdot v(x)$, where $u(x)$ and $v(x)$ are differentiable functions, then the integral of $f$ with respect to $x$ is given by the integration by parts formula:
#### $\LARGE \int u(x) \cdot v'(x) \, dx = u(x) \cdot v(x) - \int u'(x) \cdot v(x) \, dx$
###### Example
#### $\LARGE \int x e^x \, dx$
Let $u = x$ and $dv = e^x , dx$. Then $du = dx$ and $v = e^x$. Applying integration by parts:
#### $\LARGE \int x e^x \, dx = x e^x - \int e^x \, dx = x e^x - e^x + C = e^x (x - 1) + C$
### Substitution Rule (Change of Variables)
If $f(x) = g(h(x)) \cdot h'(x)$, where $g$ is an integrable function of $h(x)$ and $h(x)$ is a differentiable function of $x$, then the integral of $f$ with respect to $x$ is:
#### $\LARGE \int g(h(x)) \cdot h'(x) \, dx = \int g(u) \, du$

Where $u = h(x)$.
###### Example
#### $\LARGE \int \sin(2x) \, dx$

Let $u = 2x$, then $du = 2 , dx$ or $\frac{1}{2} du = dx$. Substituting:
#### $\int \sin(2x) \, dx = \int \sin(u) \cdot \frac{1}{2} \, du = \frac{1}{2} \int \sin(u) \, du = \frac{1}{2} (-\cos(u)) + C = -\frac{1}{2} \cos(2x) + C$
### Integrating 1 with Respect to $t$
In essence, integrating 1 with respect to t essentially means finding the function whose derivative is always 1. 
	Since the [[Derivatives#Derivative of a Constant is Zero|derivative of any constant is zero]], adding a constant C doesn't affect the fact that the derivative remains 1.
###### Given
#### $\LARGE \int 1dt$
###### Power Rule
Using the power rule of integration states that the integral of $\LARGE x^n$ is $\LARGE x{(n+1)\over (n+1)}$, where $n$ is any real number except for −1.
###### Steps to Solve:
1. Apply the power rule of integration: 
	$\LARGE \int 1dt = {t^{0+1} \over 0 + 1} + C$
2. Simplify the expression: 
	$\LARGE {t^{1} \over 1} +C$
	$\LARGE = t+ C$

Therefore,
#### $\LARGE \int 1dt = t + C$ 
### Integral of Zero
Remember that Integration is the mathematical process of finding the antiderivative or the area under the curve of a function. 
	When we integrate a function, we are essentially summing up infinitely small pieces to find the total.

###### The integral of zero with respect to any variable, such as time $t$, is a constant.
This is because there is no change in the quantity we are integrating.
	I.e. The integral of zero is a constant because there is no change to accumulate over time.

Therefore, being constant means or implies that the **initial velocity** or **initial condition** or input value, remains.
	Thus, we have 
#### $\LARGE \int 0 dt = C$

Where $C$ is the Constant of Integration
##### Application to Velocity
###### Acceleration as the Derivative of Velocity
Acceleration $a_{x}$​ is the rate of change of velocity $v_{x}$​ with respect to time $t$.
	If acceleration is zero, it means that the velocity is not changing over time.
#### $\LARGE a_{x} = {dv_{x} \over dt} = 0$
###### Integrating Zero Acceleration
To find the velocity $v_{x}$​, we integrate the acceleration $a_{x}$:
#### $\LARGE v_{x}(t) = \int a_{x}dt = \int 0dt = C$

Here, $C$ is the constant of integration.
	This constant represents the initial velocity of the object, denoted as $v_{0x}$​.
		 It signifies that the velocity remains constant over time because there is no acceleration to change it.
			 Thus we write:
				 $\LARGE v_{x}(t) = v_{0x}$
##### Application to Position
###### Velocity as the Derivative of Position
Velocity $v_{x}$​ is the rate of change of position $x$ with respect to time $t$.
	Since we found that $v_{x}(t) = v_{0x}$​, we integrate this constant velocity to find the position.
#### $\LARGE x(t) = \int v_{x}(t)dt = \int v_{0x}dt$
###### Integrating Constant Velocity
#### $\LARGE x(t) = v_{0x} t + C'$

Here, $C'$ is another constant of integration, which represents the initial position of the object, denoted as $x_{0}$​.
	Therefore, we write:
		$\LARGE x(t) = v_{0x} t + x_{0}$
## Patterns of Integrals of Function Types
### Understanding Integration Patterns Through Geometric Representation
To understand why integrating different types of polynomial functions follows specific patterns, it's useful to think about the geometric interpretation of integration, which is essentially calculating the area under a curve.
#### Integration of a Linear Function
Consider a linear function $f(x) = ax + b$. 
When you integrate this function, you are finding the area under a straight line.

1. **Graph of f(x) = ax + b:
    - This is a straight line with a slope $a$ and a y-intercept $b$
2. **Integral of $f(x)=ax+b$**:
    - The integral is:
    $$\LARGE \int (ax + b) \, dx = \frac{a}{2}x^2 + bx + C$$
3. **Geometric Interpretation**:
    - The area under a linear function between two points can be visualized as a trapezoid or a series of infinitesimally small rectangles.
    - The integral $\frac{a}{2}x^2$ represents how the area changes as the width ($x$) increases quadratically, while $bx$ represents the linear contribution to the area.
#### Integration of a Quadratic Function
Consider a quadratic function $f(x)=ax2+bx+c$. 
The graph of this [[Functions and Motion#2. Quadratic Functions|function is a parabola]].
1. **Graph of $f(x)=ax^2+bx+c$**:
    - This is a parabola opening upwards or downwards depending on the sign of $a$.
2. **Integral of $f(x)=ax^2+bx+c$**:
    - The integral is:
    $$\LARGE \int (ax^2 + bx + c) \, dx = \frac{a}{3}x^3 + \frac{b}{2}x^2 + cx + C$$
3. **Geometric Interpretation**:
    - The area under the quadratic curve between two points can be visualized as the sum of areas under an infinite number of small parabolic segments.
    - The term $\frac{a}{3}x^3$ indicates that the area scales cubically as the width ($x$) increases.
    - The quadratic term in the integral ($\frac{b}{2}x^2$) represents how the area changes with the square of the width.
#### Scaling of "Height" and "Width"
When you integrate polynomial functions, you are scaling the "height" (i.e. the functions output value with respect to $x$) of each infinitesimally small rectangle under the curve with the "width" (i.e. the interval or differential of $x$). 
	
As the degree of the polynomial increases, the relationship between height and width changes:

- **Linear Function**:
    - Height increases linearly with width, so the area scales quadratically.
    $$\LARGE \int (ax + b) \, dx = \frac{a}{2}x^2 + bx + C$$
    
- **Quadratic Function**:
    - Height increases quadratically with width, so the area scales cubically.
    $$\LARGE \int (ax^2 + bx + c) \, dx = \frac{a}{3}x^3 + \frac{b}{2}x^2 + cx + C$$
    
- **Cubic Function**:
    - Height increases cubically with width, so the area scales quartically.
    $$\LARGE \int (ax^3 + bx^2 + cx + d) \, dx = \frac{a}{4}x^4 + \frac{b}{3}x^3 + \frac{c}{2}x^2 + dx + C$$
### Integral Patterns
#### 1. Polynomial Functions

When you integrate a polynomial function, you increase the power of each term by one and divide by the new power.

*For Example:*
	A linear function integrates to a Quadratic Function.
	A Quadratic function integrates to a Cubic Function.
	A Cubic function integrates to a Quartic Function.
	Etc.
- **Linear function**: $f(x) = ax + b$
	- Becomes a Quadratic Function.
    $$\LARGE \int (ax + b) \, dx = \frac{a}{2}x^2 + bx + C$$
- **General polynomial**: $f(x) = a_n x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0$
    $$\LARGE \int (a_n x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0) \, dx = \frac{a_n}{n+1} x^{n+1} + \frac{a_{n-1}}{n} x^n + \cdots + \frac{a_1}{2} x^2 + a_0 x + C$$
#### 2. Exponential Functions
For exponential functions, the integral of $e^x$ is $e^x$, and the integral of $a^x$ is related to the natural logarithm.
	I.e. Exponential functions have integrals involving themselves or logarithms.

- **Natural exponential function**: $f(x) = e^x$
    $$\LARGE \int e^x \, dx = e^x + C$$
- **General exponential function**: $f(x) = a^x$
    $$\LARGE \int a^x \, dx = \frac{a^x}{\ln(a)} + C \quad (\text{for } a > 0 \text{ and } a \ne 1)$$
#### 3. Trigonometric Functions
The integrals of basic trigonometric functions follow specific patterns.
- **Sine function**: $f(x) = \sin(x)$
    $$\LARGE \int \sin(x) \, dx = -\cos(x) + C$$
- **Cosine function**: $f(x) = \cos(x)$
    $$\LARGE \int \cos(x) \, dx = \sin(x) + C$$
- **Tangent function**: $f(x) = \tan(x)$
    $$\LARGE \int \tan(x) \, dx = -\ln|\cos(x)| + C$$
- **Secant function**: $f(x) = \sec(x)$
    $$\LARGE \int \sec(x) \, dx = \ln|\sec(x) + \tan(x)| + C$$
#### 4. Rational Functions
Integrating rational functions often involves partial fraction decomposition.
- **Example**: $f(x) = \frac{1}{x}$
    $$\LARGE \int \frac{1}{x} \, dx = \ln|x| + C$$
#### 5. Special Functions
Some functions have standard integrals that are useful to remember.
- **Inverse trigonometric functions**:
    - $f(x) = \frac{1}{\sqrt{1-x^2}}$
        $$\LARGE \int \frac{1}{\sqrt{1-x^2}} \, dx = \sin^{-1}(x) + C$$
    - $f(x) = \frac{1}{1+x^2}$
        $$\LARGE \int \frac{1}{1+x^2} \, dx = \tan^{-1}(x) + C$$