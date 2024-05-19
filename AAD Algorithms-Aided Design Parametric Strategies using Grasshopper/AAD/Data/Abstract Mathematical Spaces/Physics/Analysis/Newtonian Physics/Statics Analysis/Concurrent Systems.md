---
up:
  - "[[Statics Analysis]]"
related:
  - "[[Non-Concurrent Systems]]"
  - "[[Dynamics Analysis]]"
  - "[[Static Equilibrium]]"
date created: 2024-05-04
---
# Concurrent Force Systems
A set of [[Statics Analysis#Structural Analysis Static Equilibrium Point Forces Point Forces as Vectors|point forces]] is considered concurrent if all the [[Statics Analysis#Line of Action|lines of action]] of those forces all come together at a single point.
	I.e. A concurrent force system is one where all forces acting on a body intersect at a common point, regardless of their directions.

Because the forces all act through a single point, **there are no [[Non-Concurrent Systems#Moments (i.e. Torque)|moments]] about this point**.
	Because no moments exist, we can treat this body as a **particle**. 
		In fact, because real particles only exist in theory, most particle analysis is actually applied to extended bodies with concurrent forces acting on them.

![[Pasted image 20240504001917.png]]
## General Static Equilibrium Analysis for Concurrent Force Systems
If a body is in static equilibrium, then by definition that body is not accelerating (i.e. velocity is not changing- and therefore doesn't need to be "not moving"). 
	If we know that the body is not accelerating then we know that **the sum of the forces acting on that body must be equal to zero**. 
		This is the basis of Concurrent Force equilibrium analysis (I.e. Translational Equilibrium) of a body. 
		
In order to solve for any unknowns in the sum of forces equation, turn the one vector equation into a set of scalar equations. 
	For two dimensional problems, split our one vector equation down into two scalar equations. 
		We do this by summing up all the $x$ components of the force vectors and setting them equal to zero in our first equation.
			Then summing up all the $y$ components of the force vectors and setting them equal to zero in our second equation.
	For three dimensional problems, add a third equation.
		The sum of all our $z$ components equal to zero.

 $\LARGE \sum{\vec{F_y}}​=0$
 $\LARGE \sum{F_x}​=0$ ; $\LARGE \sum{F_y}​=0$ ; $\LARGE \sum{F_z}​=0$
## [[Concurrent Systems|Translational Equilibrium]] in Concurrent Systems
Translational equilibrium is focused entirely on the linear aspects of motion, not addressing any rotational dynamics that might be present.
	$\begin{equation*} \LARGE \sum \vec{F} = m \times \vec{a} \end{equation*}$

**In a concurrent system**, translational equilibrium occurs when the vector sum of all forces acting on the [[Bodies|body]] equals zero ($∑F=0$).
	Applies to both [[Bodies#Particles|particles]] and [[Bodies#Rigid Bodies|rigid bodies]]. 
		All external forces must sum to zero, ensuring no net force acts on the object, thus preventing any translational motion or acceleration.
			I.e. There is no net acceleration and the body will either remain at rest or move with constant velocity.
				Therefore, $\large a=0$

Translational equilibrium specifically refers to the condition where the sum of all external forces acting on a body is zero, indicating no net force. 
	This implies that there is no net linear acceleration, meaning the body is either stationary or moving with a constant velocity (not changing speed or direction). 
### Calculating the Vector Sum of Forces
Each force is resolved into its component vectors along established axes (typically, x, y, and z axes in three-dimensional systems). 
	This involves decomposing each force into its horizontal and vertical components, using trigonometry based on the angle the force makes with the reference axes.
### The General Procedure for Finding the Equilibrium Equations
###### 1. Identify the Point of Concurrency 
Draw a [[Free Body Diagram|free body diagram]] of the body being analyzed to determine the common point through which all the forces act - this is the **point of concurrency**.
- The diagram should show all the known and unknown force vectors acting externally on the body.
- In the free body diagram, provide values for any of the know magnitudes or directions for the force vectors and provide variable names for any unknowns (either magnitudes or directions).
	![[Pasted image 20240504003640.png]]
###### 2. Chose the $x, y, z$ Axes
These axes must be perpendicular to one another, but do not need to necessarily have to be horizontal or vertical. 
###### 3. [[Static Equilibrium#Decomposing Forces|Decomposition]]
Break down all of the force vectors into [[Static Equilibrium#Vector Form Analysis (i.e. Cartesian Vectors)|component scaled unit vectors]] along the $x, y, x$ directions. 
	If forces are given in vector form or applied at angles to a coordinate system, resolve each force into its orthogonal components (typically along x, y, and possibly z axes in three-dimensional space).
- The first equation will be the sum of the magnitudes of the components in the $𝑥$ direction being equal to zero.
- The second equation will be the sum of the magnitudes of the components in the $y$ direction being equal to zero.
- And the third (if a 3D problem) will be the sum of the magnitudes in the $z$ $direction being equal to zero.
- Collectively these are known as the **equilibrium equations**.
###### 4. Sum up the Force Components
Solve the unknowns using algebra. 
	- The number of unknowns that you will be able to solve for will be the number of equilibrium equations that you have.
	- In instances where you have more unknowns than equations, the problem is known as a **statically indeterminate problem** and you will need additional information to solve for the given unknowns.
#### [[Bodies#Particles in Static Equilibrium Translational Equilibrium Translational Equilibrium in Concurrent Systems|Particle Translational Equilibrium in Concurrent Systems]]
A particle is said to be in equilibrium if it is at rest (and has been at rest) or is in motion with a constant velocity (i.e. no acceleration). 

To analyze equilibrium particles, [[Free Body Diagram|Free Body Diagrams]] are drawn to show all forces acting on the particle. 

Commonly found systems in these Free Body Diagrams of particles are:
###### Springs
With a spring length that changes in proportion to the force acting on it. 
![[Pasted image 20240519142716.png]]
###### Cables/Pulleys
Assume:
- Negligible weight.
- No stretch.
- Only support [[Curvature's Role in Stress Distribution#Tension (i.e. stretching stress)|tension]].

![[Pasted image 20240519142913.png]]
###### Contact Forces
A contact force is any force that occurs as a result of two objects making contact with each other.

Types of Contact Forces
###### Normal Force
![[Pasted image 20240519143551.png]]
Is a type contact force that's **perpendicular/orthogonal** to the surface that an object is in contact with. 
###### Friction Force
Is a type of contact force that occurs when two surfaces are in contact and moving or sliding against each other.
	Vs [[Curvature's Role in Stress Distribution#Shear Stress|Shearing Force]]
		Friction is a resistance force that occurs when two surfaces rub against each other. 
			Shear is a force that occurs when two misaligned forces push different parts of an object in opposite directions
###### Tension Force
Is a type of contact force that involves the pulling or stretching force transmitted axially along an object such as a string, rope, chain, rod, truss member, or other object, so as to stretch or pull apart the object.
	In terms of force, it is the opposite of compression.
#### Example: "Particle" Translational Equilibrium in Concurrent Systems











## [[Static Equilibrium#rotat|Rotational Equilibrium]]
Rotational equilibrium in a concurrent system typically involves less complexity regarding torque since any forces acting through the same point do not create torque about that point. Thus, if the forces are truly concurrent, the body does not experience rotational effects due to these forces. However, this assumption depends strictly on the perfect concurrency of all force vectors at a single point, which is an idealized scenario.
