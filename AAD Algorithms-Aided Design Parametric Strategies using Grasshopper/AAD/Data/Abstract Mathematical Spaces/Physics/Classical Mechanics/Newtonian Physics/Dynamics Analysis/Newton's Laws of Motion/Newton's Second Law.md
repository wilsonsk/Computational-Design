---
up:
  - "[[Newtonian Mechanics]]"
related:
  - "[[Newton's First Law]]"
  - "[[Statics Analysis]]"
  - "[[Newton's Third Law]]"
date created: 2024-05-03
---
# Newton's Second Law (i.e. Law of Force/Motion/Momentum)
**"The change of motion of an object is [[Division#Proportionality|proportional]] to the force impressed; and is made in the direction of the straight line in which the force is impressed."**
	"When a net force acts on any body with mass, it produces an acceleration of that body. The net force will be equal to the mass of the body times the acceleration of the body."

I.e. The more force you apply to an object, the more it will accelerate.
	If you push harder, it speeds up faster (i.e. accelerates at an increased rate).
		 The acceleration (how quickly the object speeds up) depends on both the amount of force you use and the mass of the object. 
			 This relationship is expressed by the formula: $\LARGE F = ma$
				Where $F$ is the force, $m$ is the mass, and $a$ is the acceleration.
					 This means if you double the force, the acceleration doubles, but if the mass is larger, the same force will cause less acceleration.

![[Pasted image 20240525095708.png]]
## Force
Fundamentally describes how the **velocity** of an object **changes** when it is subjected to external forces.
I.e. Is the analysis of acceleration - i.e. the change of an object's **velocity**. 
	I.e. Change in momentum - which is a static or constant velocity.

$\begin{equation*} \LARGE |\vec{F}| = {d(mv) \over (dt)} == m \times {dv \over dt} == {dp \over dp} == m \times |\vec{a}| \end{equation*}$ 

