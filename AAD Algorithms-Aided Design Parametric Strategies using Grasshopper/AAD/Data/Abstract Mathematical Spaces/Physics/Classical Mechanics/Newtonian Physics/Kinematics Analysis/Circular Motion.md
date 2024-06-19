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
$$s\LARGE = \phi \cdot r$$
### Angular Position $\LARGE \phi$
**Angular position** refers to the orientation of a line with another line or plane. 

It is the angle between the reference line (often the x-axis) and the line from the center of the circle to the point in question. 
	Angular position is usually denoted by ϕ\phiϕ and is measured in radians or degrees.
Used in [[#Angular Displacement ($ phi$)|Angular Displacement]]
Radius independent
### Polar Coordinates
A single coordinate that describes all motion.

### Angular Displacement ($\theta$ or $\Delta \phi$)
**Angular displacement** is the measure of the angle through which an object has rotated or moved from a reference position over a given period of time. 
	It is the change in the angular position. Angular displacement is also measured in radians or degrees and can be positive (counterclockwise rotation) or negative (clockwise rotation).
		It is the angle between the initial and final positions of the object.
$$\LARGE \Delta \phi = \phi_f - \phi_0$$

$$\LARGE \theta = \frac{s}{r}$$
where $s$ is the arc length and $r$ is the radius of the circle.
### [[Newton's Second Law#Angular Velocity|Angular Velocity]] ($\omega$)
![[Pasted image 20240617181332.png]]
Radius Independent.
	No matter how large or small the radius is, the angular velocity will be the same.
	
Angular velocity is the rate of change of angular displacement with respect to time.
	It is a vector quantity, which means it has both magnitude and direction.

Angular Velocity is a vector quantity, directed along the axis of rotation (using the right-hand rule).
	It measures the rate of change of the angle.
		Its units are radians per second $(rad/s)$.
$$\LARGE \vec{\omega} = \omega \hat{n}$$
			$\omega$ is the magnitude of the angular velocity (angular speed).
			$\hat{n}$ is a unit vector in the direction of the axis of rotation.

Angular velocity ($\omega$) is a vector that is normal (perpendicular) to the plane of the circular motion. 
	This is a fundamental aspect of how angular velocity is represented in three-dimensional space.

It is the derivative of the angular position with respect to time. 
    $$\LARGE \omega(t) = \lim_{\triangle t \rightarrow 0}{\triangle \phi \over \triangle t} = \frac{d\phi}{dt} = \phi'(t) = \dot{\phi}$$
### Linear Velocity ($v$)
$$\LARGE v=\omega \cdot r$$
![[Pasted image 20240617181227.png]]
Anything that moves or turns in the circular direction has both linear velocity and angular velocity.

Linear velocity ($v$) refers to the rate at which an object moves along a path.
	For an object in circular motion, the linear velocity is always [[Tangent Line|tangent]] to the circle. 
		The angular velocity is the ratio of the angle traversed to the amount of time it takes to traverse that angle.

Linear Velocity is radius dependent.

It measures the rate of change of the position along the circular path.
	Its units are meters per second (m/s).
		It is a vector quantity, tangential to the circular path at any point.
### [[Newton's Second Law#Angular Acceleration|Angular Acceleration]] ($\alpha$)
Angular acceleration is the rate of change of angular velocity with respect to time.
$$\LARGE \alpha(t) = \frac{d\omega}{dt} = \frac{d^2\phi}{dt^2} = \dot{\omega} = \ddot{\phi}$$
### Linear [[Components of Motion#Acceleration Vector|Acceleration]]
Radius dependent.
$$\LARGE a = \alpha \cdot r$$
### [[Components of Motion#Centripetal Force|Centripetal Force]] ($F_c$)
Centripetal force is the force that keeps an object moving in a circular path, directed towards the center of the circle.
    $$\LARGE F_c = \frac{mv^2}{r} = mr\omega^2$$
    where $m$ is the mass of the object, $v$ is the linear velocity, and $r$ is the radius.
    
### Tangential Velocity ($v$)
The linear velocity of an object moving in a circular path is tangent to the circle at any point.
    $$\LARGE v = r\omega$$
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