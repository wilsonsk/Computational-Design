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

