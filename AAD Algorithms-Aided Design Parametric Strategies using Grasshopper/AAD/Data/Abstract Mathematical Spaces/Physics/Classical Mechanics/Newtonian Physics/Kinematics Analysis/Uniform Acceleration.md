---
up:
  - "[[Kinematics Analysis]]"
related: 
date created: 2024-06-06
---
# Uniform Acceleration
## Constant Acceleration
$\LARGE a = const$ 
![[Pasted image 20240606222705.png]]![[Pasted image 20240606222714.png]]
### Linear Velocity 
Velocity Increases Linearaliy with Time
![[Pasted image 20240608095514.png]]
##### Velocity Via Integral of Acceleration
###### The [[Integrals|Integral]] of a **Constant** is a [[Secant Line#Secant Line as a Linear Function|Linear Function]].

#### $\LARGE v(t) = \int adt= at + v_{0}$

Where area is height ($a$) times width ($dt$ aka $\triangle t$), and $v_{0}$ is the [[Integrals#The Constant of Integration|Integration Constant]] (i.e. the initial velocity).

And where $at$ is the **[[Slope|slope]]** of the linear function. 
	*Note that the acceleration is $0.5$ and we can see this slope in the graph of velocity.*
##### Velocity Equation
$\LARGE v(t) = at + v_{0}$

Since $\LARGE v(t) = v_{0} + at$, if $a$ is constant, then the velocity of the object increase linearly with time. 
	This means that for each unit or interval of time, the velocity increases by a fixed amount, $a$. 
		If $a$ is constant, then $t$ is the main factor that affects $v$. 
### Quadratic Displacement
Displacement Increases Quadratically with Time
![[Pasted image 20240608102634.png]]
##### Displacement Via Integral of Velocity
#### $\LARGE x(t) = \int(at + v_{0}) dt = {1\over 2} at^{2} + v_{0}t + x_{0}$
###### Why $\frac{1}{2}at^2 = at$ 
Where going in the other direction (i.e. differentiating via [[Derivatives#Power Rule|power rule]]
*Remember: You only apply the Rules of Differentiation to the terms associated with the independent variables.*
	I.e. ${1\over 2}a$ stays as such. 
#### 1. $\LARGE \frac{d}{dt} \left( \frac{1}{2}at^2 \right) = \frac{1}{2}a \cdot \frac{d}{dt}(t^2)$
#### 2. $\LARGE \frac{d}{dt}(t^2) = 2t$
#### 3. $\frac{d}{dt} \left( \frac{1}{2}at^2 \right) = \frac{1}{2}a \cdot 2t = at$

###### Remember the [[Derivatives#Rate of Change of $t$ with Respect to Itself|Derivative of $t$ is Simply 1]]
Therefore,
#### $\LARGE v_{0}t = v_{0}$
And again, $v_{0}$ stays as such.
###### Constant of Integration
#### $\LARGE x_{0}$ 
That is the initial position.
##### Displacement Equation
$\LARGE x(t) = {1 \over 2}at^{2} + v_{0}t + x_{0}$
	Where $x(t)$ is the displacement at time, $t$, $x_{0}$ is the initial position, $v_{0}$ is the initial velocity, and $a$ is the constant acceleration.

The displacement equation shows that displacement is a function of both time $t$ and $t^{2}$.
	The term $\LARGE v_{0}t$ accounts for the initial velocity, and the term ${1 \over 2}at^{2}$ accounts for the change in velocity due to acceleration.
##### Initial Position and Velocity Contribution

$\LARGE x_{0} + V_{0}t$

This part of the equation represents the linear contribution to the displacement from the initial position and velocity.
###### Acceleration Contribution:

$\LARGE {1\over 2}at^{2}$

This part of the equation represents the contribution to the displacement due to acceleration. 
	Since this term involves $t^{2}$, it indicates that the displacement grows quadratically with time. 
		As time progresses, this term becomes more significant, leading to an increasing displacement.
###### Example
Consider an object starting from rest ($v_0 = 0$) at position $x_0 = 0$ with constant acceleration $a$:
- **Velocity**:
    - $v(t) = at$
- **Displacement**:
    - $x(t) = \frac{1}{2}at^2$
If $a = 2 , \text{m/s}^2$, then:
- At $t = 1 , \text{s}$:
    - $x(1) = \frac{1}{2} \times 2 \times 1^2 = 1 , \text{m}$
- At $t = 2 , \text{s}$:
    - $x(2) = \frac{1}{2} \times 2 \times 2^2 = 4 , \text{m}$
- At $t = 3 , \text{s}$:
    - $x(3) = \frac{1}{2} \times 2 \times 3^2 = 9 , \text{m}$
As you can see, the displacement increases more rapidly as time goes on because of the $t^2$ term.