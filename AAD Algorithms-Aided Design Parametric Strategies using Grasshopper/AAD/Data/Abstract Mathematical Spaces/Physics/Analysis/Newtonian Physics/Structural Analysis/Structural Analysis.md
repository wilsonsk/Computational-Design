---
up:
  - "[[Analysis]]"
related: 
date created: 2024-05-03
---
# Structural Analysis (i.e. Static Analysis)
## Vector
[[#Forces|Forces]] are vectors, which means they have both magnitude and direction. 
	When multiple forces act on a single point or body, they must be combined according to vector addition to find the net force.

A vector is a "resultant vector" that is **composed** of **component scalars**.
	These component scalars are applied to the **basis or standard unit vectors** of the given space. 
		Therefore, the vector is a linear combination of some scaled unit vectors.
			$\begin{equation*} \vec{v} = \begin{bmatrix} a \\ b \end{bmatrix}  = (a\vec{e_1} + b\vec{e_2})\end{equation*}$  
*See the physical Linear Algebra notes for a much more in depth study of vectors and linear systems of equations.*
### Vector Addition
In vector addition, each vector is broken down into its **component scalars** (i.e. component "vectors" - that is the result of scaled unit vectors) along the x and y axes.
	The components along the same axis are added together to get the net force components in each direction.

In a two-dimensional setting:
- The x-components of all forces are added together to get the net force in the x-direction ($F_{net,x}$​).
- The y-components of all forces are added together to get the net force in the y-direction ($F_{net,y}$​).
## Forces
![[Pasted image 20240503130700.png]]
Refers to any influence that causes a body to accelerate. 
Forces on a body can also cause stress in that body, which can result in the body [[Grids#Deformation Operations|deforming]] or breaking.
	Though forces come from a variety of sources, there are three distinguishing features to **every force**.
A force can be linear or [[#Moments (i.e. Torque)|angular]], "forces" typically refers to linear forces, while [[#Moments (i.e. Torque)|moments]] refer to angular or twisting forces.
#### Force Features
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
##### Line of Action
![[Pasted image 20240503190901.png]]
The line of action of a force is the line along which the force acts. 
	It is the geometric representation of how the force is applied. 
	Given the direction and point of application, one can find the line of action, but this term will be important in discussing concurrent forces and in the principle of transmissibility.
##### Three General Types of Forces
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
###### Concurrent Forces
![[Pasted image 20240504001917.png]]
A set of [[#Static Equilibrium Point Forces|point forces]] is considered concurrent if all the [[#Line of Action|lines of action]] of those forces all come together at a single point.

Because the forces all act through a single point, **there are no moments about this point**.
	Because no moments exist, we can treat this body as a **particle**. 
		In fact, because real particles only exist in theory, most particle analysis is actually applied to extended bodies with concurrent forces acting on them.
## Moments (i.e. Torque)
![[Pasted image 20240503132914.png]]
Refers to a quantity related to the rotational effects produced by a force.

Refers to the tendency of a force to rotate (i.e. produce or change rotational motion)a body.
Moments cause **angular accelerations**.
	In this way, moments can be thought of as **"twisting forces"**.
Are represented by [[#Vector|vectors]] = - i.e. have a magnitude, direction and point of application.
##### Etymology and Historical Use
###### Origins
The term "moment" in physics comes from the Latin word _momentum_, which means "movement" or a very brief portion of time.
	Historically, this term was used in various mechanical contexts to describe something of importance in determining motion or an outcome, such as the effect of a lever.
		The word was likely chosen because, like a brief moment in time can be pivotal, a mechanical moment describes the pivotal effect that a force can have in generating rotational motion.
##### Other Types of Moments
###### Moment of Inertia
This is another crucial concept in dynamics, describing how the mass of a body is distributed relative to an axis of rotation. The moment of inertia affects the rotational motion of an object but is not a force. It plays a role in the rotational version of Newton's second law, which relates torque, moment of inertia, and angular acceleration.
###### Bending Moment
In structural engineering, a bending moment is the internal reaction induced in a structural element when external forces cause the element to bend. It’s expressed in terms of the force multiplied by the distance to the point of interest along the element, influencing how beams and other structural components are designed to withstand loads.
###### Magnetic Moment
In physics, particularly in electromagnetism, the magnetic moment refers to the magnetic strength and orientation of a magnet or other object that produces a magnetic field. It is a vector quantity determining how a magnetic object will react in a magnetic field.
##### Axis of Rotation	
However, the [[#Point of Application|point of application]] in the context of moments, is referred to as the **axis of rotation**.
	This is the point or axis about which we will determine all the moments.
![[Pasted image 20240503133748.png]]
*In the above image, the single force (vector) would cause different moments depending on if it is "about" (i.e. in relation to) point $A$ or point $B$, and thus different rotations.*

The axis of rotation is therefore the **point we chose to fix in place**, which the body being exerted up will then rotate about. 

The axis of rotation is a "chosen point".
	The chosen point will affect the magnitude and direction of the resulting moment.
		And the moment is only valid about that point. 

When adding together moments from multiple forces, all the moments must be taken "about" (i.e. in relation to) a **shared/common axis of rotation**.
	Moments taken about different points cannot be added together to find a "net moment".

When working in **dynamics** (i.e. moving bodies) all moments will need to relate to angular accelerations. 
	Therefore, the shared/common axis of rotation will need to be a stationary one. 
##### Magnitude of a Moment
Is the degree to which the moment will cause angular acceleration in the body it is acting on. 
	It is represented by a scalar (i.e. a single number).
Can be thought of as the "strength" of the twisting force exerted on the body.

The magnitude of a moment, $M$, is measured in:
	$\begin{equation*} \LARGE M = F \times d \end{equation*}$
Where $F$ is the force, and $d$ is the distance.

The standard unit of measurement for for the magnitude of moments are Newton-meters ($\begin{equation*} \LARGE N \times m \end{equation*}$), and the standard English unit of measurement is foot-pounds ($\begin{equation*} \LARGE lb \times ft \end{equation*}$).
###### Direction of a Moment
In a 2D space, the direction can be thought of a scalar quantity corresponding to the direction of rotation the moment would cause.
	A moment that would cause a **counterclockwise rotation** is a **positive moment**.
	A moment that would cause a **clockwise rotation** is a **negative moment**.

In a 3D space, a body can rotate about an axis in any direction.
	Therefore, a vector is needed to represent the direction of a moment.
		The direction of a moment vector will line up with the axis of rotation that moment would cause, but to determine which of the two directions to use along that axis, the "right hand rule" is employed.
###### Right Hand Rule:
![[Pasted image 20240503140615.png]]
To use the right hand rule, align your right hand so that your thumb lines up with the axis of rotation for the moment and your curled fingers point in the direction of rotation for your moment. 
	If you do this, your thumb will be pointing in the direction of the moment vector.

### Calculating Moments
To calculate the moment that a force exerts on a body, two methods can be used.
##### Scalar Methods

##### Vector Methods



















## Equilibrium
For a system to be in equilibrium, the net force in both the x and y directions must be zero. 
	Mathematically, this is written as: $ΣF_x​=0$ and $ΣF_y​=0$
		It's the principle of superposition that allows this vector addition to work: the effect of the individual forces can be added together to get the total effect. 
			In equilibrium problems, this principle is used to ensure that all forces balance out, resulting in no net motion of the object in question.


### Rigid Body Rotational Equilibrium 
##### Two Ways to Use These Equations
1. Do the given set of forces place the rigid body in a state of equilibrium?
2. Determine the magnitude or direction of one or more unknown forces, needed to maintain equilibrium?
###### Rigid Body
Particles of a rigid body cannot move independent of the rigid body.
	Specifically, the particle of a rigid body can only move if its **distance** from some other point on the rigid body remains the same. 

##### Concept of Lever Arm
###### Lever Arm (Distance $d$)
The distance 𝑑d in the formula represents the lever arm. 
	The lever arm is the perpendicular distance from the axis or point of rotation to the line of action of the force. 
		This distance determines how effectively a force can cause an object to rotate around that point or axis.
###### The Force ($P$)
The force magnitude $P$ is the amount of push or pull applied.
	The direction and point at which this force is applied relative to the point of rotation determine the effectiveness of the force in causing rotational movement.
###### A Force Acts Directly on a Particle in a Rigid Body

###### And a Force Acts at a Distance from the Other Particles in a Rigid Body


###### Line of Action of a Force


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

##### Why Multiply Force by Distance?
###### Amplification by Distance
The further away the force is applied from the point or axis of rotation, the greater its ability to cause rotation. 
	This is because a longer lever arm (greater distance $d$) means that the same amount of force can produce a larger turning effect. 
		This principle is observable in everyday tools like wrenches or door handles — longer handles require less force to operate because they have a longer lever arm.

###### Rational Tendency

Distance from a point to the line of action of these forces