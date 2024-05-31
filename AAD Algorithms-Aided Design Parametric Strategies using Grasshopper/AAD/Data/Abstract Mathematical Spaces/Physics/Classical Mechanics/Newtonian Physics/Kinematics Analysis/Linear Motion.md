# Linear Motion
Linear motion refers to motion along a straight line, but it does not specify whether the speed is constant. 
	Linear motion can involve varying speed, constant speed, or even accelerated motion along a straight path.
## 1D Motion: [[Newton's Second Law#Velocity|Velocity]]
#### Assuming Non-Constant Velocity
![[Pasted image 20240529123521.png]]
### Average Velocity
![[Pasted image 20240529123542.png]]
Describes the constant Velocity between $t_{1}$ and $t_{2}$ ***if*** the motion was linear. 
#### $\LARGE \bar{v}={Δx \over \triangle t}​ = {x(t_{2}) - x(t_{1}) \over t_{2} - t_{1}}$  
*Bar denotes average or mean.*

Notice that the **Average** Velocity is slope of the [[Secant Line|Secant line]].
	The Secant Line being a linear function that connects two points of a function. 
		The Secant Line in this case, is the [[Uniform Motion#Linear Time Dependence|linear time dependence function]], with Average Velocity as its slope. 
			![[Pasted image 20240529125003.png]]

When we consider two points on the position-time graph, say (t1​,s(t1​)) and (t2​,s(t2​)), the secant line connecting these two points represents the average rate of change of position with respect to time between 𝑡1t1​ and 𝑡2t2​. 
	The slope of this secant line is the average velocity $\bar{v}$​ over the interval [𝑡1,𝑡2][t1​,t2​]:
		$\bar{v}​=t2​−t1​s(t2​)−s(t1​)​$

This slope (average velocity) is calculated by taking the difference in position and dividing it by the difference in time between the two points.
### [[Derivatives|Velocity at Time]] $t$
![[Pasted image 20240529130139.png|300]]
#### $\LARGE v= \lim\limits_{\triangle t \rightarrow 0} {Δx \over \triangle t}​ = {dx \over dt} = x'(t) = \dot{x}$
*Note: The "dot" above $x$ denotes a derivative with respect to time.*
	"$v = \dot{x}$"

As the [[Kinematics Analysis#Displacement (Δx,Δy,Δz)|displacement]] (i.e. interval between x values) of $\triangle x$ approaches 0, this represents the [[Limits|limit]]  of the secant line which is becomes a tangent line associated with "one" point or value of x (when the interval is 0).
	And the slope of this [[Tangent Line|tangent line]] is the [[Derivatives|derivative]] of the point (i.e. x value in this case). 
		And this derivative is the velocity at that point. 
![[Pasted image 20240529215642.png|300]]
This graph is the velocity ($\LARGE v(t)$) - i.e. the derivative (i.e. $\LARGE x'(t)$ or $\LARGE \dot{x}(t)$)for each point of the graph of the function $\LARGE x(t)$.
	Where each point of this function is the derivative of a t value of function x(t).
## 1D Motion: [[Newton's Second Law#Acceleration|Acceleration]]
![[Pasted image 20240531150448.png]]
### Average Acceleration Between $t_{1}$ and $t_{2}$
![[Pasted image 20240531150433.png|500]]
#### $\LARGE \bar{a} = {v(t_{2}) - v(t_{1}) \over t_{2} - t_{1}} = {\triangle v \over \triangle t}$
### Acceleration at Time $t$
![[Pasted image 20240531140529.png|500]]
#### $\LARGE a(t)= \lim\limits_{\triangle t \rightarrow 0} {Δv \over \triangle t}​ = {dv \over dt} = \dot{v} = {d^{2}x \over dt^{2}} = x''(t) = \ddot{x}$
