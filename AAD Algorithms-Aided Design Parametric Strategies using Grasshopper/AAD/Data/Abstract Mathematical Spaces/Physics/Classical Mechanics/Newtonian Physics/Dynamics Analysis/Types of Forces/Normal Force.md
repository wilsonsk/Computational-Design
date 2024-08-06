# Normal Force
This is the force exerted by the ground on the object. It acts upward, perpendicular to the surface, and is denoted as $\LARGE F_{\text{normal}}​$.

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
	
When in equilibrium:
$$\LARGE F_N = F_{\perp} = mg \cos(\alpha)$$
### [[Static Equilibrium#Decomposing Forces|Decomposing]] the Gravitational Force 
But to understand the motion of the object on the inclined plane, we decompose the gravitational force into two components.

Forces are broken down into horizontal and vertical components using trigonometry:
###### Horizontal Component $\LARGE \vec{F_x​}=\vec{F}cos(\alpha)$
###### Vertical Component $\LARGE \vec{Fy}​=\vec{F}sin(\alpha)$
#### Perpendicular Component of the Gravitational Force, $F_{\perp}$
This force arises from the object's weight due to gravity and is a part of the overall gravitational force acting on the object.
	It is a component of a single force (gravity) and is part of the gravitational pull acting on the object.

This force acts perpendicular to the surface of the inclined plane.
	It is the reaction force exerted by the plane on the object.

This Force has the same magnitude as the Normal Force of the inclined plane, but is oriented in the opposite direction. 
###### Magnitude
$$\LARGE F_{\perp} = F_{\text{gravity}} \cos(\alpha) = m \cdot g \cos(\alpha)$$
#### Parallel Component of the Gravitational Force, $F_{\parallel}$ (i.e. the Resulting Force)
This component is parallel to the inclined plane and is responsible for the object potentially sliding down the plane.
	This component is parallel to the surface of the inclined plane.
		This component causes the object to potentially slide down the plane.

Is parallel to the surface of the inclined plane, and is the result of vector addition of the $F_N$ and $F_G$.
###### Magnitude
$$\LARGE F_{\parallel} = F_{\text{gravity}}\sin(\alpha) = m\cdot g \sin(\alpha)$$
#### [[Integrals#Power Rule for Integration|Integrating]] from Acceleration 
To obtain the Velocity and then the Position. 
$$\LARGE F_{\parallel} = F_{\text{gravity}}\sin(\alpha) = m\cdot g \sin(\alpha)e_s$$
Where $e_s$ indicates the direction (in standard unit vectors) along the plane.
	And $s$ specifically is a displacement the object has moved along the inclined plane from some initial position.
$$\LARGE m \ddot{s} = mg \sin(\alpha)$$
$$\LARGE \ddot{s} = a_{s} = g \sin(\alpha)$$
$$\LARGE \dot{s} = v_s = g\sin(\alpha) t + v_0$$
$$\LARGE s(t) = \frac{1}{2}g\sin(\alpha)t^2 + v_0t + s_0$$

