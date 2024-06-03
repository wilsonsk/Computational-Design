---
up:
  - "[[Analysis]]"
related: 
date created: 2024-05-06
---
# Integrals
Working backwards from the derivative.
	Where instead of starting with the knowns being the position and time, we only have the graph of the derivative. 

Starting Point:
![[Pasted image 20240602153215.png]]

To get to the end point, we calculate the sum of the area under the graph.
#### $\LARGE x(t) = \sum_{i=0}^{t} v(t_{i}) \triangle t_{i}$
In this case, the sum of velocities for each time, $t_{i}$, scaled by the interval of time, $\triangle t_{i}$, which would produce a rectangle under the each velocity at time, $v(t_{i})$, with an area of such.
	Where $v(t_{i})$ is the "height" and $\triangle t$ is the "width".
		Where the times, $t_{i}$, goes from $t_{0}$ until at specific time t. 

When we add up the area of each rectangle, then we arrive at the approximate **coordinate**, $x$ at a specific time, $t$. 
	I.e. We produce, $x(t)$. 
	
End Point:
![[Pasted image 20240602153227.png]]

When we take the **[[Limits|limit]]** of the $\triangle t$ - i.e. $\LARGE \lim\limits_{\triangle t \rightarrow 0}$ we then make the rectangles themselves smaller and smaller, and thus the "graining" of the curve, finer and finer.
	And therefore, makes the approximation of the area under the function/curve/graph more accurate.

This alternate form:
#### $\LARGE \int_{t_{0}}^{t} v(\tilde{t}) d\tilde{t}$

Where $dt$ means $\triangle t$.
The $\int$ sign means, we are integrating the function $v(t)$ with respect to time.
	I.e. Means calculating the accumulated value (like displacement) that results from the continuous sum of the function's values over time.
		The integral sign ∫ tells us to sum up the values of the function over an interval of the variable, which in this case is time t.
			Which gives us the displacement s(t) (or position), assuming the initial position is zero.
###### Integral Sign (∫)
This indicates that we are summing up values of the function over a continuous range of 𝑡~t~.
###### Function v($\tilde{t}$)
This is the function we are integrating.
	The use of $\tilde{t}$ inside the function $v(\tilde{t})$ and the differential $d\tilde{t}$ specifies that $\tilde{t}$ is the variable of integration.
		 It differentiates the variable of integration from the limits of integration or any other variable in the problem.
###### Limits of Integration
The integration is performed from t0​ to t.
	These are the bounds between which the function $v(\tilde{t})$ is being integrated.
		 The lower limit is t0​, and the upper limit is t.

![[Pasted image 20240602154331.png]]
*Note: Any area under **above** the curve, is negative and thus subtracted from the sum.*

Now each $x(t_{i})$ is the area under the graph up to that specific point. 

Therefore, integrating the derivative function up to a point and then producing the output value of the function that produced that initial derivative. 

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