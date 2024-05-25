---
up:
  - "[[Dynamics Analysis]]"
related:
  - "[["
date created: 2024-05-03
---
# Statics Analysis
Is a branch of mechanics that deals specifically with forces in equilibrium. 
	Unlike [[#Kinematics and Dynamics|kinematics and dynamics]] , which involve objects in motion, statics focuses on analyzing objects at rest or in a state where all forces and moments are balanced, leading to no motion.
##### Relationship to Kinematics, Dynamics, and Transformations
###### Kinematics and Dynamics
While [[Dynamics Analysis#Kinematics Identifying the "Present" (i.e. initial) State State (of condition, Parameters parameters ).|kinematics]] deals with the description of motion without regard to its causes.

[[Dynamics Analysis#Dynamics "Explains" the Causality of a State Change|Dynamics]] involves the forces causing those motions, statics strictly deals with systems where the net motion is zero due to balanced forces and moments. 

Thus, kinematics and dynamics may be considered when analyzing systems leading up to a state of equilibrium, but statics analyzes the condition of equilibrium itself.
###### Vs. Statics
Whereas Statics focuses on ensuring that all forces and moments are balanced (i.e. in [[Static Equilibrium|equilibrium]]) so that no net motion occurs. This is crucial in designing anything that must not move under load, such as buildings, bridges, or statues.
	 While these fields consider the effects of motion, statics is essentially the study of structures under conditions where motion should not occur. 
		 Any potential motion (displacement, rotation) considered in static analysis is only hypothetical, used to check the stability of the structure against such movements.
###### Core Concept
Statics involves studying bodies that are in **translational and rotational equilibrium**. This means that the sum of all forces acting on a body (translational equilibrium) and the sum of all torques (moments) acting on a body (rotational equilibrium) are zero.
###### Applications
This field is crucial in engineering, particularly in structural engineering, civil engineering, and architecture, where it is essential to ensure that structures can withstand various forces without moving or collapsing.
###### [[Newton's Second Law#Transformations as Motion (i.e. Representing Motion)|Transformations]]
In statics, transformations (translational and rotational) can still be relevant but in a conceptual or hypothetical sense. For example, in designing a structure, you might consider potential displacements (translations) and rotations caused by different loading scenarios to ensure that under actual conditions, these movements do not occur — the structure remains static, maintaining equilibrium.
## [[Bodies|Bodies]] in Statics Analysis
Refers to physical objects that can be analyzed in terms of their [[Newton's Second Law#Motion|motion]], forces acting upon them, and the resulting responses. 
#### [[Bodies#Particles|Particles]]
##### In Static Analysis Systems
###### [[#Concurrent Systems Concurrent Forces|Concurrent Systems]]
[[Static Equilibrium#Bodies Particles Particles|Particles in concurrent force systems]] are subjected to multiple forces that all pass through a single common point. Here, only translational equilibrium is considered (i.e., ∑𝐹⃗=0∑F=0).
###### [[Non-Concurrent Systems|Non-concurrent Systems]]
Even in [[#Non-Concurrent Systems Non-Concurrent Forces|non-concurrent systems]], where forces do not meet at a single point, particles are analyzed purely for translational equilibrium because they cannot exhibit rotational motion.
#### [[Bodies#Rigid Bodies|Rigid Bodies]]
###### [[Concurrent Systems|Concurrent Systems]]
For [[Static Equilibrium#Bodies Rigid Bodies Rigid Bodies|rigid bodies in concurrent systems]], the main concern is ensuring [[Static Equilibrium#Translational Equilibrium in Concurrent Systems|translational equilibrium]]. 
	Although all external forces act through one point, rotational equilibrium typically does not need separate analysis unless the point of concurrency is not at the center of mass.
###### [[Non-Concurrent Systems|Non-concurrent Systems]]
Rigid bodies in non-concurrent systems require careful analysis for both translational and [[Static Equilibrium#Rotational Equilibrium in Non-Concurrent Systems|rotational equilibrium]]. Forces acting at various points on the body create moments that must be balanced to maintain rotational equilibrium (∑𝜏⃗=0∑τ=0) around any point or, more conveniently, about the center of mass.
#### [[Bodies#Deformable Bodies|Deformable Bodies]]
Deformable bodies are analyzed less frequently in basic statics due to their complex behavior under load, but they are crucial in more advanced studies like strength of materials and [[Structural Analysis|structural analysis]].

The study often focuses on how deformations are distributed within the body and ensuring that the net forces and moments remain balanced to maintain overall static equilibrium.
## Vector
[[#Forces|Forces]] are vectors, which means they have both magnitude and direction. 
	When multiple forces act on a single point or body, they must be combined according to vector addition to find the net force.

A vector is a "resultant vector" that is **composed** of **component scalars**.
	These component scalars are applied to the **basis or standard unit vectors** of the given space. 
		Therefore, the vector is a linear combination of some scaled unit vectors.
			$\begin{equation*} \vec{v} = \begin{bmatrix} a \\ b \end{bmatrix}  = (a\vec{e_1} + b\vec{e_2})\end{equation*}$  
*See the physical Linear Algebra notes for a much more in depth study of vectors and linear systems of equations.*
###### Sense of a Vector
Refers to **the direction in which the vector is pointing**.
	I.e. It indicates the path of the vector from its initial point (tail) to its terminal point (head).
### Vector Addition
In vector addition, each vector is [[Static Equilibrium#Forms of Forces - Methods of Analyzing Physical Quantities|broken down]] into its **component scalars** (i.e. component "vectors" - that is the result of scaled unit vectors) along the x and y axes.
	The components along the same axis are added together to get the net force components in each direction.
![[Pasted image 20240508144941.png]]
![[Pasted image 20240508145006.png]]
In a two-dimensional setting:
- The x-components of all forces are added together to get the net force in the x-direction ($F_{net,x}$​).
- The y-components of all forces are added together to get the net force in the y-direction ($F_{net,y}$​).
### [[Statics Analysis#Static Equilibrium Point Forces|Point Forces]] as Vectors
A point force is any [[#Forces|force]] where the **[[Statics Analysis#Point of Application|point of application]]** is considered to be a **single point**.
	In reality, most forces are technically surface forces, where the force is applied over an area, but when the area is small enough (in comparison to the bodies being analyzed) it can often be approximated as a point force.

Because point forces can be represented as a single vector (rather than a field of vectors for distributed forces), they are much easier to work with in engineering analysis.
	For this reason, point forces are used in place of distributed forces in engineering analysis whenever possible. 

The tensions in the cables supporting this container can be treated as point forces pulling in the direction of the cables.
![[Pasted image 20240503162219.png]]

The friction force between the bow and string on this cello can be treated as a point force
![[Pasted image 20240503162235.png]]
### Dot Product (i.e. Scalar Product)
Is used extensively to project one vector onto another and to determine angles between vectors.
	It is defined mathematically between two vectors and results in a scalar (a single number), unlike the cross product, which results in a vector.

Used to find:
	- Can be used to determine if two vectors are orthogonal. 
	- The **angle** between two lines.
	- The components of a vector parallel and perpendicular to a line.
		- I.e. a **[[#Projections|projection]]** of the vector onto the line
###### How to Calculate
Given two vectors $𝑎$ and $b$ in $R^n$:
	Consider two [[Static Equilibrium#Unit Vector|unit vectors]] ($\vec{\hat{i}}, \vec{\hat{j}}$)
		Remember 
			The norm (i.e. magnitude) of a unit vector  is 1.
			The $\cos({90}\degree)= 0$ .
		Therefore, two **orthogonal** vectors have a dot product of zero. 
		![[Pasted image 20240509192651.png]]
		If the vectors are **parallel**, thus the angle between them is ${0}\degree$ then:
			The $\cos({0}\degree)= 1$ .
		Therefore, two parallel vectors have a dot product of 1. 
	Now remember the relative orientations of the axes:
		An $\vec{\hat{i}}$ component is **parallel** to the $x$ axis.
			$\large \vec{\hat{i}} \cdot \vec{\hat{i}}= 1$
		$x$ axis is **perpendicular** to the $y$ axis.
			$\large \vec{\hat{i}} \cdot \vec{\hat{j}}= 0$
		$x$ axis is **perpendicular** to the $z$ axis.
			$\large \vec{\hat{i}} \cdot \vec{\hat{k}}= 0$
		$y$ axis is **perpendicular** to the $z$ axis.
			$\large \vec{\hat{j}} \cdot \vec{\hat{k}}= 0$
			
The Dot product is calculated as:
	 $\large \vec{𝑎}⋅\vec{𝑏}=𝑎_{1}𝑏_{1}1+𝑎_{2}𝑏_{2}+…+𝑎_{𝑛}𝑏_{𝑛}$ ​ 
		Where $a1​,a2​,…,an$​ and $b1​,b2​,…,bn$​ are the components of vectors $\vec{a}$ and $\vec{b}$ respectively.
Derived from Vector (i.e. component) Form:
	$\large \vec{A} = A_{x}\hat{i} + A_{y}\hat{j} + A_{z}\hat{k}$
	$\large \vec{B} = B_{x}\hat{i} + B_{y}\hat{j} + B_{z}\hat{k}$
		$\large \vec{A}⋅\vec{B} = (A_{x}\hat{i} + A_{y}\hat{j} + A_{z}\hat{k}) \cdot (B_{x}\hat{i} + B_{y}\hat{j} + B_{z}\hat{k})$
			$\large \vec{A}⋅\vec{B} = (A_{x}\hat B_{x}\hat({i}\cdot {i}) + A_{y}\hat B_{y}\hat({j}\cdot{j}) + A_{z}\hat B_{z}\hat({k}\cdot{k}))$
				Remember the dot product of two parallel lines is 1.
					Therefore,
						$\large \vec{A}⋅\vec{B} = (A_{x} B_{x}) + (A_{y} B_{y}) + (A_{z} B_{z})$
###### Geometric Interpretation
The dot product can also be interpreted geometrically as: 
	$\large \vec{a}⋅\vec{b}=∥\vec{a}∥∥\vec{b}∥cosθ$
	$\large = θ = cos^{-1} ({|\vec{a}|⋅|\vec{b}| \over {a}{b}})$
		Where $∥\vec{a}∥$ and $∥\vec{b}∥$ are the magnitudes (i.e. [[Static Equilibrium#Norm of a Vector|norms]] or lengths) of the vectors.
		And θ is the angle between them. 
This interpretation is particularly useful in understanding the angle between vectors or projecting one vector onto another.
#### Projections
###### Parallel Projections
![[Pasted image 20240509203552.png]]
The **parallel projection** or the **parallel component of $\vec{A}$** 
- I.e. The **component of a vector $\vec{A}$** that is **parallel to line $a$** (i.e. is **on** line $a$).
	-  I.e. The line/vector that would be **adjacent** vector $\vec{A}$.
		- Which is found by  
			If $\large |\vec{A_{||_{a}}}| = |\vec{A}|\cos\theta$  where $\theta$ is the angle between the vector, $\vec{A}$ and its parallel projection, $\vec{A_{||_{a}}}$ 
				Then $\large \vec{\hat{u_{a}}} \cdot \vec{A_{||_{a}}} = \vec{\hat{u_{a}}}|\vec{A}| \cos \theta$ (*see the above* [[#Geometric Interpretation|Geometric Interpretation of Dot Product]])
					Remember the norm or magnitude of a unit vector, $\vec{\hat{U}}$, is 1.  
						$\vec{\hat{u_{a}}}|\vec{A}| == 1 \times |\vec{A}| = |\vec{A}|$
							Therefore,
								Projection of A onto line $\vec{\hat{u_{A}}}$ is
								 $\large \vec{A_{||}} = |\vec{A}|\cos \theta$ which was identified originally.
									Therefore, because the two "left-hand sides" of the equations are equal:
###### The Parallel Projection (magnitude) of **vector $\vec{A}$ *onto* line $\hat{u}$**=
	 $\large |\vec{A_{||_{a}}}| = \vec{\hat{u_{a}}} \cdot \vec{A_{||_{a}}}$ 
###### Vector or component form of the Parallel Projection of **vector $\vec{A}$ *onto* line $a$** =
$\large \vec{A_{||_{a}}} = |\vec{A}|\cos\theta\times \hat{u_{a}}$  
$\large == \vec{A_{||_{a}}} = (\vec{\hat{u_{a}}} \cdot \vec{A})\vec{\hat{u_{a}}}$
###### Orthogonal Projections
The **perpendicular/orthogonal projection**.
- I.e. The **component of a vector $\vec{A}$** that is **perpendicular to line $a$** (i.e. is **on** line $a$).
	-  I.e. The line/vector that would be **opposite** vector $\vec{A}$.
		 $\large \vec{A} = \vec{A_{||}} + \vec{A_{\perp}}$ because these are the "components" of vector $\vec{A}$
			 Therefore,
				 $\large \vec{A_{\perp}} =  \vec{A} - \vec{A_{||}}$ 
### Cross Product
At its core, the cross product of two vectors in three-dimensional space results in a new vector that is perpendicular to both original vectors. 
	This operation is fundamentally about orientation and magnitude in space.
		 $\large \vec{W_{\perp}} =  \vec{U} \times \vec{V}$ 
			Where $\large \vec{w_{\perp}}$ equals  =  $\vec{U}$ cross $\vec{V}$
##### The Magnitude of $\vec{w}$
Is defined as the product of the magnitudes of U and V and the sine of the angle $\theta$:
	$∥W∥=∥U∥∥V∥sin⁡(𝜃)$
		where 𝜃 is the angle between 𝑢 and 𝑣 . 
			This magnitude represents the area of the parallelogram spanned by 𝑢 and 𝑣.
##### The Direction of $\vec{w}$
![[Pasted image 20240525102935.png]]
Vector $\vec{W}$ has a direction that is perpendicular to the plane containing $\vec{U}$ and $\vec{V}$.
	Such that $\vec{w}$ is specified by the right-hand rule.

The magnitude and direction of $\vec{w}$ can be represented by:
	 $\large \vec{w_{\perp}} =  \vec{U} \times \vec{V} = (|U||V|sin⁡(\theta)) \times {\vec{u}_{c}}$ 
		Where the [[Static Equilibrium#Unit Vector|unit vector]] $\LARGE \vec{u}_{W}$ is the **direction** of $\vec{W}$.
			And where the scalar $|U||V|sin⁡(\theta)$ defines the magnitude of $\vec{W}$.
			 
###### Orientation and Right-Hand Rule
The direction of the cross product vector is determined using the right-hand rule.
	If you point your right hand's index finger in the direction of 𝑢u and your middle finger in the direction of 𝑣, your thumb will point in the direction of 𝑢×𝑣. 
		This rule helps to resolve the ambiguity since there are two possible perpendicular directions .
##### Geometric Interpretation
The cross product can be visualized in terms of the area and orientation of the parallelogram formed by the two vectors.
	If 𝑢 and 𝑣 are the vectors, the resulting vector 𝑤=𝑢×𝑣 is orthogonal (perpendicular) to the plane containing 𝑢 and 𝑣. 
##### Algebraic Properties
The cross product is not just about finding a perpendicular vector but also incorporates several key properties:
1. **Anticommutativity**: 𝑢×𝑣=−(𝑣×𝑢).
2. **Distributivity**: 𝑢×(𝑣+𝑤)=(𝑢×𝑣)+(𝑢×𝑤).
3. **Multiplication by a Scalar**: 𝑐(𝑢×𝑣)=(𝑐𝑢)×𝑣=𝑢×(𝑐𝑣) .

These properties ensure that the cross product behaves consistently with the geometric interpretation of vectors.

##### Significance in Physics and Engineering
The cross product is crucial in various physical applications, such as determining [[Moment|torque]], [[Newton's Second Law#Angular Momentum|angular momentum]], and the magnetic force on a moving charge. 
	These applications rely on the cross product's ability to encapsulate both magnitude and directional information about vector quantities in three-dimensional space.
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
##### [[Static Equilibrium#Norm of a Vector|Magnitude]] 
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
A point force is any force where the **[[Statics Analysis#Point of Application|point of application]]** is considered to be a **single point**.
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