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
##### 1. Draw [[Free Body Diagram|Free Body Diagrams]]
###### Identify the Point of Concurrency (i.e. System Component Isolation)
Draw a [[Free Body Diagram|free body diagram]] of each body or point of concurrency being analyzed to determine the common point through which all the forces act - this is the **point of concurrency**.
	In the context of concurrent systems, where multiple forces meet at certain points, **each component or point of the system that experiences different forces** should **have its own Free Body Diagram (FBD)**.

Each part of the system (e.g., individual springs, the weight) is considered separately to analyze the forces and moments acting on it.
###### 1. **Individual Components or Objects**
Each distinct physical object or component in the system that has forces acting on it should have its own FBD.
- Also called the "body of interest".
	- **Example**: The block or mass in a spring system.
		Weight (Mass):
		- **Load or Object FBD**: The free body diagram for the mass (or weight) (for example hanging from the springs).
			- Shows the forces acting on the weight, including the gravitational force (weight) and the tension forces from the springs.
###### 2. Springs Connected at Junction
- **Spring FBD**: The free body diagram for the individual springs.
	- Shows the forces acting on each spring, including the tension forces at the points where they connect to the weight and to the supports.
	- Each spring is isolated to show the forces acting on it.
	- Displays the tension forces at the points where the spring connects to other parts of the system (e.g., the weight and the junction points).
###### 3. Junction or Connection Point
- **Junction FBD**: The free body diagram for the point where the springs are connected (e.g., point A).
	- Shows the forces acting on the junction from each of the springs and any external forces.
	- Sometimes referred to as "nodes" in structural analysis.
	- The point where multiple springs or forces converge.
	- Shows the forces acting at the junction from each of the springs and any other external forces.
###### 4. Forces and Moments at Each Point
The forces and moments acting at each specific location where different components are connected or where external forces are applied.
    - **Example**: Forces exerted by springs at the connection point.

The diagram should show all the known and unknown force vectors acting externally on the body.
- In the free body diagram, provide values for any of the know magnitudes or directions for the force vectors and provide variable names for any unknowns (either magnitudes or directions).
	![[Pasted image 20240504003640.png]]
