# Circular Motion Examples
These examples are considered difficult due to the inherent nature of [[Kinematics Analysis|Kinematics]].
	Which does not consider the origin of the motion (i.e Newtonian forces) or constraints (Lagrange).
## 1. Pendulum Swing
![[Pasted image 20240621070256.png|400]]
The acceleration always experienced by a pendulum is always gravity, $g$.
	Therefore, at every point along the circle, we must calculate the negative $y$ direction projection **onto** the tangential line.
		This projection is the [[Circular Motion#Angular Acceleration Vector Direction|Angular Acceleration]], $\LARGE \alpha$.
			Where $\LARGE \alpha = g_{effective}$
#### The Length of the Tangential Line:
The Tangential Line, itself stems from the radius.
	And the radius itself is perpendicular to the tangential line. 
		We need to identify the **length** of the **Tangential line**.

Notice that the angle $\varphi$ between radius $r$ and the $x$ axis, also exists between the $g$ vector and the Tangential Line.
	This is because the radius and the projection between the Tangential Line and $g$ vector, are parallel. 
		Therefore, the length of the vector is equal to the length of the adjacent side of the right triangle formed by $r$, $g$ and the $x$ axis.
			Which is the $\cos$ of angle $\varphi$ of the $r$ and $g$:
				$$\LARGE \cos \varphi = {\text{adjacent} \over r}$$
				Therefore:
				$$\LARGE r \cdot \cos \varphi = \text{adjacent}$$
##### [[Circular Motion#Angular Acceleration Vector Direction|Angular Acceleration]] ($\alpha$) as a Scalar Quantity of a Pendulum
- **Definition**: Angular acceleration ($\alpha$) is the rate of change of angular velocity ($\omega$) with respect to time.
	- It can be expressed as either the derivative of the [[Circular Motion#Newton's Second Law Angular Velocity Angular Velocity ($ omega$)|Angular Velocity]] or as the Second Derivative of the Angular Position.
- **Formula**: 
$$\LARGE \alpha = \ddot{\varphi} = -\frac{g}{r} \cos \varphi$$
- where:
    - $g$ is the acceleration due to gravity
    - $r$ is the radius (length of the pendulum)
    - $\varphi$ is the angle between the pendulum and the vertical axis
##### [[Circular Motion#Tangential Acceleration ($a_t$)|Tangential Acceleration]] ($a_t$)
- **Definition**: Tangential acceleration is a component of the linear acceleration along the tangent to the circular path. It represents the rate of change of the tangential (or linear) velocity.
- **Relation to Angular Acceleration**: 
$$\LARGE \alpha_{t} = r \cdot \alpha$$
$$\LARGE  \cos \varphi = {\alpha_{t} \over g}$$
Where $\alpha_{t}$ is the adjacent side.
$$\LARGE \alpha_t​ = g \cdot \cos \varphi$$
Now plug in $r \cdot \alpha$ for $\alpha_{t}$ 
$$\LARGE r\cdot \alpha = g \cdot \cos \varphi$$
$$\LARGE = \alpha = {g \cdot \cos \varphi \over r}$$
##### Explanation: In the context of the pendulum
1. **Gravitational Force**: The only force acting on the pendulum is gravity ($g$), which acts vertically downward.
2. **Component of Gravity along the Tangent**: The tangential component of the gravitational force is $g \cos \varphi$. This component causes the tangential acceleration.
3. **Angular Acceleration**: The angular acceleration ($\alpha$) is related to the tangential acceleration by the radius of the pendulum:
$$\LARGE \alpha = \ddot{\varphi} = -\frac{g}{r} \cos \varphi$$
### Limit of Kinematics
$$\LARGE \alpha = \ddot{\varphi} = -\frac{g}{r} \cos \varphi$$
This equation is not able to be integrated. 
	We have $\varphi$ but don't know its value.
		This is a Differential Equation.
## 2. Harmonic Oscillator
$$\LARGE \alpha = \ddot{\varphi} = -\frac{g}{r} \cos \varphi$$
![[Pasted image 20240621143549.png|400]]
Same as the Pendulum Swing.
	Except we do an Angle Transformation.
		$\LARGE \varphi = \phi - {\pi \over 2}$
			Where before $\varphi$ was measured from the $x$ axis. 
				In this new example, the angle $\phi$ is taken relative to the $y$ axis. 

What this Angular Transformation enables, is the $\cos$ can be changed.
$$\LARGE \alpha = \ddot{\varphi} = -\frac{g}{r} \cos \varphi \rightarrow \ddot \phi = -{g \over r} \sin \phi$$

We can now solve, albeit without differential equations or integration.
	It is an estimate.

Because the derivative of $\sin$ is $\cos$.
	And derivative of $\cos$ is $-\sin$.
## Example Problem
Consider a starting velocity of $\LARGE v_{0} = 10 \frac{m}{s}$ in a roundabout with a radius $r= 5m$.
	Upon breaking, the angular acceleration is constant $\LARGE \alpha = -0.1 \frac {1}{s^2}$
		*Note: Angular Acceleration is decreasing.*

1. How long does it take until the roundabout stops?
	I.e. At what time, $t$, is the Angular Velocity $0$?
2. How many rotations did the roundabout complete during that time?
	I.e. What is the Angular Displacement at that time, $t$?
#### Unknowns
##### 1. To Find $t$ where Angular Velocity, $\omega = 0$ 
###### Find Angular Velocity:
We know that Tangential Velocity, $\alpha_t$ is:
$$\LARGE \alpha_t = \omega \cdot r$$
Therefore:
$$\LARGE \omega = {\alpha_t \over r}$$
###### The Initial Angular Velocity, $\omega_0$
$$\LARGE = \omega_0 = {v_0 \over r} = {10{m\over s}\over 5m} = 2{1 \over s}$$
$$\LARGE 2{1 \space radian \over s} = 2 \space \text{radians}$$
###### The Angular Velocity, $\omega$
Via integrating over the Angular Acceleration, $\alpha = -0.1{1\over s^2}$ which we know is a [[Integrals#Constant Rule|constant]] which means the integral is a linear function. 

$$\LARGE \omega = \int \alpha dt = \alpha t + \omega_0$$
###### Graph Method:
Below is the graph of the Angular Velocity obtained via Integration:
	We can see that at time, $t=2s$, the Angular Velocity is $0$.
![[Pasted image 20240622075043.png]]
###### Calculation Method
We can also set $\omega=0$ and find the [[Derivatives#Critical Points|critical point]], $\LARGE {t_{c}}$
$$\LARGE 0 = \alpha {t_c} + w_0$$
$$\LARGE - w_0= \alpha {t_c}$$
$$\LARGE -{w_0\over \alpha }= {t_c}$$
Plug in values
$$\LARGE -{2{1\over s} \over 0.1{1\over s^2} }= {t_c}$$
$$\LARGE = t_c = 20s$$
##### 2. Find the Angular Displacement at critical point, $t_c$
###### Find the Angular Position at time, $t_c$
Via Integrating Angular Velocity at $\LARGE t_c=20s$.
$$\LARGE \varphi =  \int\omega dt = \int (\alpha t + \omega_0) dt$$
We know that [[Integrals#Integration of a Linear Function|Integrating a Linear Function yields a Quadratic Function]].
$$\LARGE \varphi =  \int\omega dt = \int (\alpha t + \omega_0) dt = {1\over 2}\alpha t^2 + \omega_0 t + \varphi_0$$
Remember that Angular Displacement is:
$$\LARGE \Delta \varphi = \varphi_f - \varphi_0$$
Now set the time, $t$ in this function $=t_c$:
$$\LARGE \varphi(t_c) =  \int \omega dt = {1\over 2}\alpha t_{c}^2 + \omega_{0_c} t_c + \varphi_0$$
$$\LARGE \varphi(0) = \varphi_0$$
$$\LARGE \varphi(t_c) - \varphi(0) = ({1\over 2}\alpha t_{c}^2 + \omega_{0_c} t_c + \varphi_0) - (\varphi_0)$$
$$\LARGE \varphi - \varphi_0 =  \int \omega dt = ({1\over 2} -(0.1{1\over s}) (20s^2) + 2{1\over s} (20s) + \varphi_0) - \varphi_0$$
$$\LARGE = \Delta \varphi = 20 \space radians$$ ![[Pasted image 20240622215437.png]]

To Get Number of Rotations:
$$\LARGE {\varphi - \varphi_0 \over 2\pi} = {20\over 2\pi} = {10\over \pi} 3.18 \space Rotations$$