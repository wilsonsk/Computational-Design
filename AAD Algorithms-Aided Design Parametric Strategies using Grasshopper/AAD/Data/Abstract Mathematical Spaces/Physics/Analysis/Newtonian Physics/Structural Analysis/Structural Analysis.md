---
up:
  - "[[Analysis]]"
related: 
date created: 2024-05-03
---
# Structural Analysis (i.e. Static Analysis)
  Structural analysis is a branch of civil engineering that involves the assessment and evaluation of the structural integrity and stability of buildings, bridges, and other structures. 
  
  The primary goal of structural analysis is to ensure that a structure can withstand various loads and forces it is expected to encounter over its service life without failing. 
	  This involves calculating the effects of loads, such as those from weight, wind, seismic activity, and other environmental and human-induced factors.

Structural analysis is not only about ensuring a structure does not fail but also about optimizing structures for cost, efficiency, and material use.
#### Key Aspects of Structural Analysis
###### Load Analysis
Structures must be analyzed for various types of loads they will experience. These include dead loads (the weight of the structure itself), live loads (weight of the users and movable objects), environmental loads (such as wind and snow), and dynamic loads (including impacts and vibrations).
###### Stress and Strain Calculations
The analysis involves determining the stresses (forces per unit area) and strains (deformations in a body) that occur in different components of a structure under load. The aim is to ensure that these stresses and strains do not exceed the material strengths.
###### Factor of Safety
Structures are designed with a factor of safety, which is a margin of error that accounts for uncertainties in the load assumptions, material properties, and structural behavior.
###### Behavior Under Loads
Understanding how a structure behaves under expected loads is crucial. This includes analyzing deflections (how much a structure bends or displaces), rotations, and potential buckling (sudden failure due to compressive forces).
###### Methods and Tools
Modern structural analysis often utilizes software and computational tools that employ methods like the Finite Element Method (FEM), which allows detailed simulations of how structures respond to loads.
Traditional methods such as the Method of Joints, Method of Sections, and Matrix methods are still fundamental and are used to calculate internal forces and moments manually or semi-automatically.
###### Design Compliance and Safety Codes
Structural analysis ensures that designs comply with local and international building codes and safety standards, which dictate minimum requirements for safety, stability, and durability.
## Vector
[[#Forces|Forces]] are vectors, which means they have both magnitude and direction. 
	When multiple forces act on a single point or body, they must be combined according to vector addition to find the net force.

A vector is a "resultant vector" that is **composed** of **component scalars**.
	These component scalars are applied to the **basis or standard unit vectors** of the given space. 
		Therefore, the vector is a linear combination of some scaled unit vectors.
			$\begin{equation*} \vec{v} = \begin{bmatrix} a \\ b \end{bmatrix}  = (a\vec{e_1} + b\vec{e_2})\end{equation*}$  
*See the physical Linear Algebra notes for a much more in depth study of vectors and linear systems of equations.*
### Vector Addition
In vector addition, each vector is [[Static Equilibrium#Forms of Forces - Methods of Analyzing Physical Quantities|broken down]] into its **component scalars** (i.e. component "vectors" - that is the result of scaled unit vectors) along the x and y axes.
	The components along the same axis are added together to get the net force components in each direction.

In a two-dimensional setting:
- The x-components of all forces are added together to get the net force in the x-direction ($F_{net,x}$​).
- The y-components of all forces are added together to get the net force in the y-direction ($F_{net,y}$​).
### [[Structural Analysis#Static Equilibrium Point Forces|Point Forces]] as Vectors
A point force is any [[#Forces|force]] where the **[[Structural Analysis#Point of Application|point of application]]** is considered to be a **single point**.
	In reality, most forces are technically surface forces, where the force is applied over an area, but when the area is small enough (in comparison to the bodies being analyzed) it can often be approximated as a point force.

Because point forces can be represented as a single vector (rather than a field of vectors for distributed forces), they are much easier to work with in engineering analysis.
	For this reason, point forces are used in place of distributed forces in engineering analysis whenever possible. 

The tensions in the cables supporting this container can be treated as point forces pulling in the direction of the cables.
![[Pasted image 20240503162219.png]]

The friction force between the bow and string on this cello can be treated as a point force
![[Pasted image 20240503162235.png]]
### Force Vector Representation
When vectors are drawn to form [[Free Body Diagram|free body diagrams]], the magnitude and direction are usually given in one of two formats (i.e. [[Static Equilibrium#Vector Form Analysis (i.e. Cartesian Vectors)|vector form]] or [[Static Equilibrium#Scalar Form Analysis|scalar form]]).

In either format we will need two values to fully define a force vector in a 2D system (either a magnitude and a single angle or a magnitude in each of the two coordinate axes).

And three values to fully define a force vector in a 3D system (either a magnitude and two angles or a magnitude in each of the three coordinate axes). 
## Forces
![[Pasted image 20240503130700.png]]
Refers to any influence that causes a body to accelerate. 
Forces on a body can also cause stress in that body, which can result in the body [[Grids#Deformation Operations|deforming]] or breaking.
	Though forces come from a variety of sources, there are three distinguishing features to **every force**.
A force can be linear or [[#Moments (i.e. Torque)|angular]], "forces" typically refers to linear forces, while [[#Moments (i.e. Torque)|moments]] refer to angular or twisting forces.
### Force Features
##### Magnitude 
The degree to which the force will accelerate the body it is acting on.
	It is represented by a single number - i.e. a scalar. 
Can be thought of as the "strength" of a force.

Measured in units of $\begin{equation*} \LARGE (mass) \times (distance) \over \LARGE (time)^2 \end{equation*}$
	The most common unit is the **Newton (N)** where:
		$\begin{equation*} \LARGE 1 (N) = (kg) \times (mass) \over \LARGE (1 second)^2 \end{equation*}$
##### Direction
The direction of the force being applied to a body. 
Has no units, but is usually given by reporting angles between the vector representing the force and the coordinate axes.
	Or given by the $\LARGE x,y,z$ components of the vector.
##### Point of Application
The point at which the force is applied to a body.
For [[#Particle|particles]] there is only a **single point** for the forces to act on.
For [[#Rigid Body|rigid bodies]] there are an infinite number of possible points of application.

Some points of application will lead to the body undergoing simple linear acceleration and others will exert a moment on the body which will cause the body to undergo rotational acceleration as well as linear. 
##### Point of Concurrency
Refers to the location where multiple force lines of action intersect. 
- In a concurrent force system, all the forces meet or are assumed to meet at this single point. This point is crucial for the analysis of the system because it simplifies calculations related to moments—since the moment arm length is zero at this point, the moments created by these forces about this point are zero.
- In non-concurrent systems, each force has its distinct point of application and does not necessarily meet at a single point of concurrency. Here, the point of application becomes critical in determining the moment arms when calculating moments about any point of interest for ensuring rotational equilibrium.
##### Line of Action
![[Pasted image 20240503190901.png]]
The line of action of a force is the line along which the force acts. 
	It is the geometric representation of how the force is applied. 
	Given the direction and point of application, one can find the line of action, but this term will be important in discussing concurrent forces and in the principle of transmissibility.
### Three General Types of Forces
The type of resulting force depends on the nature of the [[#Point of Application|point of application]].
###### [[Static Equilibrium|Point Forces]]
![[Pasted image 20240503131754.png]]
A point force is any force where the **[[Structural Analysis#Point of Application|point of application]]** is considered to be a **single point**.
Point forces are represented by a single vector. 
###### Surface Forces
![[Pasted image 20240503131804.png]]
Surface forces are indicated by a number of vectors graphed side by side with a profile line to indicate the magnitude of the force at any point. 
	Is a type of distributed force.
###### Body Forces
![[Pasted image 20240503131813.png]]
Body forces are sometimes shown as a [[Scalar Fields|field]] of vectors.
	Is a type of distributed force.
###### Principle of Transmissibility
![[Pasted image 20240503132426.png]]
The point of application of a force can be moved anywhere along its line of action without changing the external reaction forces on a rigid body.
	Only valid for rigid bodies.

Any force that has the same magnitude and direction, and which has a point of application somewhere along the same line of action will cause the same acceleration and will result in the same moment.
	 Therefore, the points of application of forces may be moved along the line of action to simplify the analysis of rigid bodies.

Therefore, the exact point or surface that the force is acting on can be drawn as either the head or the tail of the force vector in the free body diagram.
![[Pasted image 20240504001503.png|400]]

However, **when analyzing the internal forces** (stress) in a rigid body, the exact point of application does matter. 
	This difference in stresses may also result in changes in geometry which will in turn affect reaction forces. 
		For this reason, the principle of transmissibility should only be used when examining **external forces** on bodies that are assumed to be rigid.
		![[Pasted image 20240504001606.png]]
###### [[Concurrent Systems|Concurrent Forces]]
![[Pasted image 20240504001917.png]]
A set of [[#Static Equilibrium Point Forces|point forces]] is considered concurrent if all the [[#Line of Action|lines of action]] of those forces all come together at a single point.

Because the forces all act through a single point, **there are no moments about this point**.
	Because no moments exist, we can treat this body as a **particle**. 
		In fact, because real particles only exist in theory, most particle analysis is actually applied to extended bodies with concurrent forces acting on them.
###### [[Non-Concurrent Systems|Non-Concurrent Forces]]
![[Pasted image 20240504111352.png|200]]
For an **rigid body** in static equilibrium—that is, a non-deformable body where **forces are not concurrent**—the sum of both the **forces** and the **moments** acting on the body must be equal to zero.

The addition of moments (as opposed to particles, where we only looked at the forces) adds another set of possible equilibrium equations, allowing us to solve for more unknowns as compared to particle problems.

Moments, like forces, are vectors. This means that our vector equation needs to be broken down into scalar components before we can solve the equilibrium equations.















###### A straight line that connects the line of action of a force to some point in the rigid body.
It is the shortest distance between them, i.e. perpendicular/orthogonal.
	The length of this line can be called $d$.
		This distance 𝑑d is crucial because it determines the lever arm, which is the effective distance at which the force can cause rotation about the point or axis.
### Moment of a Force (about a point or axis) aka Torque
![[Pasted image 20240502152224.png]]
![[Pasted image 20240502152321.png]]
The **moment of a force** is the tendency of some forces to cause rotation.

The moment of a force (often called torque) about a point or axis is the product of the force magnitude, $P$, and the perpendicular distance, $d$, from the point or axis to the line of action of the force.

It is the assessment of the potential of the force to cause rotation about that specific point or axis.

Magnitude of a force, $F$ produces a Moment about a point, $c$.

The Moment, $M$

###### Magnitude of the Moment
In this case, it is the degree of rotation the moment would cause.

The magnitude is calculated as $∣M∣=∣r∣∣F∣sin(θ)$, where $θ$ is the angle between the position vector and the force vector. 
	**If the distance $d$ is the perpendicular distance from the line of action of the force to the axis or point of rotation**, then the magnitude can also be simply expressed as **$M=F \times d$.**



###### Rational Tendency

Distance from a point to the line of action of these forces