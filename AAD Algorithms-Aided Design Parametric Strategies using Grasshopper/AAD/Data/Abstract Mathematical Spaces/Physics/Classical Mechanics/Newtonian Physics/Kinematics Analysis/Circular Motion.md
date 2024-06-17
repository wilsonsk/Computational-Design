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
#### Key Concepts
##### Angular Displacement ($\theta$)
Angular displacement refers to the angle in radians through which a point or line has been rotated in a specified sense about a specified axis. It is the angle between the initial and final positions of the object.
$$\LARGE \theta = \frac{s}{r}$$
    where $s$ is the arc length and $r$ is the radius of the circle.
##### [[Newton's Second Law#Angular Velocity|Angular Velocity]] ($\omega$)
Angular velocity is the rate of change of angular displacement with respect to time.
	It is a vector quantity, which means it has both magnitude and direction.
    $$\LARGE \omega = \frac{d\theta}{dt}$$
##### [[Newton's Second Law#Angular Acceleration|Angular Acceleration]] ($\alpha$)
Angular acceleration is the rate of change of angular velocity with respect to time.
    $$\LARGE \alpha = \frac{d\omega}{dt}$$
##### [[Components of Motion#Centripetal Force|Centripetal Force]] ($F_c$)
Centripetal force is the force that keeps an object moving in a circular path, directed towards the center of the circle.
    $$\LARGE F_c = \frac{mv^2}{r} = mr\omega^2$$
    where $m$ is the mass of the object, $v$ is the linear velocity, and $r$ is the radius.
    
##### Tangential Velocity ($v$)**
The linear velocity of an object moving in a circular path is tangent to the circle at any point.
    $$\LARGE v = r\omega$$
##### Period ($T$) and Frequency ($f$)
The period is the time taken for one complete revolution. Frequency is the number of revolutions per unit time.
    $$\LARGE T = \frac{2\pi}{\omega}, \quad f = \frac{1}{T}$$
#### Derivation and Relationships
###### From Angular to Linear Quantities
The linear quantities (such as velocity and acceleration) in circular motion are derived from their angular counterparts.
- **Linear Displacement ($s$)**:
    $$\LARGE s = r\theta$$
- **Linear Velocity ($v$)**:
    $$\LARGE v = r\omega$$
- **Linear Acceleration**: The total linear acceleration $a$ has two components: radial (centripetal) acceleration $\LARGE a_r$​ and tangential acceleration $\LARGE a_t$​.
    $$\LARGE a_r = r\omega^2, \quad a_t = r\alpha$$