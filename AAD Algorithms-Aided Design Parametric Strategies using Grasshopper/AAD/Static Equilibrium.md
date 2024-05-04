# Static Equilibrium
Engineering statics is the study of objects in static equilibrium, and the simple assumption of all [[Structural Analysis#Forces|forces]] adding up to zero is the basis for the subject area of engineering statics.
$\begin{equation*} \LARGE \sum \vec{F} = m \times \vec{a} \end{equation*}$

Where $\LARGE a = 0 ; \sum{\vec{F}} = 0$

Objects in static equilibrium are objects that are not accelerating (either linear acceleration or angular acceleration).
	These objects may be stationary, such as a building or a bridge, or they may have a constant velocity, such as a car or truck moving at a constant speed on a straight patch of road.
## [[Newton's Second Law|Newton's Second Law]]
States that the force exerted on an object is equal to the mass of the object times the [[Newton's Second Law#Acceleration|acceleration]] it experiences. 
	Therefore, if we know that the acceleration of an object is equal to zero, then we can assume that the sum of all forces acting on the object is zero. 
	
Individual forces acting on the object, represented by [[Structural Analysis#Vector|force vectors]], may not have zero magnitude but the sum of all the force vectors will always be equal to zero for objects in equilibrium. 
## [[Newton's Second Law#Angular Acceleration|Angular Acceleration]]
Equilibrium follows a similar pattern for angular accelerations. 
	The [[Newton's Second Law#Rotational Motion|rotational equivalent of Newton's Second Law]] states that the moment exerted on an object is equal to the moment of inertia of that object times the angular acceleration of the object.
		 If we know the angular acceleration of an object is equal to zero, then we know the sum of all moments acting on the object is equal to zero.

$\begin{equation*} \LARGE \sum{\vec{M}} = I \times \vec{a} \end{equation*}$
Where $\LARGE a = 0 ; \sum{\vec{M}} = 0$
## [[Structural Analysis#Static Equilibrium Point Forces|Point Forces]] as Vectors
A point force is any force where the **[[Structural Analysis#Point of Application|point of application]]** is considered to be a **single point**.
	In reality, most forces are technically surface forces, where the force is applied over an area, but when the area is small enough (in comparison to the bodies being analyzed) it can often be approximated as a point force.

Because point forces can be represented as a single vector (rather than a field of vectors for distributed forces), they are much easier to work with in engineering analysis.
	For this reason, point forces are used in place of distributed forces in engineering analysis whenever possible. 

The tensions in the cables supporting this container can be treated as point forces pulling in the direction of the cables.
![[Pasted image 20240503162219.png]]

The friction force between the bow and string on this cello can be treated as a point force
![[Pasted image 20240503162235.png]]
## Line of Action
![[Pasted image 20240503190856.png]]
The line of action of a force is the line along which the force acts. 
	It is the geometric representation of how the force is applied. 
	Given the direction and point of application, one can find the line of action, but this term will be important in discussing concurrent forces and in the [[Structural Analysis#Principle of Transmissibility|principle of transmissibility]].
## Force Vector Representation
When vectors are drawn to form [[Free Body Diagram|free body diagrams]], the magnitude and direction are usually given in one of two formats.

In either format we will need two values to fully define a force vector in a 2D system (either a magnitude and a single angle or a magnitude in each of the two coordinate axes).

And three values to fully define a force vector in a 3D system (either a magnitude and two angles or a magnitude in each of the three coordinate axes). 
### Magnitude and Direction Form
Overall magnitude and angle(s) to indicate direction.
##### 2Dimensional
![[Pasted image 20240503162507.png]]
##### 3Dimensional
![[Pasted image 20240503162807.png]]
### Component Form
Magnitudes in each of the coordinate directions.
##### 2Dimensional
![[Pasted image 20240503162606.png]]
##### 3Dimensional
![[Pasted image 20240503162812.png]]
### Converting Between Force Vector Forms
Because the two different forms of the vector are equivalent, we can switch between representations without changing the problem. 
	Often in engineering problems, it will initially be easier to write the force in magnitude and angle form, but later, analysis will be easier if forces are written in component form.
 
To switch from magnitude and direction form to component form you will use right triangles and trigonometry to determine the component of the overall magnitude in each direction. 
	This is a simple vector decomposition.
	To switch back from component form into magnitude and direction form you simply use the reverse of this initial process.
## Static Equilibrium Analysis for Concurrent Force Systems
If a body is in static equilibrium, then by definition that body is not accelerating. 
	If we know that the body is not accelerating then we know that **the sum of the forces acting on that body must be equal to zero**. 
		This is the basis for equilibrium analysis for a [[Points|particle]]. 

In order to solve for any unknowns in the sum of forces equation, turn the one vector equation into a set of scalar equations. 
	For two dimensional problems, split our one vector equation down into two scalar equations. 
		We do this by summing up all the $x$ components of the force vectors and setting them equal to zero in our first equation.
			Then summing up all the $y$ components of the force vectors and setting them equal to zero in our second equation.
	For three dimensional problems, add a third equation.
		The sum of all our $z$ components equal to zero.

 $\LARGE \sum{\vec{F_y}}​=0$
 $\LARGE \sum{F_x}​=0$ ; $\LARGE \sum{F_y}​=0$ ; $\LARGE \sum{F_z}​=0$

Trigonometry is essential for breaking down the forces into their x and y components when they're acting at an angle. 
	For a force vector at an angle β from the vertical, the trigonometric functions ($sin$) and ($cos$) are used to find the magnitudes of the components:
		- The x-component (horizontal) of the force is found by multiplying the force's magnitude by the sine of the angle: $F⋅sin(β)$.
		- The y-component (vertical) of the force is found by multiplying the force's magnitude by the cosine of the angle: $F⋅cos(β)$.

This breakdown allows you to add up all the horizontal components separately from all the vertical components, which is exactly what you do when you're solving for equilibrium.
	When the sum of the x-components and the sum of the y-components both equal zero, the object is in a state of equilibrium—it won't accelerate in any direction because the net force acting on it is zero.
### The Procedure for Finding the Equilibrium Equations
1. Draw a [[Free Body Diagram|free body diagram]] of the body being analyzed. 
	- The diagram should show all the known and unknown force vectors acting externally on the body.
	- In the free body diagram, provide values for any of the know magnitudes or directions for the force vectors and provide variable names for any unknowns (either magnitudes or directions).
		![[Pasted image 20240504003640.png]]
2. Chose the $x, y, z$ axes.
	- These axes must be perpendicular to one another, but do not need to necessarily have to be horizontal or vertical. 
3. Break down all of the force vectors into component scaled unit vectors along the $x, y, x$ directions. 
	- The first equation will be the sum of the magnitudes of the components in the $𝑥$ direction being equal to zero.
	- The second equation will be the sum of the magnitudes of the components in the $y$ direction being equal to zero.
	- And the third (if a 3D problem) will be the sum of the magnitudes in the $z$ $direction being equal to zero.
	- Collectively these are known as the **equilibrium equations**.
1. Solve the unknowns using algebra. 
	- The number of unknowns that you will be able to solve for will be the number of equilibrium equations that you have.
	- In instances where you have more unknowns than equations, the problem is known as a **statically indeterminate problem** and you will need additional information to solve for the given unknowns.