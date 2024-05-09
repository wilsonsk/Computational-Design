# Static Equilibrium
Engineering statics is the study of objects in static equilibrium, and the simple assumption of all [[Structural Analysis#Forces|forces]] adding up to zero is the basis for the subject area of engineering statics.

Static Equilibrium implies that a body is in both Translational Equilibrium and Rotational Equilibrium.
	Meaning that the net external force is zero and that the net external moment about any point is also zero.
		It's the principle of superposition that allows this vector addition to work: the effect of the individual forces can be added together to get the total effect. 
### [[Newton's Second Law|Newton's Second Law]]
States that the force exerted on an object is equal to the mass of the object times the [[Newton's Second Law#Acceleration|acceleration]] it experiences. 
#### Therefore, if we know that the acceleration of an object is equal to zero, then we can assume that the sum of all forces acting on the object is zero. 
	
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
- Horizontal Component $\LARGE \vec{F_x​}=\vec{F}cos(θ)$
- Vertical Component $\LARGE \vec{Fy}​=\vec{F}sin(θ)$
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
 
To switch from magnitude and direction form to component form you will use [[#Creating Right Triangles|right triangles]] and [[#Trigonometric Tools for Decomposition of Force Vectors|trigonometry]]to determine the component of the overall magnitude in each direction. 
	This is a simple vector decomposition.
	To switch back from component form into magnitude and direction form you simply use the reverse of this initial process.
#### 2D Converting Magnitude and Direction to Component Form
![[Pasted image 20240508145141.png]]
To go from a magnitude and direction (i.e. scalar form) to component form (i.e. vector form), we will first draw a right triangle with the hypotenuse being the original vector. 
	The horizontal arm of the triangle will then be the 𝑥-component of the vector while the vertical arm is the 𝑦 component of the vector. 
		If we know the angle of the vector with respect to either the horizontal or the vertical, we can use the sine and cosine relationship to find the 𝑥 and 𝑦 components.
####  2D Converting Component Form to Magnitude and Direction
![[Pasted image 20240508145321.png]]
To find the magnitude and the direction of a vector using components, we will use the same process in reverse.
	We will draw the components as the legs of a right triangle, where the hypotenuse of the triangle shows the magnitude and direction of the vector.

To find the magnitude of the vector we will use the Pythagorean Theorem, taking the square root of the sum of the squares of each component. 
	To find the angle, we can easily use the inverse tangent function, relating the opposite and adjacent legs of our right triangle.
#### Converting Between Vector Representations in 3D
![[Pasted image 20240508145439.png|400]]
In three dimensions, we will have either three components (𝑥, 𝑦, and 𝑧) for component form or a magnitude and two angles for the direction in magnitude and direction form. 

To convert between forms we will need to draw in two sets of right triangles. 
The hypotenuse of the first triangle will be the original vector and one of the legs will be one of the three components. 
	The other leg will then be the hypotenuse of the second triangle. 
		The legs of this second triangle will then be the remaining two components. 
			Use sine and cosine relationships to find the magnitude of each component along the way. 

This general process of two consecutive right triangles will always hold true, but depending on angles that are given or chosen which components end up being which leg can vary. 

Carefully plotting everything out in a diagram is important for this reason.
## Evaluating Magnitudes and Orientations of Force Vectors
### General Steps
![[Pasted image 20240506124701.png]]
1. **Decompose** each force into $x, y, z$ components (i.e. [[#Vector Form Analysis (i.e. Cartesian Vectors)|vector form]]).
	- If [[#[3D Decomposition](https //www.udemy.com/course/engineering-mechanics-statics/learn/lecture/41715220 overview)|3D Decomposition]], then can use the 
2. **Sum $x$ components** to identify resultant $\LARGE F_x$.
3. **Sum $y$ components** to identify resultant $\LARGE F_y$.
4. **Sum $z$ components** to identify resultant $\LARGE F_z$.
5. The Resultant Force vector is then: $\LARGE F_R = \sum \vec{F} = \sum \vec{F_x} + \sum \vec{F_y} + \sum \vec{F_z}$ 
6. The Force Angle and Magnitude is found using the Resultant Force Vector.
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
##### 2D Pythagorean Theorem
Can be used for Right Triangles.
![[Pasted image 20240508141253.png]]
$\large c^2 = a^2 + b^2$
##### 3D Pythagorean Theorem
Can be used for Right Triangles.
![[Pasted image 20240508141235.png]]
$\large d^2 = a^2 + b^2 + c^2$
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
###### Magnitude of 2D Resultant Force
![[Pasted image 20240506124550.png]]
###### Orientation of 2D Resultant Force
![[Pasted image 20240506124756.png]]
###### Magnitudes of 2D Component Vectors 
For a force vector at an angle $\LARGE \theta$ from the vertical, the trigonometric functions ($sin$) and ($cos$) are used to find the magnitudes of the components:
	Remember: Just consider whether the component ($\LARGE \vec{F_x}, \vec{F_y}, \vec{F_z}$) is **opposite** or **adjacent** from the angle of the force (within the right triangle).
###### $\LARGE |\vec{F_x}|$ Component ("horizontal") Vector of the 2D Force Vector
Is found by multiplying the force's magnitude by the sine of the angle: 
- When the $x$ component is **opposite** $\theta$: 
	$\LARGE sin(\theta) = {|\vec{F_x \space component}| \over |\vec{F}|} == |\vec{F}|⋅sin(\theta) = |\vec{F_x \space component}|$
###### $\LARGE |\vec{F_y}|$ Component ("vertical") Vector of the 2D Force Vector
Is found by multiplying the force's magnitude by the cosine of the angle:
- When the $y$ component is **adjacent** $\theta$.
	$\LARGE cos(\theta) = {|\vec{F_y \space component}| \over |\vec{F}|} == |\vec{F}|⋅sin(\theta) = |\vec{F_y \space component}|$
###### Magnitude of 2D Resultant Vector
Is the just the summing of like component vectors once discerned via trigonometry using angles and resultant prime vector.
#### [3D Decomposition](https://www.udemy.com/course/engineering-mechanics-statics/learn/lecture/41715220#overview) 

##### Normalizing Vectors (i.e. unit vectors)
![[Pasted image 20240506125205.png]]
Creates a "unit vector" (not the same as a "standard unit vector"/"standard basis vector") in the same direction, with a **norm** = 1.
###### Unit Vector 
Not the same as a "standard unit vector"/"standard basis vector".
Refers to a vector with a norm = 1. 
$\LARGE \vec{\hat{U}_F} = {\vec{F} \over |\vec{F}|} = {\vec{F_{x}\hat{i}}+\vec{F_{y}\hat{j}}+\vec{F_{z}\hat{k}}\over \sqrt{\vec{F_{x}}\hat{i}^2+\vec{F_{y}}\hat{j}^2+\vec{F_{z}}\hat{k}^2}} == \vec{F}= |\vec{F}|\vec{\hat{U}_F}$
###### Norm of a Vector
$\LARGE |\vec{someVector}|$
The **magnitude** or "length" of a vector from head to tail of vector.
##### To Find the Angles between the $x, y, z$ Axes Relative to the 3D Force Vector
And therefore, find the Resultant Force Vector (i.e. its component vectors, its magnitude and its orientation).
###### Utilizes $\LARGE A'$ 
To find force component vectors using the [[#Transverse Angle $ Theta$|Transverse Angle]] (in the $x$ and $y$ plane) method or the [[#Coordinate Direction Angles|Coordinate Direction Angles]]. 
![[Pasted image 20240506124911.png]]

These angles can then be used to find the magnitudes and orientations of the 3D component vectors.
###### Magnitudes of 3D Component Vectors 
Utilizing the angles produced via [[#Azimuth Angle $ Phi$|Azimuth]], [[#Transverse Angle $ Theta$|Transverse]] or [[#Coordinate Direction Angles|Coordinate Direction Angles]], the trigonometric functions ($sin$) and ($cos$) can then be used to find the magnitudes of the component vectors, and thus the vector form also.
![[Pasted image 20240506133208.png]]
###### Coordinate Direction Angles
Measured from the **positive** $x, y, z$ axes.
The 3D Force Vector will always be **adjacent** to the Coordinate Direction Angle and therefore, obtained via the $cos$ function.
Are used to find the **orientation** of the Resultant Vector.
- $\LARGE \alpha$ = **Positive** angle between the Force Vector and the $\LARGE x$ axis
		$\LARGE |\vec{F_x}| = |\vec{F}| \cos \alpha == \cos \alpha = {|\vec{F_x}| \over |\vec{F}|}$
- $\LARGE \beta$ = **Positive** angle between the Force Vector and the $\LARGE y$ axis.
		$\LARGE |\vec{F_y}| = |\vec{F}| \cos \beta == \cos \beta = {|\vec{F_y}| \over |\vec{F}|}$
- $\LARGE \gamma$ = **Positive** angle between the Force Vector and the $\LARGE z$ axis.
		$\LARGE |\vec{F_z}| = |\vec{F}| \cos \gamma == \cos \gamma = {|\vec{F_z}| \over |\vec{F}|}$
![[Pasted image 20240506125710.png]]
![[Pasted image 20240506133202.png]]
###### Transverse Angle $\Theta$
The angle between the $\LARGE x, y$ plane and the Force Vector.
Are used to find the **orientation** of the Resultant Vector.
###### Azimuth Angle $\Phi$ 
The angle between the $\LARGE z$ axis and the Force Vector.
Are used to find the **orientation** of the Resultant Vector.

![[Pasted image 20240506125924.png]]
###### Magnitude of 3D Resultant Vector
Is the just the summing of like component vectors once discerned via trigonometry using angles and resultant prime vector.
##### [Example of a 3D Force Vector "Problem"](https://www.udemy.com/course/engineering-mechanics-statics/learn/lecture/41715228#overview) (i.e. finding a Resultant Force Vector- its components, magnitude and orientation)
![[Pasted image 20240508140307.png|400]]
Specify the **magnitude** and the **coordinate direction angles** $\alpha_1$, $\beta_1$, and $\gamma_1$ of **$\large F_1$**, so that the Resultant Force Vector of the the three forces action on the bracket is $|\vec{F_R}| = -350k$ lbs.  Note that $\vec{F_3}$ lies in the $x y$ plane.
1. Decompose the force vectors ($\vec{F_1}$, $\vec{F_2}$, $\vec{F_3}$) into vector form. 
	![[Pasted image 20240508140449.png]]
2. Calculate $\large \vec{F_1}$ in vector form using algebra to solve for unknown variables.
	1. Set the sum of the force vectors equal to the magnitude of the Resultant Force Vector, $|\vec{F_R}| = -350k$. 
		![[Pasted image 20240508140719.png]]
3. Calculate the magnitude of $\large |\vec{F_1}|$ using [[#3D Pythagorean Theorem|3D Pythagorean Theorem]].
	![[Pasted image 20240508141408.png]]
4. Calculate the **Coordinate Direction Angles** $\alpha_1$, $\beta_1$, and $\gamma_1$ of **$\large F_1$**
	![[Pasted image 20240508141512.png]]
###### Position Vectors (a fourth method to "find" Resultant Force Vectors)
Refers to a fundamental concept used to describe the location of a point or an object in space relative to a chosen reference point- this chosen reference point is typically chosen to be the "origin of a coordinate system".

A position vector, denoted as $\large r$, is a **vector** that **originates from a fixed reference point** (usually the origin of a coordinate system) and points to the position of an object.
	It describes the displacement of the object from the origin.
		This position vector, itself, has component vectors (i.e. scaled standard unit vectors).

$\large \vec{r} = x\textbf{i} + y\textbf{j} + z\textbf{k}$ 

Where $x, y$ and $z$ are the coordinates of the point (i.e. location) being described/measured in the Cartesian plane.
Where $\textbf{i, j, k}$ are the unit vectors along the $x,y,z$ axes, respectively. 

*Example of a Position Vector from the Origin*
![[Pasted image 20240508143840.png]]
*Example of a Position Vector NOT from the Origin*
![[Pasted image 20240508144123.png|400]]
The position vector that lies "**between**" a point and a reference point that is NOT the origin.
Use head to tail, [[Structural Analysis#Vector Addition|vector addition]].

$\large \vec{r} = x\textbf{i} + y\textbf{j} + z\textbf{k}$ 

$\large \vec{r_A} =\vec{r} + \vec{r_B}$ 
	$\large \vec{r} =\vec{r_B} - \vec{r_A}$ 
		Where $\vec{r_B}$ is the "point r is going to".
		And $\vec{r_A}$ is the "point r is leaving from".
		$\vec{r}$ can then be thought of as $\vec{r_{AB}}$
Therefore:
$\large \vec{r_B} = x_{B}\textbf{i} + y_{B}\textbf{j} + z_{B}\textbf{k}$ 
$\large \vec{r_A} = x_{A}\textbf{i} + y_{A}\textbf{j} + z_{A}\textbf{k}$ 

Position Vector $\large \vec{r}$
	$\large \vec{r} = (x_{B}-x_{A})\textbf{i} + (y_{B}-y_{A})\textbf{j} + (z_{B}-z_{A})\textbf{k}$ 
###### Usage in Mechanics:
- **[[Newtonian Mechanics#Analysis Kinematics Identifying the "Present" (i.e. initial) State State (of condition, Parameters parameters ). Kinematics|Kinematics]]**: Position vectors are used to track the location of objects as they move. Changes in the position vector over time describe the path or trajectory of the object.
- **[[Newtonian Mechanics#Analysis Dynamics "Explains" the Causality of a State Change Dynamics|Dynamics]]**: The derivative of the position vector with respect to time gives the velocity vector, and the second derivative gives the acceleration vector, both of which are crucial for analyzing forces and motion according to Newton’s laws.
###### Finding the Magnitude of a Position Vector
1. Find the **[[#Coordinate Direction Angles|coordinate direction angles]]** of the vectors that the position vector lies between (in this case $\vec{r_A}$ and $\vec{r_B}$)
	![[Pasted image 20240508150001.png]]
2. Find the **magnitude** of the position vector 
	- Using the Pythagorean Theorem
		![[Pasted image 20240508150103.png]]
3. Find the Coordinate Direction Angles
	![[Pasted image 20240508150213.png]]
###### Force Directed Along a Line (i.e. an example of the position vector method)
![[Pasted image 20240508150847.png|200]]
Notice Resultant Force Vector, $\vec{F_{AB}}$ has the same position, and [[Structural Analysis#Sense of a Vector|sense]] as the position vector, $\vec{r}$. 
	Therefore, $\vec{r}$ can be used to find $\vec{F}$.
	
To find the Force Vector, $\vec{F_{AB}}$ of the position vector $\vec{r_{AB}}$:
- Find the unit vector, $\vec{u_{AB}}$, that goes from point $A$ to point $B$.
	- This is done by using position vector, $\vec{r_{AB}}$, that exists between point $A$ to point $B$.

1. Find the Coordinates of Points $A$ and $B$.
2. Find $\vec{F} = F\hat{u}$ (i.e. the component force vectors of the position vectors).
	1. Find $\vec{r}$.
	2. Find [[#Unit Vector|unit vector]], $\hat{u} = {\vec{r} \over r}$.
3. Find the Resultant Force Vectors (component vectors, orientation and magnitude).
###### Example of Force Directed Along a Line
![[Pasted image 20240509125239.png|400]]
1. Find the Coordinates of Points $A$ and $B$
	![[Pasted image 20240509125334.png]]
2. Find $\vec{F} = F\hat{u}$: (i.e. the Component Force Vectors- $\vec{F{_AC}}$ and $\vec{F{_AB}}$) using the position vectors
	1. Find $\vec{r_{AC}}$.
		![[Pasted image 20240509125752.png]]
		![[Pasted image 20240509125811.png]]
	2. Find $\vec{r_{AB}}$.
		![[Pasted image 20240509125828.png]]
		![[Pasted image 20240509125835.png]]
	3. Find [[#Unit Vector|unit vector]], $\large \hat{u_{AC}} = {\vec{r_{AC}} \over r}$
		![[Pasted image 20240509130421.png]]
	4. Find [[#Unit Vector|unit vector]], $\large \hat{u_{AB}} = {\vec{r_{AB}} \over r}$
		![[Pasted image 20240509130432.png]]
	5. Find $\vec{F_{AC}} = F\hat{u_{AC}}$
		![[Pasted image 20240509130655.png]]
	6. Find $\vec{F_{AB}} = F\hat{u_{AB}}$
		![[Pasted image 20240509130703.png]]
	7.  Find Resultant Force Vector (component vectors, orientation and magnitude)
		- Component vectors:
			![[Pasted image 20240509130809.png]]
		- Orientation:
			![[Pasted image 20240509131929.png]]
		- Magnitude:
			![[Pasted image 20240509131312.png]]
			
		