Where $d$ is "change", $\triangle$, $t$ is time, $v$ is [[#Velocity|velocity]], $p$ is [[#Momentum|momentum]].  

And where Force, $\vec{F}$ and [[#Acceleration|acceleration]], $\vec{a}$ are vector quantities, having both a magnitude and a direction. 
	Mass, $m$, on the other hand, is a scalar quantity having only a magnitude. 
		The mass is scaled by the acceleration - i.e. for each unit within the total mass, there is one "level" of acceleration. 
			Then the sum total of these "levels" of acceleration equal to the force.
			
Based on the equation, it can be inferred that the **magnitude of the net force acting on the body** will be **equal to** the **mass of the body times the magnitude of the acceleration**.
	And that the direction of the net force on the body will be equal to the direction of the acceleration of the body.
		
The more mass an object has, the greater its inertia, and therefore the more it resists changes to its motion.
	The greater the mass, the greater the inertia, and the more force is required to change the object's state of motion.
## Motion
Motion describes the change in position of an object over a time relative to a reference frame, influenced by applied forces. 
### Transformations as Motion (i.e. Representing Motion)
Transformations are the mathematical descriptions or representations of motion.
	They provide a framework to quantify, analyze, and simulate how objects move in space, which is crucial for fields ranging from animation and robotics to engineering and physics.
###### Dynamic vs. Static
It's important to note that while transformations can represent motion, they can also represent static changes—like rotating a stationary object in a design without it needing to be in motion over time. 
	The context ([[Dynamics Analysis|dynamic]] vs. [[Statics Analysis|static]]) dictates how transformations are interpreted.
### Types of Transformations
[[Transformations/Transformations|Transformations]], particularly [[Euclidean Transformations#Translations|translations]] and [[Euclidean Transformations#Rotations|rotations]], can be used to mathematically describe or represent the motion of objects in physics. 
#### [[Euclidean Transformations#Translations|Translation Transformation]]
Can describe an object [[Linear Motion|moving in a straight line]] from one location to another without changing its orientation or speed—akin to translational motion in physics.
###### Application to Force Vectors
A translational transformation of a force vector might involve shifting the point of application of the force along a line of action, without changing the magnitude or direction of the force itself. This is particularly relevant in statics for analyzing how different placements of forces affect the stability of a structure.
###### Application to Bodies
When a body undergoes a translational transformation, it moves from one position to another without any rotation. In physics, this corresponds to the entire body [[Linear Motion|moving linearly]] in space, which can occur under the action of uniform forces.
#### [[Euclidean Transformations#Rotations|Rotational Transformation]]
Corresponds to an object rotating around a fixed axis, similar to rotational motion in physics.
###### Application to [[Statics Analysis#Force Vector Representation|Force Vectors]]
Rotational transformations can be applied to force vectors by changing the direction of the force while keeping its point of application and magnitude constant. This type of transformation is crucial when analyzing scenarios like torques generated by forces not aligned with the axes of rotation.
###### Application to [[Statics Analysis#Bodies|Bodies]]
A rotational transformation involves the body rotating around an axis or point. This transformation is fundamental in dynamics, where the orientation of a body changes due to moments or torques applied to it.
#### Integration in Statics and Dynamics
##### [[Statics Analysis|Statics]]
Even though statics primarily focuses on systems at equilibrium, understanding how translational and rotational transformations affect force vectors and bodies helps in designing systems that maintain equilibrium under various loads. For instance, knowing how to position structural elements to balance forces and moments is key to ensuring stability.
##### Dynamics
Dynamics deals with how bodies respond to forces, often involving motion. Here, translational and rotational transformations describe how objects move under these forces, whether linearly (translational motion) or around an axis (rotational motion).
## Velocity 
**Velocity** is a vector quantity that refers to the **rate of change of an object's position**. 
	It has both magnitude (speed) and direction, which distinguishes it from speed.
		Velocity tells us not only how fast an object is moving but also in which direction it is moving.

Velocity is a ratio.
	Where a specific quantity of [[Kinematics Analysis#Displacement (Δx,Δy,Δz)|displacement]] is associated or paired with a specific quantity of time.
		This is a [[Data/Abstract Mathematical Spaces/Physics/Dimensional Analysis/Measurement#Derived Dimensions|derived dimension]].

$\large v = {\triangle x \over \triangle t}$
	Where $v$ is velocity.
	$\triangle x$ is the change in the object's position (i.e. the displacement of the object) .
	$\triangle t$ is the change in time.

Velocity can be either **constant** or **variable**:
- If an object travels at a constant velocity, it moves in a straight line at a constant speed.
- If the velocity changes, it may do so in terms of magnitude (speed) or direction, or both.
###### Speed
A scalar quantity that does not involve direction. 
## Acceleration  
**Acceleration** is a vector quantity that describes the **rate of change of velocity**.
	It indicates how quickly an object's velocity changes in magnitude (how fast it speeds up or slows down) and direction (how its direction of travel changes) over time. 
		An object accelerates if either its speed or direction (or both) changes.

Acceleration is a ratio.
	I.e. It tells you how much of one thing you have compared to another.

$\large a = {\triangle v \over \triangle t}$
Where $v$ is acceleration.
	$\triangle v$ is the change in the object's [[#Velocity|velocity]].
	$\triangle t$ is the change in time.
	
Acceleration can occur in various contexts:
###### Positive Acceleration
An increase in the magnitude of velocity (speeding up).
###### Negative Acceleration or Deceleration
A decrease in the magnitude of velocity (slowing down).
###### Centripetal Acceleration
A change in the direction of velocity, which occurs when an object moves in a circular path.
## Momentum
Momentum describes the **quantity of motion of a moving object**. 
	Momentum is a vector quantity, which means it has both magnitude and direction. 
		It is closely linked to the mass of the object and its velocity, and it plays a crucial role in the dynamics of moving systems.

Momentum is a scaling. 
### Linear Momentum
Linear momentum ($p$) of an object is defined as the **product** of its **mass** ($m$) and its **velocity** ($v$). 

Mathematically, it is expressed as:
	$\LARGE p=mv$

Where the object's velocity, $v$, is **scaled** by the object's mass, $m$.
	I.e. For 1 unit of mass, the object's velocity is applied. 
## Angular Momentum
Angular momentum ($L$) of an **object about a point** is defined as the **[[Statics Analysis#Cross Product|cross product]]** of the **[[Static Equilibrium#Position Vectors (a fourth method to "find" Resultant Force Vectors)|position vector]]** ($r$) relative to **the point and the linear momentum of the object**:
	$\large L=r×p$
##### Law of Conservation of Momentum
Momentum is conserved in isolated systems, according to the law of conservation of momentum.
The conservation of linear momentum is a fundamental principle that holds in both isolated concurrent and non-concurrent systems. 
	This principle states that **unless external forces act on a system, its total linear momentum remains unchanged over time**. 
		This applies universally across physics, providing a critical tool for analyzing and predicting the behavior of systems under various force conditions.
###### Conservation of [[#Linear Momentum|Linear Momentum]] 
In the absence of external forces, the total linear momentum of a non-concurrent system remains constant.
###### Conservation of [[#Angular Momentum|Angular Momentum]]
In the absence of external torques, the total angular momentum of the system about any point or axis remains constant.
## Angular Velocity
Also known as angular frequency vector, is a pseudovector representation of how the angular position or orientation of an object changes with time.
	I.e. How quickly an object rotates around an axis of rotation and how fast the axis itself changes direction
	
$\large \omega = {\triangle \theta \over \triangle t}$
## Angular Acceleration
Angular acceleration is the rate of change of an object's rotational speed in a clockwise or counterclockwise direction.

$\large \alpha = {\triangle \omega \over \triangle t} = {\omega_{2} - \omega_{1} \over t_{2} - t_{1}}$
## Rotational Motion
Newton's second law also applies to moments and rotational velocities. 
	The revised version of the second law equation states that the **net [[Non-Concurrent Systems#Moments (i.e. Torque)|moment]]**, $\vec{M}$, acting on the object will be equal to the **mass moment of inertia of the body about the axis of rotation, (𝐼)** times the **angular acceleration of the body, $\vec{a}$**.

$\begin{equation*} \LARGE \vec{M} = I \times \vec{a} \end{equation*}$

The moment and the angular acceleration of the body have arrows above them, indicating that they are vector quantities with both a magnitude and direction. 
	The mass moment of inertia, on the other hand, is a scalar quantity having only a magnitude. 
		The magnitude of the net moment will be equal to the mass moment of inertia times the magnitude of the angular acceleration, and the direction of the net moment will be equal to the direction of the angular acceleration.

