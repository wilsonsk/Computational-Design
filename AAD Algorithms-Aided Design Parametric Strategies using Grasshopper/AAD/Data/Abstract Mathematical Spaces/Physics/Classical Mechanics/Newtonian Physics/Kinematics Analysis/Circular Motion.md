---
up:
  - "[[Kinematics Analysis]]"
related: 
date created: 2024-06-16
---
# Circular Motion
Circular motion is a type of motion where an object moves along the circumference of a circle. 

This motion can be characterized by several parameters, such as angular velocity, angular acceleration, radius, and centripetal force. 
	The study of circular motion is essential in understanding the dynamics of systems ranging from simple mechanical systems to complex astronomical objects.
## Motion is Effectively 1 Dimensional
![[Pasted image 20240617175350.png|300]]
Due to the circular trajectory, there then exists a radius that the motion is along.
	The radius is constant.
		Therefore, motion can be described in 1 dimension, using a single, polar coordinate.
			If using Cartesian Coordinates, it would still be 2D as we'd still be using $x$ and $y$ axes to describe the position, and motion.
###### Arc s
Radius dependent.
$$s\LARGE = \varphi \cdot r$$
### Angular Position $\LARGE \varphi$
**Angular position** refers to the orientation of a line with another line or plane. 

It is the angle between the reference line (often the x-axis) and the line from the center of the circle to the point in question. 
	Angular position is usually denoted by ϕ\varphiϕ and is measured in radians or degrees.
