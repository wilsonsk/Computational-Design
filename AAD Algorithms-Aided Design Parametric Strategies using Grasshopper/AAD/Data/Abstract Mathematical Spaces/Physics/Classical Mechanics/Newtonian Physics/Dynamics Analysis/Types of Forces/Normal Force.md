# Normal Force
This is the force exerted by the ground on the object. It acts upward, perpendicular to the surface, and is denoted as $\LARGE F_{\text{normal}}​$.
	*Note: The [[Data/Abstract Mathematical Spaces/Physics/Analysis/Multivariable Calculus/Gradients|gradient]] of a [[Mapping#Scalar Functions as a Subset of Functions|scalar function]] (such as a [[Potentials#Potential Function, $U(r)$|potential energy function]] or a surface defined by an equation) is indeed used to identify the [[Data/Abstract Mathematical Spaces/Physics/Analysis/Multivariable Calculus/Partial Derivatives#Normal Vector to a 3D Surface|normal direction to a surface]] in 3D.*

![[Pasted image 20240806125122.png]] ![[Pasted image 20240806125514.png]]
## Reaction Force (I.e. the Normal Force)
This object appears to have an acceleration due to the fact of its weight as the acceleration of gravity, and no velocity because an object cannot move thru this "ground" object.
	But, based on the [[Newton's Third Law|Newton's Third Law of Motion]], then the "ground object" is exerting its own force in the **opposite direction** and with the inverse magnitude.
		So both forces equate to 0 in equilibrium. 

The object exerts a downward force on the ground due to gravity, and the ground exerts an equal and opposite upward force on the object. 
	This upward force is the Normal Force.
		This Normal Force is perpendicular to the surface of the object exerting a reactionary force. 
##### [[Static Equilibrium|Static Equilibrium]]
When the object is at rest on the ground, it is in a state of static equilibrium, meaning there is no net force acting on it, and therefore, it has no acceleration.
	According to Newton's first law (an object at rest remains at rest unless acted upon by a net external force), the forces must balance each other out: 
$$\LARGE F_{\text{normal}} = F_{\text{gravity}}$$
$$\LARGE \text{Where } F_{\text{gravity}} = m \cdot g$$
		When the object is at rest on the ground, the net force acting on it is zero because the normal force exactly balances the gravitational force.
			And the Forces are parallel to each other.
				With no net force, there is no acceleration. 
					This means that the object remains at rest (its velocity is zero).
## Forces of an Inclined Plane
![[Pasted image 20240806132046.png]]
*Imagine a completely friction free object and surface of inclined plane*.
The Force of the Object still works downward in the direction of the acceleration of this object due to gravity. 
	But the [[Newton's Third Law#Action and Reaction Forces]] are no longer parallel to each other. 
#### Normal Force of the Inclined Plane
And there is still a reaction force in the normal orientation of the inclined plane.
	The reaction force exerted by the inclined plane, perpendicular to its surface. 

This force arises from the contact interaction between the object and the inclined plane. It is the plane's response or reaction to the object's perpendicular gravitational force component.
	It is a reactive force provided by the surface to prevent the object from penetrating the plane. 
		It adjusts to balance the perpendicular component of the gravitational force when the object is in equilibrium.
			Does not need to be decomposed since it is already aligned with one of the primary directions we are considering.
##### Normal Force Decomposed into Cartesian coordinates ($\hat{i}$ for the horizontal and $\hat{j}$​ for the vertical)
We use the angle $\alpha$ of the inclined plane.
($\vec{F}_N$​) into x and y components
	The normal force $\vec{F}_N$ makes an angle $\alpha$ with the vertical axis (which is perpendicular to the inclined plane).
###### Magnitude of Normal Force
$$\LARGE F_N = mg \cos(\alpha)$$
###### x-component ($F_{N,x}$​)
$$\LARGE F_{N,x} = F_N \sin(\alpha) = (mg \cos(\alpha)) \sin(\alpha)$$
###### y-component ($F_{N,y}$​)
$$\LARGE F_{N,y} = F_N \cos(\alpha) = (mg \cos(\alpha)) \cos(\alpha) = mg\cos^2(\alpha)$$
###### Vector Form of Normal Force
$$\vec{F_N} = F_{n,x}\hat{i} + F_N \cos(\alpha)\hat{j} = (mg \cos(\alpha)) \sin(\alpha)\hat{t} + (mg \cos(\alpha)) \cos(\alpha) = mg\cos^2(\alpha)$$
###### In Equilibrium
$$\LARGE \text{If } F_N = F_{G,\perp} = mg \cos(\alpha)\text{ and } F_{G, \perp} = mg\cos(\alpha)$$
$$\LARGE \text{Then } F_{\text{net, }\perp} = F_{N} - F_{G,\perp} = 0$$
### [[Static Equilibrium#Decomposing Forces|Decomposing]] the Gravitational Force of the Object (i.e. its weight) 
Forces are broken down into horizontal and vertical components using trigonometry:
###### Horizontal Component $\LARGE \vec{F_x​}=\vec{F}cos(\alpha)$
###### Vertical Component $\LARGE \vec{Fy}​=\vec{F}sin(\alpha)$

But to understand the motion of the object on the inclined plane, we decompose the gravitational force into two components.
	Note that 'G' stands for "Force of object" (as the weight of the object due to gravity).
$$\LARGE \vec{F_G} = 0\hat{i} + - mg\hat{j}$$
$$\LARGE F_{\text{G}} = F_{G,\perp}\cos(\alpha) + F_{G,\parallel}\sin(\alpha)$$
#### Perpendicular Component of the Gravitational Force, $F_{\perp}$
This force arises from the object's weight due to gravity and is a part of the overall gravitational force acting on the object.
	It is a component of a single force (gravity) and is part of the gravitational pull acting on the object.

###### Direction
Perpendicular to the plane, pointing into the plane.
	This force acts perpendicular to the surface of the inclined plane.
		It is the reaction force exerted by the plane on the object.

This Force has the same magnitude as the Normal Force of the inclined plane, but is oriented in the opposite direction. 
###### Magnitude
$$\LARGE F_{\perp} = F_{\text{gravity}} \cos(\alpha) = m \cdot g \cos(\alpha)$$
#### Parallel Component of the Gravitational Force, $F_{\parallel}$ 
This component is parallel to the inclined plane and is responsible for the object potentially sliding down the plane.
###### Direction
Parallel to the plane, pointing down the plane.
	This component is parallel to the surface of the inclined plane.
		This component causes the object to potentially slide down the plane.

Is parallel to the surface of the inclined plane, and is the result of vector addition of the $F_N$ and $F_G$.
###### Magnitude
$$\LARGE F_{\parallel} = F_{\text{gravity}}\sin(\alpha) = m\cdot g \sin(\alpha)$$
#### Calculating the Resultant Force, $F_R$ aka $F_{\text{net}}$ (Assuming No Friction)
$$\LARGE \sum F = F_{\text{net}} = m \cdot g$$
To find the resultant force, we sum the forces in both the parallel and perpendicular directions. 
	However, since the normal force and the perpendicular component of the gravitational force balance each other out, the resultant force primarily concerns the parallel component.
		The direction of the resultant force is along the plane, dictated by the parallel component of the gravitational force and any opposing frictional force.
##### Resultant Force
$$\LARGE F_{\text{net},\parallel} = F_{G,\parallel} $$
#### From the Resultant Force [[Integrals#Power Rule for Integration|Integrating]] from Acceleration, $F_R$ aka $F_{\text{net}}$
To obtain the Velocity and then the Position. 
$$\LARGE F_{\parallel} = F_{\text{gravity}}\sin(\alpha) = m\cdot g \sin(\alpha)e_s$$
Where $e_s$ indicates the direction (in standard unit vectors) along the plane.
	And $s$ specifically is a position.
		And $\LARGE \ddot{s}$ is the acceleration (i.e. gravity).
$$\LARGE m \ddot{s} = mg \sin(\alpha)$$
$$\LARGE \ddot{s} = a_{s} = g \sin(\alpha)$$
$$\LARGE \dot{s} = v_s = g\sin(\alpha) t + v_0$$
$$\LARGE s(t) = \frac{1}{2}g\sin(\alpha)t^2 + v_0t + s_0$$
### Example: Calculating the Resultant [[Data/Abstract Mathematical Spaces/Physics/Classical Mechanics/Newtonian Physics/Statics Analysis/Static Equilibrium#Evaluating Magnitudes and Orientations of Force Vectors]]
If no angle is given, we can still calculate the resultant force if we know the components of the forces acting on the object in the Cartesian coordinate system (i.e., $\hat{i}$ and $\hat{j}$ directions). 

Suppose we have an object of mass $m$ on an inclined plane, and we know the following:
- The gravitational force ($\vec{F}_G$) acts vertically downward with magnitude $mg$.
- The normal force ($\vec{F}_N$) is perpendicular to the inclined plane.

We will decompose these forces into their Cartesian components and then calculate the resultant force.
#### Given Data
- Mass of the object: $m = 10 \, \text{kg}$
- Gravitational acceleration: $g = 9.8 \, \text{m/s}^2$
- Gravitational force: $\vec{F}_G = -mg \hat{j} = -10 \times 9.8 \hat{j} = -98 \hat{j} \, \text{N}$
- Normal force components: Suppose we know that $F_{N,x} = 30 \, \text{N}$ and $F_{N,y} = 84.87 \, \text{N}$ (we can use these values if they were given or derived from additional context).
#### Decomposing the Forces

1. **Gravitational Force**: - In Cartesian coordinates: $$ \vec{F}_G = 0 \hat{i} - 98 \hat{j} \, \text{N} $$ 2. **Normal Force**: - Components in Cartesian coordinates: $$ \vec{F}_N = F_{N,x} \hat{i} + F_{N,y} \hat{j} = 30 \hat{i} + 84.87 \hat{j} \, \text{N} $$
#### Summing the Forces
1. **x-component of the resultant force**: $$ F_{\text{net},x} = F_{G,x} + F_{N,x} = 0 + 30 = 30 \, \text{N} $$ 2. **y-component of the resultant force**: $$ F_{\text{net},y} = F_{G,y} + F_{N,y} = -98 + 84.87 = -13.13 \, \text{N} $$
#### Resultant Force Magnitude 
The magnitude of the resultant force is given by: $$ F_{\text{net}} = \sqrt{(F_{\text{net},x})^2 + (F_{\text{net},y})^2} $$ $$ F_{\text{net}} = \sqrt{(30)^2 + (-13.13)^2} $$ $$ F_{\text{net}} = \sqrt{900 + 172.40} $$ $$ F_{\text{net}} = \sqrt{1072.40} $$ $$ F_{\text{net}} \approx 32.74 \, \text{N} $$
#### Resultant Force Direction 
The direction of the resultant force can be found using the angle $\theta$ it makes with the horizontal axis ($\hat{i}$): $$ \tan(\theta) = \frac{F_{\text{net},y}}{F_{\text{net},x}} $$ $$ \tan(\theta) = \frac{-13.13}{30} $$ $$ \theta = \tan^{-1}\left(\frac{-13.13}{30}\right) $$ $$ \theta \approx -23.56^\circ $$
This angle indicates that the resultant force is directed downwards and to the right, with an angle of about $-23.56^\circ$ with respect to the horizontal axis.
