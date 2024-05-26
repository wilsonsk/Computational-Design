---
up:
  - "[[Newtonian Mechanics]]"
related:
  - "[[Non-Concurrent Systems]]"
  - "[[Concurrent Systems]]"
  - "[[Dynamics Analysis]]"
date created: 2024-05-15
---
# Moment (i.e. Torque)
![[Pasted image 20240503132914.png]]
Refers to a quantity related to the rotational effects produced by a force.
	When a force is applied to a [[Bodies|body]] it will produce a tendency for the body to **rotate about a point that is *not* on the [[Statics Analysis#Line of Action|line of action]] of the force**.
		This tendency to rotate is sometimes called a **torque**, but most often it is called the **moment of a force**, or more simply the moment.

Refers to the tendency of a force to rotate (i.e. produce or change rotational motion)a body.
Moments cause **angular accelerations**.
	In this way, moments can be thought of as **"twisting forces"**.
Are represented by [[#Vector|vectors]] = - i.e. have a magnitude, direction and point of application.
#### The Moment Value
A moment value (or torque) does describe the **likelihood or ease of rotation** about a point or axis. 
	A higher magnitude of the moment indicates a greater tendency for the object to rotate. 
		The moment (or torque) of a force about a point is a measure of its tendency to cause rotation about that point.
			It is calculated as:
					$M=F×d$
				Where M is the moment, F is the magnitude of the force, and d is the perpendicular distance from the point of interest to the line of action of the force.
###### High Moment Value
A high moment value implies that the force, combined with the distance from the point of rotation, creates a significant turning effect.
		This makes it easier to rotate the object around the point or axis.
###### Low Moment Value
A low moment value indicates a weaker turning effect, making it less likely to cause rotation.
###### [[#Magnitude of a Moment|Magnitude]] of the Moment
The magnitude of the moment indicates the strength of the rotational effect.
	A larger moment means a stronger rotational effect and, therefore, a higher likelihood of causing rotation.

Moments occur when forces are applied such that they do not all act through a single point (i.e., in [[Static Equilibrium#Static Equilibrium Analysis for Concurrent Force Systems|non-concurrent force systems]]).
	In these cases, **the forces have the potential to create rotational effects about a point or axis**, and these effects are described by moments.
#### Etymology and Historical Use
###### Origins
The term "moment" in physics comes from the Latin word _momentum_, which means "movement" or a very brief portion of time.
	Historically, this term was used in various mechanical contexts to describe something of importance in determining motion or an outcome, such as the effect of a lever.
		The word was likely chosen because, like a brief moment in time can be pivotal, a mechanical moment describes the pivotal effect that a force can have in generating rotational motion.
#### [[Non-Concurrent Systems|Non-Concurrent Force Systems]]
###### Moment Creation
In non-concurrent systems, since forces do not all pass through one common point, each force can be associated with a moment arm relative to any chosen point of rotation. The moment arm is the perpendicular distance from the point or axis of rotation to the line of action of the force.
###### Calculating the Moment
The moment caused by a force in such systems is calculated as the cross product of the position vector r (from the point of rotation to the point where the force is applied) and the force vector F, expressed as $M=r×F$. This moment (or torque) measures the tendency of the force to cause rotational motion about the point or axis.
#### [[Static Equilibrium#Static Equilibrium Analysis for Concurrent Force Systems|Concurrent Force Systems]]
**Moment Creation**
In a concurrent system, if the point of concurrency is chosen as the axis of rotation, the moment arm is zero, resulting in zero torque.
###### Point of Concurrency
However, if a different point (not the point of concurrency) is chosen as the axis of rotation, there will be a non-zero perpendicular distance (moment arm) from this point to the lines of action of the forces.
	This non-zero moment arm results in the generation of torque by each force about the chosen axis of rotation.
	    I.e. Where all forces intersect.
		    At this point, if it is chosen as the axis of rotation, the moment arm for each force is zero because the force's line of action passes through this point.
###### Axis of Rotation
Can be any point.
	If it is the point of concurrency, the moment arm is zero, resulting in zero torque for the forces acting through this point.
		If it is not the point of concurrency, the moment arm is non-zero, and forces can create torque.
###### Forces Acting Through the Point of Concurrency:
When all forces intersect at a single point (the point of concurrency), and this point is chosen as the axis of rotation, the moment arm (perpendicular distance) from the point to the line of action of each force is zero.
	Therefore, torque τ at the point of concurrency is zero because τ=F⋅0=0.
###### Static Equilibrium
For concurrent force systems, ensuring static equilibrium involves only checking that the vector sum of all forces equals zero (∑F=0), as there are no moments to consider about the point of concurrency.
#### Other Types of Moments
###### Moment of [[Newton's First Law|Inertia]]
This is another crucial concept in dynamics, describing how the mass of a body is distributed relative to an axis of rotation. The moment of inertia affects the rotational motion of an object but is not a force. It plays a role in the rotational version of Newton's second law, which relates torque, moment of inertia, and angular acceleration.
###### Bending Moment
In structural engineering, a bending moment is the internal reaction induced in a structural element when external forces cause the element to bend. It’s expressed in terms of the force multiplied by the distance to the point of interest along the element, influencing how beams and other structural components are designed to withstand loads.
###### Magnetic Moment
In physics, particularly in electromagnetism, the magnetic moment refers to the magnetic strength and orientation of a magnet or other object that produces a magnetic field. It is a vector quantity determining how a magnetic object will react in a magnetic field.
###### Moment Capacity
The internal property that resists bending caused by an external load

$\large (P) \times (x)$
	Where $P =$ the load.
	$x=$  the distance of the load from a cross-section of the beam.
## Momentum vs Moments
Momentum is a vector quantity, meaning it has both magnitude and direction.
### Linear Momentum
Linear momentum ($p$) of an object is defined as the **product** of its **mass** ($m$) and its **velocity** ($v$). Mathematically, it is expressed as:
	$\large p=mv$
###### Relevance in Non-Concurrent Systems
In systems where forces are not acting at a single point (non-concurrent), the linear momentum of each component or part of the system can vary independently, and the total linear momentum of the system is the vector sum of the linear momenta of all its parts.
	The principle of conservation of momentum states that in an isolated system (no external forces), the total linear momentum remains constant.
###### Relevance in Concurrent Systems
In a concurrent system, where all forces meet at a common point, linear momentum is still a relevant concept. 
	*For instance*, consider objects moving towards each other along the same line, influenced by forces that are aligned (concurrent). 
		The total linear momentum of the system is the vector sum of the individual momenta. 

[[#Law of Conservation of Momentum|Conservation of momentum]] is a key principle here, particularly evident in collision and explosion scenarios where, despite the forces being concurrent, the overall momentum of the system remains constant if no external forces are acting.
### [[Newton's Second Law#Angular Momentum|Angular Momentum]]
Angular momentum ($L$) of an **object about a point** is defined as the **[[Statics Analysis#Cross Product|cross product]]** of the **[[Static Equilibrium#Position Vectors (a fourth method to "find" Resultant Force Vectors)|position vector]]** ($r$) relative to **the point and the linear momentum of the object**:
	$\large L=r×p$
###### Relevance in Non-Concurrent Systems
In non-concurrent systems, forces do not meet at a single point and can create rotational effects about different points or axes. 
	The angular momentum is particularly useful in analyzing these effects. 
		For such a system, the total angular momentum about any point or axis is the vector sum of the angular momenta of all particles or components making up the system. 
			Angular momentum, like linear momentum, is conserved in an isolated system, unless an external torque acts upon it.
  
The similarity in terms stems from their root in Latin ("movēre" means "to move"), but they address different aspects of dynamics. 
	**Momentum** relates to the translation of mass.
		**Momentum** concerns the overall motion of the object moving through space, irrespective of any rotation it may also be undergoing.
	While **moments** relate to the rotation around a point or axis.
		Whereas **Moments or torque** specifically refer to rotational motion about an axis and do not directly impact the translational motion of the center of mass in the way linear momentum does.
Thus, while related to movement, they are not directly related to each other in terms of physical phenomena.
##### Law of Conservation of Momentum
Momentum is conserved in isolated systems, according to the law of conservation of momentum.
The conservation of linear momentum is a fundamental principle that holds in both isolated concurrent and non-concurrent systems. 
	This principle states that **unless external forces act on a system, its total linear momentum remains unchanged over time**. 
		This applies universally across physics, providing a critical tool for analyzing and predicting the behavior of systems under various force conditions.
###### Conservation of [[#Linear Momentum|Linear Momentum]] 
In the absence of external forces, the total linear momentum of a non-concurrent system remains constant.
###### Conservation of [[#Angular Momentum|Angular Momentum]]
In the absence of external torques, the total angular momentum of the system about any point or axis remains constant.
## Components of Moments
### Perpendicular Distance
![[Pasted image 20240524152107.png]]
The moment arm (d) is the perpendicular distance from the point about which the moment is being calculated to the line of action of the force.

![[Pasted image 20240524152119.png]]
If the force is applied at an angle other than 90 degrees to the moment arm, the effective moment arm is $\LARGE d′=d\sin (θ)$, where θ is the angle between the force and the moment arm.
	I.e. That if the force F is applied at an angle $\theta$ != 90, then it will be more difficult to turn the bolt since the moment arm $d' = dsin(\theta)$ will be smaller than d.

![[Pasted image 20240524152129.png]]
lf F is applied along the wrench, its moment arm will be zero since the line of action of F will intersect point 0 (the z axis). 
	As a result. the moment of F about 0 is also zero and no turning can occur.

![[Pasted image 20240524154030.png]]
We can generalize the above discussion and consider the force $\vec{F}$ and Point $O$ that lie in the gray plane. 
	The moment $Mo$ about point $O$, or **about an axis passing through $O$** and **perpendicular** to the plane, is a [[#Vector Moment|vector]] quantity since it has a specified [[#Magnitude of a Moment|magnitude]] and [[#Direction of a Moment|direction]].
### [[#Magnitude of a Moment|Magnitude]] Dependence 
The magnitude of the moment is directly proportional to both the force and the perpendicular distance. 
	A larger force or a longer moment arm results in a greater moment.
### Axis of Rotation
The [[#Point of Application|point of application]] in the context of moments, is referred to as the **axis of rotation**.
	This is the point or axis about which we will determine all the moments.
		I.e. The Axis of Rotation is the axis which the moment is directed along. 
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

###### The moment of a force does not always cause a rotation.
	![[Pasted image 20240525101634.png]]
### Magnitude of a Moment
Is the degree to which the moment will cause angular acceleration in the body it is acting on. 
	It is represented by a scalar (i.e. a single number).
Can be thought of as the "strength" of the twisting force exerted on the body.

The magnitude of a moment, $|\vec{M}|$, is measured in:
	$\begin{equation*} \LARGE |\vec{M}| = F \times d \end{equation*}$
Where $F$ is the force, and $d$ is the [[#Perpendicular Distance|perpendicular distance]] from the [[#Axis of Rotation|axis of rotation]] at point $O$ to the [[Statics Analysis#Line of Action|line of action]] of the force.
##### Why Scale Force by Perpendicular Distance?
For each unit of perpendicular distance from the axis of rotation to the line of action of the force, there the magnitude of the force is applied. 
###### Amplification by Perpendicular Distance
The further away the force is applied from the point or axis of rotation, the greater its ability to cause rotation. 
	This is because a longer lever arm (greater distance $d$) means that the same amount of force can produce a larger turning effect. 
		This principle is observable in everyday tools like wrenches or door handles — longer handles require less force to operate because they have a longer lever arm.

The standard unit of measurement for for the magnitude of moments are Newton-meters ($\begin{equation*} \LARGE N \times m \end{equation*}$), and the standard English unit of measurement is foot-pounds ($\begin{equation*} \LARGE lb \times ft \end{equation*}$).
### Direction of a Moment
The direction of $M_{o}$ is defined by its moment axis, which is perpendicular to the plane that contains the force $F$ and its moment arm $d$. 

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

The right-hand rule is used to establish the sense of direction of $M_{o}$.
	 According to this rule the natural curl of the fingers of the right hand, as they arc drawn towards the palm, represent the tendency for rotation caused by the moment.
		  As this action is performed. the thumb of the right hand will give the directional sense of $M_{o}$ Notice that the moment vector is represented three-dimensionally by a curl around an arrow. 
		  In two dimensions this vector is represented only by the curl.
			   Since in this case the moment will tend to cause a counterclockwise rotation. the moment vector is actually directed out of the page.
### Resultant Moment
![[Pasted image 20240525013735.png]]
For 2D problems, where all the forces lies within the x-y plane, the resultant moment ($M_{R_{o}}$) about point $O$ can be determined by **finding all algebraic sum of the moments caused by all the forces in the system**.

If we remember that as an *axis*, the **axis of rotation** (along which the moments are directed) has both a positive and negative direction, then:
	As a convention **counterclockwise** moments are considered to be **positive moments**, "away from the plane".
		**Clockwise** moments are considered to be **negative moments**, "approaching the plane".
			Therefore, each moment can be represented by a **plus** or **minus** sign. 
## Calculating Moments
To calculate the moment that a force exerts on a body, two methods can be used.
### [[Static Equilibrium#Scalar Form Analysis|Scalar Methods]]
##### I.e. Scalar Formulation *of* the Scalar Moment 
###### Scalar Formulation
Refers to the method used to calculate the moment using scalar quantities. 
	In this formulation, the moment M is determined by multiplying the magnitude of the force F by the perpendicular distance d from the point of interest to the line of action of the force.
###### Scalar Moment
This is the **result** of this scalar formulation is a scalar moment, which is a single numerical value representing the magnitude of the turning effect of the force.
	This scalar moment does not include directional information about the axis of rotation but simply provides the magnitude of the moment.

The (scalar) moment (M) is calculated as the product of the force (F) and the perpendicular distance (d) from the line of action of the force to the point of rotation.
	This can be expressed as:
	    $\large M=F⋅d$
    Here, M is the scalar moment, F is the magnitude of the force, and d is the perpendicular distance (moment arm).

The term "moment" is referred to as a scalar formulation because it simplifies the concept into a single numerical value that represents the turning effect of a force about a point.
###### Scalar Moment Contextual Applications
Used in contexts where only the magnitude of the moment is needed, such as in basic statics problems involving two-dimensional structures (e.g., levers, beams). 
	This simplifies calculations and is sufficient for many practical applications.


Scalar methods often require the resolution of forces into perpendicular components, especially in 2D equilibrium problems. 

Here, the Law of Cosines and Law of Sines can be used to find these components when the geometry of the system forms a triangle. 
	*For example*, if a force acts at an angle to a beam, these laws help determine the horizontal and vertical components of this force, which are crucial for checking whether the sum of the forces in any direction (horizontal and vertical) equals zero, as required for static equilibrium.
### [[Static Equilibrium#Vector Form Analysis (i.e. Cartesian Vectors)|Vector Methods]]
##### I.e. Vector Formulation and Vector Moment
###### Vector Formulation
In contrast, the vector formulation involves calculating the moment as a vector quantity using the [[Statics Analysis#Cross Product|cross product]] of the [[Static Equilibrium#Position Vectors (a fourth method to "find" Resultant Force Vectors)|position vector]]r (from the point of rotation to the point where the force is applied) and the force vector F.
    $\LARGE M=r×F$
###### Vector Moment
The result is a vector moment, which includes both the magnitude and direction of the moment. The direction indicates the axis of rotation and follows the right-hand rule, providing a complete description of the rotational effect.
###### Vector Moment Contextual Applications
Necessary in contexts where the direction of the moment is important, such as in three-dimensional problems, complex machinery, and dynamics. 
	The vector moment provides a comprehensive description, including both magnitude and direction.

When calculating moments using vector methods, forces are often decomposed into components along orthogonal axes. 

If the force's line of action and the moment arm form a triangle with the axis of rotation, trigonometric laws can help determine the angle between the force and lever arm.
	Which is crucial for calculating the perpendicular component (lever arm) necessary for $M=r×F$.