Used in [[#Angular Displacement ($ phi$)|Angular Displacement]]
Radius independent
### Polar Coordinates
A single coordinate that describes all motion.

### Angular Displacement ($\theta$ or $\Delta \varphi$)
**Angular displacement** is the measure of the **angle** through which an object has rotated or moved from a reference position over a given period of time. 
	It is the change in the angular position. Angular displacement is also measured in radians or degrees and can be positive (counterclockwise rotation) or negative (clockwise rotation).
		It is the angle between the initial and final positions of the object.
$$\LARGE \Delta \varphi = \varphi_f - \varphi_0$$

$$\LARGE \theta = \frac{s}{r}$$
Where $s$ is the arc length and $r$ is the radius of the circle.
### Linear Velocity ($v_{t}$)
Linear velocity ($v$) refers to the rate at which an **object moves along a path**.

![[Pasted image 20240617181227.png]]
In the context of circular motion, tangential velocity and linear velocity are synonymous and both describe the speed at which an object moves along the circular path.
#### Components of Linear Velocity
Linear velocity in circular motion can be decomposed into two orthogonal components:
##### Tangential Velocity ($v_t$)
Linear Velocity is radius dependent.
The magnitude of the tangential velocity is given by: 
$$\LARGE v_{t}=\omega \cdot r$$
- $r$ is the radius of the circular path
- $\omega$ is the angular velocity (rate of change of the angle with respect to time)

This is the component of the linear velocity that is tangent to the circular path.
	It represents the rate at which the object moves along the circumference of the circle.

The direction of the tangential velocity is always perpendicular to the radius at any point on the path.
##### Radial (Centripetal) Velocity
For uniform circular motion (where the speed is constant), there is no component of linear velocity in the radial direction because the object is not moving towards or away from the center. 
	The radial component of the velocity is zero.
	
For non-uniform circular motion (where the speed changes), there can be a radial component of velocity if the radius of the circular path changes. 

However, in typical circular motion with a fixed radius, the radial velocity component is zero.
#### Linear Velocity Components in Uniform Circular Motion
In uniform circular motion:
- The speed is constant.
- The tangential velocity is the only component of linear velocity.
- There is no radial component of linear velocity.
#### Linear Velocity Components in Non-Uniform Circular Motion
In non-uniform circular motion:
- The speed can change, leading to a changing tangential velocity.
- If the radius of the circular path changes, there can be a radial component of linear velocity.

For an object in circular motion, the linear velocity is always [[Tangent Line|tangent]] to the circle. 
	The angular velocity is the ratio of the angle traversed to the amount of time it takes to traverse that angle.

It measures the rate of change of the position along the circular path.
	Its units are meters per second (m/s).
		It is a vector quantity, tangential to the circular path at any point.

Anything that moves or turns in the circular direction has both linear velocity and angular velocity.

### [[Newton's Second Law#Angular Velocity|Angular Velocity]] ($\omega$)
The rate of the change of the **Angular** Position (i.e. the angle) as an object moves along a circular path.
![[Pasted image 20240617181332.png]]
Radius Independent.
	No matter how large or small the radius is, the angular velocity will be the same.
	
Angular velocity is the rate of change of angular displacement with respect to time.
	It is a vector quantity, which means it has both magnitude and direction.
		Its direction is normal to the plane of the circular motion.

Angular Velocity is a vector quantity, directed along the axis of rotation (using the right-hand rule).
	It measures the rate of change of the angle.
		Its units are radians per second $(rad/s)$.
$$\LARGE \vec{\omega} = \omega \hat{n}$$
			$\omega$ is the magnitude of the angular velocity (angular speed).
			$\hat{n}$ is a unit vector in the direction of the axis of rotation.

Angular velocity ($\omega$) is a vector that is normal (perpendicular) to the plane of the circular motion. 
	This is a fundamental aspect of how angular velocity is represented in three-dimensional space.

It is the derivative of the angular position with respect to time. 
    $$\LARGE \omega(t) = \lim_{\triangle t \rightarrow 0}{\triangle \varphi \over \triangle t} = \frac{d\varphi}{dt} = \varphi'(t) = \dot{\varphi}$$
### Linear [[Components of Motion#Acceleration Vector|Acceleration]]
The rate of change of the velocity of an object as it moves along a path.
Radius dependent.
$$\LARGE a = \alpha \cdot r$$
![[Pasted image 20240619112640.png]]
*Note: The Normal Acceleration (i.e. Centripetal Acceleration) and the Tangential Acceleration are paired together at $90\degree$* at a given point.
	They are components of Linear Acceleration.
#### Components of Linear Acceleration
###### Formula for Total Linear Acceleration ($a$)**
$$\LARGE \vec{a} = \vec{a_t} + \vec{a_c}$$
Linear acceleration in circular motion can be broken down into two components:
##### Tangential Acceleration ($a_t$)
![[Pasted image 20240621130543.png|200]]
Tangential acceleration is the rate of change of tangential velocity.
	It represents how the speed of the object along the circular path is changing with time.
		 The formula for tangential acceleration is: 
		  $$\LARGE \alpha_{t}​=rα$$ where:
- $r$ is the radius of the circular path
- $\alpha$ is the angular acceleration (rate of change of angular velocity with respect to time)
###### Tangential Acceleration is always directed tangent to the circle.
Tangential acceleration is the rate at which a tangential velocity varies in the rotational motion of any object.
	It acts in the direction of a tangent at the point of motion for an object. 

The tangential velocity also acts in the same direction for an object undergoing circular motion.
	Tangential acceleration only exists when an object travels in a circular path.
		 It is positive if the body is rotating at a faster velocity, negative when the body is decelerating, and zero when the body is moving uniformly in the orbit.

Tangential acceleration is similar to linear acceleration, however, it is only in one direction. 
	This has something to do with circular motion. 
		Tangential acceleration is therefore the rate of change of a particle’s [tangential velocity](https://www.geeksforgeeks.org/tangential-velocity-formula/) in a circular orbit. It always points to the tangent of the body’s route.

Tangential acceleration works when an object moves in a circular path. 
	Tangential acceleration is similar to linear acceleration, but it is not the same as straight-line linear acceleration.
		 If an item moves in a straight line, it is linearly accelerating.
##### [[#Components of Motion Centripetal Force Centripetal Force ($F_c$)|Centripetal]] (aka Radial aka Normal) Acceleration ($a_c$)
![[Pasted image 20240621130609.png|200]]
The component directed towards the center of the circle, representing changes in the direction of the velocity vector.
$$\LARGE a_c = \frac{v_t^2}{r}$$​Where $a_c$ is the centripetal acceleration, $v_t$ is the tangential velocity, and $r$ is the radius of the circular path.

**Definition**
Centripetal acceleration is the acceleration that acts towards the center of the circular path, causing the change in direction of the tangential velocity, thus keeping the object in circular motion.

**Direction**
Always points radially inward towards the center of the circular path.
### [[Newton's Second Law#Angular Acceleration|Angular Acceleration]] ($\alpha$)
![[Pasted image 20240621130534.png|200]]
Angular acceleration is the rate of change of Angular Velocity (i.e. the velocity of the change in the angle) with respect to time.

Angular acceleration ($\alpha$) is indeed defined as the rate of change of angular velocity with respect to 
time:
$$\LARGE \alpha(t) = \frac{d\omega}{dt} = \frac{d^2\varphi}{dt^2} = \dot{\omega} = \ddot{\varphi}$$

It can also be expressed as the second derivative of the angular position ($\varphi$) with respect to time:
$$\LARGE \alpha = \ddot{\varphi} = -\frac{g}{r} \cos \varphi$$
I.e. This is a Differential Equation.
 
Where:
    - $\omega$ is the angular velocity
    - $\varphi$ is the angular position
    - $\ddot{\varphi}$ is the second derivative of $\varphi$ with respect to time (angular acceleration)
##### Relationship to the [[#Tangential Acceleration ($a_t$)|Tangential Acceleration]] ($a_t$)
Tangential acceleration is the linear acceleration tangent to the circular path. 
	It represents the rate of change of the tangential (or linear) velocity.
###### Relationship to Angular Acceleration: 
Where:
    - $a_t$ is the tangential acceleration
    - $r$ is the radius of the circular path
    - $\alpha$ is the angular acceleration
##### Angular Acceleration Vector Direction
It is normal to the plane of the circular motion.

**Right-Hand Rule**: To determine the direction of the angular acceleration vector ($\alpha$), you use the right-hand rule:
    Point your right-hand fingers in the direction of the rotation (along the axis of rotation).
    Curl your fingers in the direction of the angular velocity vector ($\omega$).
    Your thumb will point in the direction of the angular velocity vector.
    
If the angular velocity is increasing, the angular acceleration vector points in the same direction as the angular velocity vector.
	If the angular velocity is decreasing, the angular acceleration vector points in the opposite direction to the angular velocity vector.
### [[Components of Motion#Centripetal Force|Centripetal Force]] ($F_c$)
Centripetal force is the net force that acts towards the center of a circular path, causing centripetal acceleration.
	It is the force that keeps an object moving in a circular trajectory.
$$\LARGE F_c = \frac{mv^2}{r} = mr\omega^2$$
Where $m$ is the mass of the object, $v$ is the linear velocity, and $r$ is the radius.
#### Relationship Between Centripetal Acceleration and Centripetal Force
###### Direct Proportionality
Centripetal force is directly proportional to centripetal acceleration.
	This relationship is given by Newton's second law of motion ($F = m \cdot a$), applied to circular motion.
###### Combined Formula
By substituting the expression for centripetal acceleration into the formula for centripetal force, we get: 

**Using Linear (Tangential) Velocity ($v_t$):**
$$\LARGE F_c = m \cdot \frac{v_t^2}{r}$$​
Where $\LARGE v_t$ is the Tangential Velocity, and $\LARGE \frac{v_t^2}{r}$ is the Centripetal Acceleration

- **Explanation**: This formula expresses centripetal force ($F_c$) in terms of the mass ($m$) of the object, its tangential velocity ($v_t$), and the radius ($r$) of the circular path.
- **Usefulness**: It directly relates the centripetal force to the linear speed of the object moving along the circular path.

**Using Angular Velocity ($\omega$):**
$$\LARGE F_c = mr\omega^2$$
- **Explanation**: This form expresses centripetal force in terms of the mass ($m$) of the object, the radius ($r$) of the circular path, and the angular velocity ($\omega$).
- **Usefulness**: It shows how centripetal force depends on the rate of rotation (angular velocity) and the distance from the center of the circular path.

This shows that centripetal force depends on the mass of the object, the square of its tangential velocity, and the radius of the circular path.
### Period ($T$) and Frequency ($f$)
The period is the time taken for one complete revolution. Frequency is the number of revolutions per unit time.
    $$\LARGE T = \frac{2\pi}{\omega}, \quad f = \frac{1}{T}$$
### Derivation and Relationships
###### From Angular to Linear Quantities
The linear quantities (such as velocity and acceleration) in circular motion are derived from their angular counterparts.
- **Linear Displacement ($s$)**:
    $$\LARGE s = r\theta$$
- **Linear Velocity ($v$)**:
    $$\LARGE v = r\omega$$
- **Linear Acceleration**: The total linear acceleration $a$ has two components: radial (centripetal) acceleration $\LARGE a_r$​ and tangential acceleration $\LARGE a_t$​.
	
$$\LARGE a_r = r\omega^2, \quad a_t = r\alpha$$