##### 2. Chose the $x, y, z$ Axes
These axes must be perpendicular to one another, but do not need to necessarily have to be horizontal or vertical. 
##### 3. [[Static Equilibrium#Decomposing Forces|Decomposition]]
Break down all of the force vectors into [[Static Equilibrium#Vector Form Analysis (i.e. Cartesian Vectors)|component scaled unit vectors]] along the $x, y, x$ directions. 
	If forces are given in vector form or applied at angles to a coordinate system, resolve each force into its orthogonal components (typically along x, y, and possibly z axes in three-dimensional space).
- The first equation will be the sum of the magnitudes of the components in the $𝑥$ direction being equal to zero.
- The second equation will be the sum of the magnitudes of the components in the $y$ direction being equal to zero.
- And the third (if a 3D problem) will be the sum of the magnitudes in the $z$ $direction being equal to zero.
- Collectively these are known as the **equilibrium equations**.
##### 4. Sum up the Force Components
Solve the unknowns using algebra. 
	- The number of unknowns that you will be able to solve for will be the number of equilibrium equations that you have.
	- In instances where you have more unknowns than equations, the problem is known as a **statically indeterminate problem** and you will need additional information to solve for the given unknowns.
### [[Bodies#Particles in Static Equilibrium Translational Equilibrium Translational Equilibrium in Concurrent Systems|Particle Translational Equilibrium in Concurrent Systems]]
A [[Bodies#Particles in Static Equilibrium Translational Equilibrium Translational Equilibrium in Concurrent Systems|particle in Translational Equilibrium]] is said to be in equilibrium if it is at rest (and has been at rest) or is in motion with a constant velocity (i.e. no acceleration). 

To analyze equilibrium particles, [[Free Body Diagram|Free Body Diagrams]] are drawn to show all forces acting on the particle. 

Commonly found systems in these Free Body Diagrams of particles are:
#### Particle Spring Systems
The force exerted by a spring is proportional to its displacement from the equilibrium position according to [[Form-Finding Strategies Using Kangaroo#Hooke's Law|Hooke's Law]]: $\LARGE F=kΔx$.
	With a spring length that changes in proportion to the force acting on it. 
###### Variable Magnitude of the Force Along a Spring
The magnitude of a force along a spring can change depending on the displacement of the spring from its equilibrium position. This is a key characteristic of spring forces described by [[Form-Finding Strategies Using Kangaroo#Hooke's Law|Hooke's Law]].
	As the displacement ($\large Δx$) changes, the magnitude of the force ($|\vec{F}|$) changes proportionally.
		This means that as the spring stretches or compresses, the displacement ($Δx$) changes, which **means the force magnitude changes, thus the force exerted by the spring is not constant**.
			It **varies as the spring stretches or compresses**.
###### Variable Component Vectors of Force Vectors Along a Spring
And therefore, the **component vectors of the Force Vectors** change as well.
	I.e. As the spring extends (i.e. as the displacement ($Δx$) changes), the x and y components can change (relative to their [[Form-Finding Strategies Using Kangaroo#Rest Length|rest lengths]]) because the overall displacement and hence the force changes.
![[Pasted image 20240519142716.png]]
#### Cables/Pulleys
Assume:
- Negligible weight.
- No stretch.
- Only support [[Curvature's Role in Stress Distribution#Tension (i.e. stretching stress)|tension]].

![[Pasted image 20240519142913.png]]
#### Contact Forces
A contact force is any force that occurs as a result of two objects making contact with each other.

##### Types of Contact Forces in Concurrent Particle Systems
###### [[Free Body Diagram#Normal Forces (i.e. Reaction Forces)|Normal Force]]
![[Pasted image 20240519143551.png]]
Is a type contact force that's **perpendicular/orthogonal** to the surface that an object is in contact with. 
###### [[Free Body Diagram#Friction Forces|Friction Force]]
Is a type of contact force that occurs when two surfaces are in contact and moving or sliding against each other.
	Vs [[Curvature's Role in Stress Distribution#Shear Stress|Shearing Force]]
		Friction is a resistance force that occurs when two surfaces rub against each other. 
			Shear is a force that occurs when two misaligned forces push different parts of an object in opposite directions
###### [[Free Body Diagram#Tension Forces|Tension Force]]
Is a type of contact force that involves the pulling or stretching force transmitted axially along an object such as a string, rope, chain, rod, truss member, or other object, so as to stretch or pull apart the object.
	In terms of force, it is the opposite of compression.
### Example: Translational Equilibrium in Concurrent Particle Spring Systems
*Note: this problem is different than that problems from [[Static Equilibrium#Force Directed Along a Line (i.e. an example of the position vector method)|previous problems]] where the coordinates or dimensions were used as the [[Static Equilibrium#Vector Form Analysis (i.e. Cartesian Vectors)|components]] of the [[Statics Analysis#Force Vector Representation|Force Vector]].*
	*This is a **SPRING** system, compared to a force within or along a line or cable.*
	*In this new example problem, the dimensions can still be used to find the angle (via tangent function) of the force vectors, but they **can not** be used as **component vectors**.*
		*[[#Springs#Variable Component Vectors of Force Vectors Along a Spring|Remember]], the springs themselves can be compressed or stretched.* 
			*Because the springs are [[Form-Finding Strategies Using Kangaroo#Extensibility|extendible]], the [[#Variable Magnitude of the Force Along a Spring|magnitude of the Force Vectors are variable]].*
				*Therefore, the dimensions are not the components because depending on the magnitude of the force along the spring, the x and y component vectors can differ from their starting dimensions- i.e. their [[Form-Finding Strategies Using Kangaroo#Rest Length|rest lengths]].*
 
![[Pasted image 20240521130100.png|500]]
*Note* this problem asks for the "stretch" of the springs- not the spring force (i.e. the magnitude of the spring Force Vectors).
	"Stretch" refers to the "s" or "x" - the [[#Springs|displacement of the spring]].
#### Steps
1. Create a [[#1. Draw Free Body Diagram Free Body Diagrams|Free Body Diagram]] for each component or point of the system that experiences different forces.
	1. The $y$ components of the Force Vector:
		![[Pasted image 20240521132457.png]]
	2. The $x$ components of the Force Vector:
		![[Pasted image 20240521133017.png|400]]
2. Decompose the Force Vectors as Means to Find the Spring Force Vector Magnitudes
	As further means to derive the "stretch" values for each spring Force Vector. 
	1. The $y$ components of the Force Vector:
		Which contain the "mass or weight" of the [[#1. **Individual Components or Objects**|body of interest]]
		![[Pasted image 20240521132641.png]]
	2. The $x$ components of the Force Vector:
		In this case the angles are not given.
			Therefore we can use the tangent function to extract the angle given the dimensions of the rest lengths of force vectors' components. 
				![[Pasted image 20240521133118.png]]
			Once the angle is acquired, we can then use the angle to find the $x$ components - as they lie adjacent to the Force Vector.
				Remember, the dimensions cannot be used as the components themselves in spring systems, because of the [[#Variable Component Vectors of Force Vectors Along a Spring|extendibility inherent ]]to the springs.
					So $\sum |\vec{F_{x}}| \space != -3\hat{i} + 4\hat{i}$  where $3\hat{i}$ and$4\hat{i}$ are the dimensions given.  
						But instead is:
							![[Pasted image 20240521133900.png]]
							![[Pasted image 20240521133914.png]]
							![[Pasted image 20240521134032.png]]
		The result is the magnitude of the Force Vector for $spring_{AC}$ (aka $\LARGE |\vec{F{s_{AC}}}|$) which is $15.848N$
			With this value, we can now find the "stretch" or displacement value of the spring AC (aka $\large s_{AC}$).
				$\LARGE F=kΔx$.
					The problem gives $K_{AC}$ as $20{N\over m}$
					![[Pasted image 20240521134850.png]]
		To get the "stretch" ($\large s_{AB}$) of Force Vector AB ($\vec{F_{AB}}$) we need the spring Force Vector Magnitude ($|\LARGE \vec{F_{s{AB}}}|$).
			To obtain that we just plug in ($\LARGE \vec{F_{s_{AC}}}$) into our $\LARGE \vec{F_{x}}$ equilibrium equation. 
				![[Pasted image 20240521133900.png]]
				![[Pasted image 20240521135543.png]]
## [[Static Equilibrium#rotat|Rotational Equilibrium]] in Concurrent Systems
Rotational equilibrium in a concurrent system typically involves less complexity regarding torque since any forces acting through the same point do not create torque about that point. Thus, if the forces are truly concurrent, the body does not experience rotational effects due to these forces. However, this assumption depends strictly on the perfect concurrency of all force vectors at a single point, which is an idealized scenario.
