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
	Where the vector is scaled according to its magnitude, in a given direction.
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
### Converting Between Vector and Scalar Forms
Because the two different forms of the vector are equivalent, we can switch between 
representations without changing the problem. 
	Often in engineering problems, it will initially be easier to write the force in magnitude and angle form, but later, analysis will be easier if forces are written in component form.
 
To switch from magnitude and direction form to component form you will use right triangles and trigonometry to determine the component of the overall magnitude in each direction. 
	This is a simple vector decomposition.
	To switch back from component form into magnitude and direction form you simply use the reverse of this initial process.
## Evaluating Magnitudes and Orientations of Force Vectors
### General Steps
![[Pasted image 20240506124701.png]]
1. **Decompose** each force into $x, y, z$ components (i.e. [[#Vector Form Analysis (i.e. Cartesian Vectors)|vector form]]).
2. **Sum $x$ components** to identify resultant $\LARGE F_x$.
3. **Sum $y$ components** to identify resultant $\LARGE F_y$.
4. **Sum $z$ components** to identify resultant $\LARGE F_z$.
5. The Resultant Force vector is then: $\LARGE F_R = \sum \vec{F} = \sum \vec{F_x} + \sum \vec{F_y} + \sum \vec{F_z}$ 
### Trigonometric Tools for Decomposition of Force Vectors 
Trigonometry is essential for breaking down the forces into their x and y components when they're acting at an angle. 
#### Creating Right Triangles
![[Pasted image 20240506130756.png]] ![[Pasted image 20240506130747.png]]
Create a $90 \degree$ triangle using the two component vectors ($\LARGE \vec{F_x}, \vec{F_y}$) and the Force Vector.
	And if needed for a 3D force, another $90 \degree$ triangle using two the $\LARGE \vec{F_z}$ component vector, the $\LARGE \vec{F'}$ component vector and the Force Vector.  

These Right Triangles enable the ability to utilize $\cos(\theta)$ and $sin(\theta)$ functions to find the magnitude of the Force Vector and its component vectors, as well as the orientation of the Force Vector.
	Just consider whether the component ($x, y, z$) is opposite or adjacent from the angle of the force (within the right triangle).

Remember that the component (i.e. standard unit vectors) are the "sliding" in that they are some scaled, linear combination that produces the resultant/force vector. 
	Therefore, to obtain the component "side opposite" of the triangle (i.e. the 3rd "side") of the right triangle, "slide" (where the slide expresses a scaling of the component vectors) to position the component vector between and opposite the angle under study.
#### Tools for Non-Right Triangles
###### Law of Cosines
Used when the component $90 \degree$ triangle is not constructed.
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
#### 2D Decomposition
###### Magnitude of Resultant Force
![[Pasted image 20240506124550.png]]
###### Orientation of Resultant Force
![[Pasted image 20240506124756.png]]
###### Magnitudes of Component Vectors 
For a force vector at an angle $\LARGE \theta$ from the vertical, the trigonometric functions ($sin$) and ($cos$) are used to find the magnitudes of the components:
	Remember: Just consider whether the component ($x, y, z$) is **opposite** or **adjacent** from the angle of the force (within the right triangle).
###### $\LARGE x$ Component ("horizontal") Vector of the Force Vector
Is found by multiplying the force's magnitude by the sine of the angle: 
- When the $x$ component is **opposite** $\theta$: 
	$\LARGE F⋅sin(\theta)$
###### $\LARGE y$ Component ("vertical") Vector of the Force Vector
Is found by multiplying the force's magnitude by the cosine of the angle:
- When the $y$ component is **adjacent** $\theta$.
	$\LARGE F⋅cos(\theta)$
##### 3D Decomposition 
Utilizes $\LARGE A'$ to find force components in the $x$ and $y$ plane. 
![[Pasted image 20240506124911.png]]
###### Normalizing Vectors (i.e. unit vectors)
![[Pasted image 20240506125205.png]]
Creates a "unit vector" (not the same as a "standard unit vector"/"standard basis vector") in the same direction, with a **norm** = 1.
###### Unit Vector 
Not the same as a "standard unit vector"/"standard basis vector".
Refers to a vector with a norm = 1. 
###### Norm of a Vector
The **magnitude** or "length" of a vector from head to tail of vector.
###### To Find the Angles between the $x, y, z$ Axes Relative to the Force Vector
Measured from the **positive** $x, y, z$ axes:
![[Pasted image 20240506125710.png]]
![[Pasted image 20240506133202.png]]
###### Transverse Angle $\Theta$
The angle between the $\LARGE x, y$ plane and the Force Vector.
###### Azimuth Angle $\Phi$ 
The angle between the $\LARGE z$ axis and the Force Vector.
![[Pasted image 20240506125924.png]]
###### Magnitudes of Component Vectors 
For a force vector at an angle $\LARGE \theta$ from the vertical, the trigonometric functions ($sin$) and ($cos$) are used to find the magnitudes of the components:
![[Pasted image 20240506133208.png]]

