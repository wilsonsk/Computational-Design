---
up:
  - "[[Structural Analysis]]"
related:
  - "[[Non-Concurrent Systems]]"
  - "[[Analysis]]"
  - "[[Static Equilibrium]]"
date created: 2024-05-04
---
# Concurrent Force Systems
If a body is in static equilibrium, then by definition that body is not accelerating. 
	If we know that the body is not accelerating then we know that **the sum of the forces acting on that body must be equal to zero**. 
		This is the basis of Concurrent Force equilibrium analysis (I.e. Translational Equilibrium) of a body. 
		
A set of [[Structural Analysis#Structural Analysis Static Equilibrium Point Forces Point Forces as Vectors|point forces]] is considered concurrent if all the [[Structural Analysis#Line of Action|lines of action]] of those forces all come together at a single point.

Because the forces all act through a single point, **there are no [[Non-Concurrent Systems#Moments (i.e. Torque)|moments]] about this point**.
	Because no moments exist, we can treat this body as a **particle**. 
		In fact, because real particles only exist in theory, most particle analysis is actually applied to extended bodies with concurrent forces acting on them.
###### Particles
These are a "body" under analysis within these Concurrent Systems.		
###### Rigid Body
These are the "body" under analysis within Non-Concurrent Systems.
Particles of a rigid body cannot move independent of the rigid body.
	Specifically, the particle of a rigid body can only move if its **distance** from some other point on the rigid body remains the same. 

![[Pasted image 20240504001917.png]]
## General Static Equilibrium Analysis for Concurrent Force Systems
In order to solve for any unknowns in the sum of forces equation, turn the one vector equation into a set of scalar equations. 
	For two dimensional problems, split our one vector equation down into two scalar equations. 
		We do this by summing up all the $x$ components of the force vectors and setting them equal to zero in our first equation.
			Then summing up all the $y$ components of the force vectors and setting them equal to zero in our second equation.
	For three dimensional problems, add a third equation.
		The sum of all our $z$ components equal to zero.

 $\LARGE \sum{\vec{F_y}}​=0$
 $\LARGE \sum{F_x}​=0$ ; $\LARGE \sum{F_y}​=0$ ; $\LARGE \sum{F_z}​=0$
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
###### 3. Decomposition
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