# Linear Motion
Linear motion refers to motion along a straight line, but it does not specify whether the speed is constant. 
	Linear motion can involve varying speed, constant speed, or even accelerated motion along a straight path.

This "straight line" implies motion along a **single axis**.
	Where a [[#Position|position]] changes along a single axis. 
		This does **not** mean that the velocity or acceleration are necessarily straight graphically.
## Position
Position refers to the specific location of an object in space at a given point in time.
	It is described relative to a reference point, typically called the origin, in a coordinate system.
##### Change of Position as Displacement
When we derive the kinematic equations from the basic principles of motion, we integrate acceleration to find velocity and then integrate velocity to find displacement.
#### Positions are Represented by [[Static Equilibrium#Position Vectors|Position Vectors]].
**Mathematical Representation**:
In a one-dimensional space, position $x(t)$ is a function of time $t$.

In a two-dimensional space, position is represented by a vector
$\LARGE \vec{r}(t) = x(t) \hat{i} + y(t) \hat{j}$

In a three-dimensional space, position is represented by a vector
$\LARGE \vec{r}(t) = x(t) \hat{i} + y(t) \hat{j} + z(t) \hat{k}$
where $\hat{i}$, $\hat{j}$, and $\hat{k}$ are the unit vectors along the $x$, $y$, and $z$ axes respectively.
### Position as the Basis for Velocity
###### [[Newton's Second Law#Velocity|Velocity]]:
Velocity is defined as the rate of change of position with respect to time.
It describes how fast and in which direction an object's position is changing.

**Mathematical Definition**:
The [[#Velocity Vector|velocity vector]] $\vec{v}(t)$ is the first derivative of the position vector $\vec{r}(t)$ with respect to time: 
$\LARGE \vec{v}(t) = {d\vec{r}(t) \over dt}$

**Components**:
In one-dimensional motion, velocity is the derivative of the position function: 
$\LARGE v(t) = \frac{dx(t)}{dt}$
    
In two-dimensional motion, velocity is the derivative of the position vector: 
$\LARGE \vec{v}(t) = \frac{d}{dt} (x(t) \hat{i} + y(t) \hat{j}) = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j}$
    
In three-dimensional motion, velocity is: 
$\LARGE \vec{v}(t) = \frac{d}{dt} (x(t) \hat{i} + y(t) \hat{j} + z(t) \hat{k}) = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} + \frac{dz(t)}{dt} \hat{k}$
### Example
Let's consider an example in two-dimensional motion:
###### Position Vector: Suppose the position vector of a particle is given by: 
$\LARGE \vec{r}(t) = t^2 \hat{i} + t^3 \hat{j}$
###### Velocity Vector: The velocity vector is the derivative of the position vector: 
$\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{d}{dt} (t^2 \hat{i} + t^3 \hat{j}) = 2t \hat{i} + 3t^2 \hat{j}$

This tells us how the position changes with time, both in magnitude and direction.
## 1D Motion: [[Newton's Second Law#Velocity|Velocity]]
#### Assuming Non-Constant Velocity
![[Pasted image 20240529123521.png]]
### Average Velocity (i.e. Average Rate of Change)
![[Pasted image 20240529123542.png]]
Describes the constant Velocity between $t_{1}$ and $t_{2}$ ***if*** the motion was linear. 
#### $\LARGE \bar{v}={Δx \over \triangle t}​ = {x(t_{2}) - x(t_{1}) \over t_{2} - t_{1}}$  
*Bar denotes average or mean.*

Notice that the **Average** Velocity is slope of the [[Secant Line|Secant line]].
	The Secant Line being a linear function that connects two points of a function. 
		The Secant Line in this case, is the [[Uniform Motion#Linear Time Dependence|linear time dependence function]], with Average Velocity as its slope. 
			![[Pasted image 20240529125003.png]]

When we consider two points on the position-time graph, say (t1​,s(t1​)) and (t2​,s(t2​)), the secant line connecting these two points represents the average rate of change of position with respect to time between t1​ and t2​. 
	The slope of this secant line is the average velocity $\bar{v}$​ over the interval [𝑡1,𝑡2][t1​,t2​]:
		$\bar{v}​=t2​−t1​s(t2​)−s(t1​)​$

This slope (average velocity) is calculated by taking the difference in position and dividing it by the difference in time between the two points.

#### Example Problem
![[Pasted image 20240602171421.png]]
![[Pasted image 20240602171453.png]]
### [[Derivatives|Velocity at Time]] $t$ (i.e. Instantaneous Rate of Change)
![[Pasted image 20240529130139.png|300]]
#### $\LARGE v= \lim\limits_{\triangle t \rightarrow 0} {Δx \over \triangle t}​ = {dx \over dt} = x'(t) = \dot{x}$
*Note: The "dot" above $x$ denotes a derivative with respect to time.*
	"$v = \dot{x}$"

As the [[Kinematics Analysis#Displacement (Δx,Δy,Δz)|displacement]] (i.e. interval between x values) of $\triangle x$ approaches 0, this represents the [[Limits|limit]]  of the secant line which is becomes a tangent line associated with "one" point or value of x (when the interval is 0).
	And the slope of this [[Tangent Line|tangent line]] is the [[Derivatives|derivative]] of the point (i.e. x value in this case). 
		And this [[Derivatives|derivative]] is the velocity at that point. 
![[Pasted image 20240529215642.png|300]]
This graph is the velocity ($\LARGE v(t)$) - i.e. the derivative (i.e. $\LARGE x'(t)$ or $\LARGE \dot{x}(t)$)for each point of the graph of the function $\LARGE x(t)$.
	Where each point of this function is the derivative of a t value of function x(t).
#### Example Problem Setup

We have a position function x(t) and we want to find its derivative x′(t), which represents the velocity v(t).
##### Definition of the Derivative
The derivative x′(t) of x(t) is given by the limit:
![[Pasted image 20240602162841.png]]
#### ![[Pasted image 20240602163652.png]]
Therefore, if:
	$\LARGE v(t) = {dx \over dt}$
		Then, one can actually find the displacement of $x$ via:
			$\LARGE dx = v(t) dt$
#### [[Derivatives#Example Finding the Derivative|Example of Solving a Derivative Function]]

### Velocity Vector
The velocity vector represents the rate of change of the position vector with respect to time.
	It indicates how fast and in which direction an object's position is changing.

**Mathematical Definition**:
The velocity vector $\vec{v}(t)$ is the first derivative of the position vector $\vec{r}(t)$ with respect to time: 
$\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt}$

**Components**:
In one-dimensional motion: 
$\LARGE v(t) = \frac{dx(t)}{dt}$

In two-dimensional motion: 
$\LARGE\vec{v}(t) = \frac{d}{dt}(x(t) \hat{i} + y(t) \hat{j}) = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j}$

In three-dimensional motion: $\LARGE\vec{v}(t) = \frac{d}{dt}(x(t) \hat{i} + y(t) \hat{j} + z(t) \hat{k}) = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} + \frac{dz(t)}{dt} \hat{k}$
###### Example of Acceleration Vector
Let's consider an example in two-dimensional motion:
- **Position Vector**: Suppose the position vector of a particle is given by: $\vec{r}(t) = t^2 \hat{i} + t^3 \hat{j}$
- **Velocity Vector**: The velocity vector is the first derivative of the position vector: $\vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{d}{dt}(t^2 \hat{i} + t^3 \hat{j}) = 2t \hat{i} + 3t^2 \hat{j}$
## 1D Motion: [[Newton's Second Law#Acceleration|Acceleration]]
![[Pasted image 20240531150448.png]]
### Average Acceleration Between $t_{1}$ and $t_{2}$
![[Pasted image 20240531150433.png|500]]
#### $\LARGE \bar{a} = {v(t_{2}) - v(t_{1}) \over t_{2} - t_{1}} = {\triangle v \over \triangle t}$
### Acceleration at Time $t$
![[Pasted image 20240531140529.png|500]]
#### $\LARGE a(t)= \lim\limits_{\triangle t \rightarrow 0} {Δv \over \triangle t}​ = {dv \over dt} = \dot{v} = {d^{2}x \over dt^{2}} = x''(t) = \ddot{x}$

I.e. The **derivative**, $a(t)$, *is* the **slope of the tangent line** *which is* the **limit**, $\lim\limits_{\triangle v \rightarrow 0}$  of the **linear function that connects two points** (i.e. the secant line), $\triangle v$, as **the displacement between the points, $\triangle t$, decreases to 0**. 
### Acceleration Vector

![[Pasted image 20240606124505.png|500]]
The acceleration vector represents the rate of change of the velocity vector with respect to time. 
	It indicates how fast and in which direction an object's velocity is changing.
Acceleration is **orthogonal** to the tangential velocity vector. 

**Mathematical Definition**:
The acceleration vector $\vec{a}(t)$ is the first derivative of the velocity vector $\vec{v}(t)$ with respect to time, or equivalently, the second derivative of the position vector $\vec{r}(t)$ with respect to time: 
$\LARGE\vec{a}(t) = \frac{d\vec{v}(t)}{dt} = \frac{d^2\vec{r}(t)}{dt^2}$

**Components**:
In one-dimensional motion: 
$\LARGE a(t) = \frac{dv(t)}{dt} = \frac{d^2x(t)}{dt^2}$

In two-dimensional motion: 
$\LARGE \vec{a}(t) = \frac{d}{dt}(\frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j}) = \frac{d^2x(t)}{dt^2} \hat{i} + \frac{d^2y(t)}{dt^2} \hat{j}$

In three-dimensional motion: 
$\LARGE \vec{a}(t) = \frac{d}{dt}(\frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} + \frac{dz(t)}{dt} \hat{k}) = \frac{d^2x(t)}{dt^2} \hat{i} + \frac{d^2y(t)}{dt^2} \hat{j} + \frac{d^2z(t)}{dt^2} \hat{k}$

###### Example of Acceleration Vector
Let's consider an example in two-dimensional motion:
- **Position Vector**: Suppose the position vector of a particle is given by: $\vec{r}(t) = t^2 \hat{i} + t^3 \hat{j}$
- **Velocity Vector**: The velocity vector is the first derivative of the position vector: $\vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{d}{dt}(t^2 \hat{i} + t^3 \hat{j}) = 2t \hat{i} + 3t^2 \hat{j}$
- **Acceleration Vector**: The acceleration vector is the first derivative of the velocity vector: $\vec{a}(t) = \frac{d\vec{v}(t)}{dt} = \frac{d}{dt}(2t \hat{i} + 3t^2 \hat{j}) = 2 \hat{i} + 6t \hat{j}$
## Example of Velocity Over Time
### Given
![[Pasted image 20240603125923.png]]
![[Pasted image 20240603125931.png]]
### Solve
![[Pasted image 20240603130014.png]]Where "path" refers to the **position** function (i.e. the function from which the velocity is derived).

##### Solving Position Function
To find this [[#Position|position]] function, we must **[[Integrals#What "Integrate" Means|integrate velocity's functional dependence with respect to time]]**.
	I.e. Integrate or summing the velocity function's output values produced by a range of input values.
###### Step 1: Use the [[Integrals#Power Rule for Integration|Power Rule for Integration]] on the Polynomial Equation (i.e. the velocity equation)
Use the Power Rule for [[Integrals|Integration]] on each "time dependent **term**" 
	![[Pasted image 20240603130516.png]]
	![[Pasted image 20240603130539.png]]
###### Step 2: [[Integrals#Integral Constant|Integration Constant]] as the Last Term, $x_0$ 
This term gets differentiated when we go from $x(t)$ to $x'(t)$.
###### Step 3: Calculate the Acceleration
Calculate the [[Derivatives|derivative]], because acceleration is given as the time derivative of the velocity.
	In this case using the [[Derivatives#Power Rule|Power Rule of Differentiation]]
That is, we will use the Power Rule of Differentiation *on* that $v(t)$ *to obtain* the differential of velocity, $a(t)$.

Remember $v(t)$:
![[Pasted image 20240606155414.png]]
Using the Power Rule of Differentiation:
## $\LARGE \frac{d}{dx} x^n = n x^{n-1}$ 

##### $\LARGE At^{6} = 6At^{5}$
##### $\LARGE Bt^{5} = 5Bt^{4}$
##### $\LARGE Ct^{4} = 4Ct^{3}$
##### $\LARGE Dt^{3} = 3Dt^{2}$
##### $\LARGE Et^{2} = 2Et$
##### $\LARGE Ft = F$

Therefore, $a(t)$ is:
![[Pasted image 20240606125001.png]]

![[Pasted image 20240606124950.png]]