---
up:
  - "[[Newtonian Mechanics]]"
related: 
date created: 2024-05-28
---
# Kinematics Analysis
###### The Description of Motion
![[Pasted image 20240528132613.png]]
  
**Kinematics** is a branch of mechanics that deals with the **description** of motion and trajectory without considering the forces that cause it. 
	That is, without the considering of [[Statics Analysis#Forces|forces]].
		It focuses on the geometric aspects of motion, such as displacement, velocity, and acceleration of objects. 
			Kinematics is concerned with the position of points, bodies, and systems of bodies, and how these positions change over time.
				Displacement: The change in position of an object.
				Velocity: The rate of change of displacement with time.
				Acceleration: The rate of change of velocity with time.

It involves the study of the positions, velocities, and accelerations of objects and how these quantities change over time. 
##### Kinetic
The term **kinematics** does have a connection to the word **kinetic**. 
	Both words derive from the Greek word "kinesis," which means movement or motion. 

**Kinetic**: The term "kinetic" relates to motion and is often used in physics to describe anything pertaining to or resulting from motion. 
- **Kinetic Energy**: The energy an object possesses due to its motion. It is given by the formula: 
	    $$\LARGE KE = \frac{1}{2}mv^2$$
 where $m$ is the mass of the object and $v$ is its velocity.

Understanding kinematics is essential for analyzing and predicting the motion of objects in various contexts, from everyday activities to complex engineering systems. 
	It forms the foundation for further studies in [[Dynamics Analysis|dynamics]], where the forces causing the motion are also considered.
## Components of Kinematics
##### Position (x, y, z)
The location of an object in space relative to a reference point, often described using a coordinate system (e.g., Cartesian coordinates).
##### Displacement (Δx,Δy,Δz)
The change in position of an object. 
	It is a [[Statics Analysis#Vector|vector]] quantity, meaning it has both [[Statics Analysis#The Magnitude of $ vec{w}$|magnitude]] and [[Statics Analysis#Direction|direction]].
		Displacement is calculated as the difference between the final and initial positions of the object.
##### [[Newton's Second Law#Velocity|Velocity]] (v)
The rate at which an object changes its position. It is a vector quantity and can be described as:
	**[[Linear Motion#Average Velocity|Average Velocity]] (𝑣ˉvˉ)**: Total displacement divided by the total time taken.
	**Instantaneous Velocity (v(t))**: The velocity of an object at a specific moment in time, found by taking the derivative of the position with respect to time.

It is the derivative of position.
##### [[Newton's Second Law#Speed|Speed]]
The magnitude of velocity. Unlike velocity, speed is a scalar quantity and does not have direction.
##### [[Newton's Second Law#Acceleration|Acceleration]] (a)
The rate at which an object changes its velocity. It is a vector quantity and can be described as:
    **Average Acceleration (𝑎ˉaˉ)**: Change in velocity divided by the total time taken.
    **Instantaneous Acceleration (a(t))**: The acceleration of an object at a specific moment in time, found by taking the derivative of velocity with respect to time.

It is the derivative of velocity.
	And the second derivative of position.
##### Reference Frames
The perspective from which motion is observed and measured. Motion can appear different depending on the chosen reference frame (e.g., stationary vs. moving reference frames).
##### Relative Motion
The calculation of the motion of an object as observed from a particular reference frame, taking into account the motion of the reference frame itself.
##### Vectors
##### [[Static Equilibrium#Position Vectors (a fourth method to "find" Resultant Force Vectors)|Position Vectors]]
	$\large \vec{r_{AB}} = (x_{B}-x_{A})\textbf{i} + (y_{B}-y_{A})\textbf{j} + (z_{B}-z_{A})\textbf{k}$
## Motion
##### Equations of Motion
In kinematics, the motion of objects can often be described using specific equations, especially when dealing with constant acceleration. The most common kinematic equations for linear motion in one dimension (assuming constant acceleration) are:
	1. v=v0​+at
		- Where 𝑣v is the final velocity, 𝑣0v0​ is the initial velocity, 𝑎a is the acceleration, and 𝑡t is the time.
	2. 𝑥=𝑥0+𝑣0𝑡+12𝑎𝑡2x=x0​+v0​t+21​at2
		- Where 𝑥x is the final position, 𝑥0x0​ is the initial position, 𝑣0v0​ is the initial velocity, 𝑎a is the acceleration, and 𝑡t is the time.
	1. 𝑣2=𝑣02+2𝑎(𝑥−𝑥0)v2=v02​+2a(x−x0​)
		- Where 𝑣v is the final velocity, 𝑣0v0​ is the initial velocity, 𝑎a is the acceleration, 𝑥x is the final position, and 𝑥0x0​ is the initial position.
##### Types of [[Newton's Second Law#Transformations as Motion (i.e. Representing Motion)|Motion]] (i.e. [[Transformations|transformations]])
###### [[Uniform Motion|Uniform Motion]]
Uniform motion refers to motion with a constant speed in a straight line. 
	This means that the object covers equal distances in equal intervals of time, regardless of how small those intervals are.
		There are no changes in the speed or direction of the motion.
		
Key characteristics of uniform motion:
- **Constant Velocity**: The speed and direction of the object remain constant.
- **Zero Acceleration**: There is no change in velocity over time.
- **Straight Line Path**: The motion occurs in a straight line.

Mathematically, if an object is in uniform motion, its displacement (Δ𝑥Δx) over a time interval (Δt) can be described by: 
	$\LARGE Δx=v⋅Δt$ 
		Where $v$ is the constant velocity.
###### [[Linear Motion|Linear Motion]]
Linear motion refers to motion along a straight line, but it does not specify whether the speed is constant. 
	Linear motion can involve varying speed, constant speed, or even accelerated motion along a straight path.
	
Key characteristics of uniform motion:
- **Straight Line Path**: The motion occurs in a straight line.
- **Variable or Constant Velocity**: The speed of the object can change or remain constant.
- **Acceleration**: Linear motion can involve acceleration or deceleration (change in velocity over time).

[[Non-Linear Motion]]
###### Projectile Motion: Motion in two dimensions under the influence of gravity.
###### [[Circular Motion|Circular Motion]]
Motion along a circular path, characterized by angular displacement, angular velocity, and angular acceleration.

