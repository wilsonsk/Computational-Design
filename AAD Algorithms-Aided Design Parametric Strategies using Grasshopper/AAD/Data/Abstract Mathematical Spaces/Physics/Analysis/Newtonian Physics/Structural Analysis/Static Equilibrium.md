# Static Equilibrium
Engineering statics is the study of objects in static equilibrium, and the simple assumption of all [[Structural Analysis#Forces|forces]] adding up to zero is the basis for the subject area of engineering statics.

Static Equilibrium implies that a body is in both Translational Equilibrium and Rotational Equilibrium.
	Meaning that the net external force is zero and that the net external moment about any point is also zero.
		It's the principle of superposition that allows this vector addition to work: the effect of the individual forces can be added together to get the total effect. 
### [[Newton's Second Law|Newton's Second Law]]
States that the force exerted on an object is equal to the mass of the object times the [[Newton's Second Law#Acceleration|acceleration]] it experiences. 
	Therefore, if we know that the acceleration of an object is equal to zero, then we can assume that the sum of all forces acting on the object is zero. 
	
Individual forces acting on the object, represented by [[Structural Analysis#Vector|force vectors]], may not have zero magnitude but the sum of all the force vectors will always be equal to zero for objects in equilibrium. 
## [[Concurrent Systems|Translational Equilibrium]]
Translational equilibrium is focused entirely on the linear aspects of motion, not addressing any rotational dynamics that might be present.

Translational equilibrium specifically refers to the condition where the sum of all external forces acting on a body is zero, indicating no net force. 
	This implies that there is no net linear acceleration, meaning the body is either stationary or moving with a constant velocity (not changing speed or direction). 

$\begin{equation*} \LARGE \sum \vec{F} = m \times \vec{a} \end{equation*}$

Where $\LARGE a = 0 ; \sum{\vec{F}} = 0$

Objects in static equilibrium are objects that are not accelerating (either linear acceleration or angular acceleration).
	These objects may be stationary, such as a building or a bridge, or they may have a constant velocity, such as a car or truck moving at a constant speed on a straight patch of road.

## [[Non-Concurrent Systems|Rotational Equilibrium]]
Rotational equilibrium occurs when the net external torque (or moment) acting on a body about any axis is zero. 
	This condition means that there is no net angular acceleration, and as a result, the object either remains stationary in terms of rotation or rotates with a constant angular velocity.

$\begin{equation*} \LARGE \sum{\vec{M}} = I \times \vec{a} \end{equation*}$
Where $\LARGE a = 0 ; \sum{\vec{M}} = 0$
###### [[Newton's Second Law#Angular Acceleration|Angular Acceleration]]
Equilibrium follows a similar pattern for angular accelerations. 
	The [[Newton's Second Law#Rotational Motion|rotational equivalent of Newton's Second Law]] states that the moment exerted on an object is equal to the moment of inertia of that object times the angular acceleration of the object.
		 If we know the angular acceleration of an object is equal to zero, then we know the sum of all moments acting on the object is equal to zero.

## Forms of Forces - Methods of Analyzing Physical Quantities
### Scalar Form Analysis
I.e. Magnitude and Direction Form.
Overall magnitude and angle(s) to indicate direction.
##### 2Dimensional
![[Pasted image 20240503162507.png]]
##### 3Dimensional
![[Pasted image 20240503162807.png]]
###### Force Representation
Forces are represented by their magnitudes and the angles they make with reference axes.
	The direction is considered using angles, and forces are typically discussed in terms of horizontal and vertical components.
###### Decomposing Forces
Forces are broken down into horizontal and vertical components using trigonometry:
- Horizontal Component $\LARGE Fx​=Fcos(θ)$
- Vertical Component $\LARGE Fy​=Fsin(θ)$
###### Summing Components
Components are summed algebraically:
- $\LARGE ∑Fx$​ for all horizontal components
- $\LARGE ∑Fy$​ for all vertical components
- Check for equilibrium: $\LARGE ∑Fx​=0$ and $\LARGE ∑Fy​=0$
###### Application in Statics
Mainly used for checking translational equilibrium.
Suitable for straightforward problems where forces are primarily aligned with or against reference axes.
###### Limitations:
Does not inherently handle moments or rotational forces unless explicitly calculated through additional steps.
### Vector Form Analysis (i.e. Cartesian Vectors)
I.e. Component Form.
Magnitudes in each of the coordinate directions.
##### 2Dimensional
![[Pasted image 20240503162606.png]]
##### 3Dimensional
![[Pasted image 20240503162812.png]]
###### Force Representation
Forces are represented as vectors, $\LARGE \vec{F}=\vec{F_{x}​i}+\vec{F_{y}​j}+\vec{F_{z}​k}$.
- Each component is associated with a unit vector, emphasizing both magnitude and direction.
###### Decomposing Forces
Forces are decomposed into components based on their direction in three-dimensional space:
- $\LARGE \vec{F_{x}}​=\vec{F}cos(θ)$
- $\LARGE \vec{F_{y}}​=\vec{F}sin(θ)$
- $\LARGE Fz$​ (if applicable, based on additional angular measurements)
###### Summing Components
Vector addition is used to sum components:
- $\LARGE \sum\vec{F}=(∑\vec{F_{x}}​)i+(∑\vec{F_{y}}​)j+(∑\vec{F_{z}}​)k$
- Check for equilibrium: $\LARGE ∑F=0$ (meaning zero in all vector components)
###### Application in Statics
- Used for both translational and rotational equilibrium.
- Essential for complex problems involving three-dimensional force interactions and when calculating moments using cross products.
###### Advantages
- Provides a comprehensive approach by incorporating the directional nature of forces and enabling moment calculations directly through vector operations.
### Trigonometric Tools
Trigonometry is essential for breaking down the forces into their x and y components when they're acting at an angle. 
	For a force vector at an angle β from the vertical, the trigonometric functions ($sin$) and ($cos$) are used to find the magnitudes of the components:
		- The x-component (horizontal) of the force is found by multiplying the force's magnitude by the sine of the angle: $F⋅sin(β)$.
		- The y-component (vertical) of the force is found by multiplying the force's magnitude by the cosine of the angle: $F⋅cos(β)$.
###### Law of Cosines
Relates magnitudes to cosines of their corresponding angles.
Used to find magnitudes and angles of non-right triangles.

$\LARGE c = \sqrt{a^2 + b^2 -2 a b cos \gamma}$

This is useful for finding unknown side lengths (i.e. magnitudes) or angles in problems where three forces are acting at various angles to each other, and their magnitudes are known.

![[Pasted image 20240504091250.png]]
###### Law of Sines
Proportion used to relate magnitudes to the sines of the corresponding angles.

$\LARGE a = b {sin \alpha \over sin \beta} == {sin A \over a} = {sin B \over b} = {sin C \over c}$

It is useful when the problem involves two sides (i.e. magnitudes) and an angle between them (or vice versa), providing a way to find unknown angles or sides when resolving forces into their components.

![[Pasted image 20240504091311.png]]

This breakdown allows you to add up all the horizontal components separately from all the vertical components, which is exactly what you do when you're solving for equilibrium.
	When the sum of the x-components and the sum of the y-components both equal zero, the object is in a state of equilibrium—it won't accelerate in any direction because the net force acting on it is zero.
### Converting Between Vector and Scalar Forms
Because the two different forms of the vector are equivalent, we can switch between representations without changing the problem. 
	Often in engineering problems, it will initially be easier to write the force in magnitude and angle form, but later, analysis will be easier if forces are written in component form.
 
To switch from magnitude and direction form to component form you will use right triangles and trigonometry to determine the component of the overall magnitude in each direction. 
	This is a simple vector decomposition.
	To switch back from component form into magnitude and direction form you simply use the reverse of this initial process.
