# Components of Motion
## Position
Position refers to the specific location of an object in space at a given point in time.
	It is described relative to a reference point, typically called the origin, in a coordinate system.
#### Change of Position as Displacement
When we derive the kinematic equations from the basic principles of motion, we integrate acceleration to find velocity and then integrate velocity to find displacement.
#### Position as Vector Components $x(t)$, $y(t)$, $z(t)$ 
Are the scalar components of the position vector.
	"Scalar components" refers to the "points" that a [[Abstract Mathematical Spaces#Vector Fields|vector field maps to a vector.]]
###### Scalar Quantity
A **[[Static Equilibrium#Scalars|scalar]]** because it is a single numerical value.

A scalar quantity is a single value that represents magnitude but does not have direction.
	In the context of 1D motion, the position $x(t)$ is a scalar because it is a single numerical value that describes the object's location along a single axis.
###### Coordinate
A **[[Static Equilibrium#Coordinates|coordinate]]** because it specifies the object's position along the $x$ axis.

A coordinate is a value that specifies a position in a space relative to some reference point (the origin).
#### Position as Basis Vectors $\hat{i}$ and $\hat{j}$ and $\hat{k}$
Are the unit vectors in the $x$ $y$ and $z$ directions, respectively.
#### 1D Position
$\LARGE x(t)$ 
In 1D, the position of an object is represented by a single coordinate, typically $x(t)$, which is a function of time, $t$. 
	This coordinate is itself a scalar value that indicates the object's location along a single axis.
#### 2D and 3D Positions are Represented by [[Static Equilibrium#Position Vectors|Position Vectors]]
In a two-dimensional space, position is represented by a vector, $\vec{r}$ 

Where each position vector contains 2 or 3 coordinates for each dimension.
	Therefore, representing its components in those dimensions.
		The components provide the necessary information to describe both the magnitude and direction of the vector in space.
###### The components of the Velocity Vector are themselves, scalars.
These scalar components scale the basis vectors (i.e. standard  unit vectors) to define the direction and magnitude of the vectors in each dimension.
###### Unit Vector Form
#### $\LARGE \vec{r}(t) = x(t) \hat{i} + y(t) \hat{j}$
###### Column Vector Form
#### $\LARGE \vec{r}(t) = \begin{pmatrix} x(t) \\ y(t) \end{pmatrix}$

In a three-dimensional space, position is represented by a vector, $\vec{r}$
$\LARGE \vec{r}(t) = x(t) \hat{i} + y(t) \hat{j} + z(t) \hat{k}$
where $\hat{i}$, $\hat{j}$, and $\hat{k}$ are the unit vectors along the $x$, $y$, and $z$ axes respectively.
### [[Derivatives|Position as the Basis for Velocity]]
#### First Derivative: Rate of Change
The first derivative of a function $x(t)$ with respect to time $t$ measures the rate of change of $x(t)$. 
	This is often referred to as the velocity in physical contexts. 
		Mathematically, it's written as:
#### $\LARGE v(t) = {dx(t) \over dt}$

This tells us how the position $x(t)$ changes as time changes.
###### [[Newton's Second Law#Velocity|Velocity]]
Velocity is defined as the rate of change of position with respect to time.
It describes how fast and in which direction an object's position is changing.

**Mathematical Definition**
The [[#Velocity Vector|velocity vector]] $\vec{v}(t)$ is the first derivative of the position vector $\vec{r}(t)$ with respect to time: 
$\LARGE \vec{v}(t) = {d\vec{r}(t) \over dt}$

**Components**:
In one-dimensional motion, velocity is the derivative of the position function: 
$\LARGE v(t) = \frac{dx(t)}{dt}$
    
In two-dimensional motion, velocity is the derivative of the position vector: 
$\LARGE \vec{v}(t) = \frac{d}{dt} (x(t) \hat{i} + y(t) \hat{j}) = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j}$
    
In three-dimensional motion, velocity is: 
$\LARGE \vec{v}(t) = \frac{d}{dt} (x(t) \hat{i} + y(t) \hat{j} + z(t) \hat{k}) = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} + \frac{dz(t)}{dt} \hat{k}$
### [[Second Derivatives|Velocity as the Basis for Acceleration]]
The second derivative of $x(t)$ with respect to time $t$ measures the rate of change of the velocity, or equivalently, the rate of change of the rate of change of the position.
	This is known as the acceleration in physical contexts.
		 Mathematically, it's written as:
#### $\LARGE v(t) = {d\over dt}({dx(t) \over dt}) = {d^{2}x(t)\over dt^{2}}$

Where $\Large {d\over dt}({dx(t) \over dt})$ means **"change of a change in..."**
	Therefore, you get $\Large {d^{2}x(t)\over dt^{2}}$
### Example
Let's consider an example in two-dimensional motion:
###### Position Vector: Suppose the position vector of a particle is given by: 
$\LARGE \vec{r}(t) = t^2 \hat{i} + t^3 \hat{j}$
###### Velocity Vector: The velocity vector is the derivative of the position vector: 
$\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{d}{dt} (t^2 \hat{i} + t^3 \hat{j}) = 2t \hat{i} + 3t^2 \hat{j}$

This tells us how the position changes with time, both in magnitude and direction.
### Path of the Object
This is the actual trajectory that the object follows over time.
	It refers to the actual path that the object follows as it moves. 

Can be [[Uniform Motion|uniform]] and/or [[Linear Motion|linear]], or [[Non-Linear Motion|non-linear]].
	I.e. This path can be any shape: a straight line, a parabola, a circle, or a more complex curve.

If the path is non-linear then it is a "[[Curves|curve]]".
###### [[#Position Vector|Position Vector]]
The vector that describes the position of the object at any given time $t$.
$\vec{r}(t) = (x(t), y(t))$
###### [[#Velocity Vector|Velocity Vector]]
The velocity vector is tangent to this path at any given point and represents the instantaneous direction and speed of the object.

The derivative of the position vector with respect to time, representing the object's instantaneous velocity and direction.
$\vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \left( \frac{dx(t)}{dt}, \frac{dy(t)}{dt} \right)$
###### [[#Osculating Circle|Osculating Circle]]:
At any given point on the path, the osculating circle provides the best local approximation of the curve of the path of the object.
	The radius of curvature ($r$) and the center of curvature define this osculating circle.
	The normal (centripetal) acceleration points towards the center of the osculating circle and is responsible for changing the direction of the velocity vector, keeping the object on the curved path.
### [[Notion of Surface Curvature#Oscillating Circles|Circular Path]]
Refers to the osculating circle, which is the circle that best approximates the curvature of a path of the object at a given point. 
	The osculating circle provides a local representation of the path's curvature and is directly related to the concept of centripetal (normal) acceleration.

When an object moves along a curved path, its velocity vector changes direction continuously. 
	To maintain this curved motion, there must be an acceleration component that is perpendicular to the velocity vector. 
		This [[#Normal (i.e. Perpendicular) Acceleration|perpendicular acceleration]] is called the normal or centripetal acceleration.
			 The osculating circle provides a geometric representation of this curvature at any given point on the path.
			 
I.e. The "circular path" in the context of normal (centripetal) acceleration refers to the osculating circle at a given point on the curve. 
	The normal acceleration vector is perpendicular to the velocity vector and points towards the center of this osculating circle, ensuring the object follows the curved path.
		 This concept helps in understanding how the curvature of the path and the corresponding acceleration components interact to produce the observed motion.
#### Osculating Circles
#### $\LARGE \vec{a}_{\perp}(t) = \left( \frac{|\vec{v}|^2}{r} \right) \hat{n}$
Where $\hat{n}$ is the unit vector towards the [[Notion of Surface Curvature#Center of Curvature|center of curvature]].
	Therefore, this is the scaling of the normal vector (directed towards the center of curvature). 
		By a factor of magnitude of velocity, squared, [[Division#Contracting|divided]] by radius of the osculating circle. 

**Pertains to**: **[[#Relationship Between Acceleration and Velocity Vectors|Acceleration]]** and **[[Notion of Surface Curvature#Oscillating Circles|Curvature]]**
**Purpose**: To describe how the path of an object curves at a specific point.
**Description**: An osculating circle at a point on a curve is the circle that best approximates the curve at that point. It has the same tangent and curvature as the curve at that point.
**[[Notion of Surface Curvature#Radius of Curvature|Radius of Curvature]]** ($r$): The radius of the osculating circle, representing the sharpness of the curve at a point.
#### $\vec{a}_{\perp}(t) = \left( \frac{|\vec{v}|^2}{r} \right) \hat{n}$

**[[Notion of Surface Curvature#Center of Curvature|Center of Curvature]]**: The center of the osculating circle.
**[[#Normal (i.e. Perpendicular) Acceleration|Normal (Centripetal) Acceleration]]**: The component of acceleration pointing towards the center of curvature, which changes the direction
#### $\vec{a}_{\perp}(t) = \left( \frac{|\vec{v}|^2}{r} \right) \hat{n}$

**Usage**: Helps understand the curvature of the path and the normal component of acceleration.
**Visualization**: Imagine a small circle that "kisses" the curve at a point, matching its curvature exactly.
#### [[Curves#Hodograph|Hodographs]]
Refers to the curve traced by the [[#Velocity Vector|velocity vector]] $\vec{v}(t)$ in velocity space.

**Pertains to**: **Velocity**
**Purpose**: To visualize how the velocity vector of a moving object changes over time.
**Description**: A hodograph is the locus of the tips of the velocity vectors plotted in velocity space. It shows how the velocity vector changes in both magnitude and direction.
**Velocity Space**: The space in which the hodograph is plotted, with coordinates representing components of the velocity vector.
**Instantaneous Velocity**: Each point on the hodograph represents the velocity vector of the object at a specific time.
**Usage**: Helps visualize how the velocity vector changes over time in terms of both magnitude and direction.
**Visualization**: Imagine plotting the tip of the velocity vector in a separate space (velocity space) as the object moves.
### Centripetal
The term **centripetal** comes from Latin words "centrum" meaning center and "petere" meaning to seek. 
	It refers to a [[Statics Analysis#Forces|force]] or [[#Newton's Second Law Acceleration Acceleration|acceleration]] that acts towards the center of a circular path.
		 In the context of motion, centripetal forces are responsible for keeping an object moving in a curved or circular path.

**Direction**
Centripetal force and acceleration always point towards the center of the circular path. 
	This inward force is what keeps the object moving in a circle rather than in a straight line.
#### Centripetal Force
Centripetal force is the force that keeps an object moving in a circular path and is directed towards the center of the circle around which the object is moving.

**Cause of Circular Motion**: Without centripetal force, an object would move off in a straight line due to [[Newton's First Law#Inertia|inertia]] ([[Newton's First Law|Newton's First Law of Motion]]). 
	The centripetal force changes the direction of the object's velocity, resulting in circular motion.
#### $\LARGE F_c = \frac{mv^2}{r}$
Where:
- $F_{c}$ is the centripetal force.
- $m$ is the mass of the object.
- $v$ is the magnitude of the [[#Tangential (i.e. Parallel) Acceleration|tangential velocity]] of the object.
- $r$ is the radius of the circular path.
#### Centripetal Acceleration
Centripetal acceleration is the acceleration that is directed towards the center of a circular path.
	It is responsible for changing the direction of the velocity vector of an object moving in a circular path.
#### $\LARGE a_c = \frac{v^2}{r}$
Where:
- $a_{c}$​ is the centripetal acceleration.
- $v$ is the tangential velocity of the object.
- $r$ is the radius of the circular path.
## [[Newton's Second Law#Velocity|Velocity]]
### [[Linear Motion#1D Motion Newton's Second Law Velocity Velocity|Velocity in Linear Motion]]
### [[Non-Linear Motion#Velocity|Velocity in Non-Linear Motion]]

### Velocity Vector
The velocity vector represents the rate of change of the position vector with respect to time.
	It indicates how fast and in which direction an object's position is changing.

***Remember***: The components of the Velocity Vector are themselves, scalars.
	These scalar components scale the basis vectors (i.e. standard  unit vectors) to define the direction and magnitude of the vectors in each dimension.
###### The velocity vector at a point on the curve is tangent to the curve at that point.
It represents the direction and rate of change of the position vector at that point.
###### Tangent Line
The tangent line at a point on the curve is the line that touches the curve at that point and has the same direction as the velocity vector.
	The velocity vector can be considered as a directed segment of the tangent line, scaled by the speed of the object.
###### Slope of the Tangent Line
The [[#1D Components of the Velocity Vector|components of the velocity vector]] represent the slopes of the tangent line in the respective coordinate directions.
	The components of the velocity vector give the rate of change of the position coordinates with respect to time, which is equivalent to the slope of the tangent line in each coordinate direction.
###### Example In 2D
###### Position Vector
#### $\LARGE \vec{r}(t) = (x(t), y(t))$
###### Velocity Vector
#### $\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \left( \frac{dx(t)}{dt}, \frac{dy(t)}{dt} \right)$
###### Tangent Line
At a specific point $(x_0, y_0)$ at time $t_0$, the tangent line can be described as:
#### $\LARGE y - y_0 = m (x - x_0)$
###### Slope of the Tangent Line
$m$ is the slope of the tangent line. 

The slope of the tangent line, $m$, is given by the **ratio** of the components of the velocity vector:
#### $\LARGE m = \frac{\frac{dy(t_0)}{dt}}{\frac{dx(t_0)}{dt}}$

###### Mathematical Definition:
The velocity vector $\vec{v}(t)$ is the first derivative of the position vector $\vec{r}(t)$ with respect to time: 
$\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt}$
##### 1D Components of the Velocity Vector
In 1D motion: 
$\LARGE v(t) = \frac{dx(t)}{dt}$
This derivative represents the [[Derivatives#Is the Tangent Line The Slope of a Tangent Line Slope (i.e. a rate/ratio between $ Delta y / Delta x$) of the Tangent Line Tangent Line|slope of the tangent line]] to the curve $x(t)$ at any point in time.
	In other words, it indicates how fast the position $x(t)$ is changing at that particular moment.
##### 2D Components of the Velocity Vector
In 2D motion: 
The **ratio** of the components $\frac{dx(t)}{dt}$ $\frac{dy(t)}{dt}$ are the [[Derivatives#Is the Tangent Line The Slope of a Tangent Line Slope (i.e. a rate/ratio between $ Delta y / Delta x$) of the Tangent Line Tangent Line|slopes of the tangent lines]] to the $x(t)$ and $y(t)$ components, respectively.
###### Unit Vector Form
#### $\LARGE\vec{v}(t) = \frac{d}{dt}(x(t) \hat{i} + y(t) \hat{j}) = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j}$
###### Column Vector Form
$\LARGE \vec{v}(t) = \begin{pmatrix} \frac{dx(t)}{dt} \\ \frac{dy(t)}{dt} \end{pmatrix}$
##### 3D Components of the Velocity Vector
In 3D motion: 
The **ratio** of the components $\frac{dx(t)}{dt}$ $\frac{dy(t)}{dt}$ and $\frac{dz(t)}{dt}$ are the [[Derivatives#Is the Tangent Line The Slope of a Tangent Line Slope (i.e. a rate/ratio between $ Delta y / Delta x$) of the Tangent Line Tangent Line|slopes of the tangent lines]] to the $x(t)$, $y(t)$ and $z(t)$ components, respectively.
###### Unit Vector Form
#### $\LARGE\vec{v}(t) = \frac{d}{dt}(x(t) \hat{i} + y(t) \hat{j} + z(t) \hat{k}) = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} + \frac{dz(t)}{dt} \hat{k}$
###### Column Vector Form
#### $\LARGE \vec{v}(t) = \begin{pmatrix} \frac{dx(t)}{dt} \\ \frac{dy(t)}{dt} \\ \frac{dy(t)}{dt} \end{pmatrix}$
###### Example of Velocity Vector
Let's consider an example in two-dimensional motion:
- **Position Vector**: Suppose the position vector of a particle is given by: $\vec{r}(t) = t^2 \hat{i} + t^3 \hat{j}$
- **Velocity Vector**: The velocity vector is the first derivative of the position vector: $\vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{d}{dt}(t^2 \hat{i} + t^3 \hat{j}) = 2t \hat{i} + 3t^2 \hat{j}$
## [[Newton's Second Law#Acceleration|Acceleration]]
### [[Linear Motion#1D Motion Newton's Second Law Acceleration |Acceleration in Linear Motion]]
### [[Non-Linear Motion#Acceleration|Acceleration in Non-Linear Motion]]
### Acceleration Vector
![[Pasted image 20240606124505.png|500]]
The acceleration vector represents the rate of change of the velocity vector with respect to time. 
	It indicates how fast and in which direction an object's velocity is changing.
Acceleration is **orthogonal** to the tangential velocity vector. 

***Remember***: The components of the Velocity Vector are themselves, scalars.
	These scalar components scale the basis vectors (i.e. standard  unit vectors) to define the direction and magnitude of the vectors in each dimension.
###### Mathematical Definition:
The acceleration vector $\vec{a}(t)$ is the first derivative of the velocity vector $\vec{v}(t)$ with respect to time, or equivalently, the second derivative of the position vector $\vec{r}(t)$ with respect to time: 
$\LARGE\vec{a}(t) = \frac{d\vec{v}(t)}{dt} = \frac{d^2\vec{r}(t)}{dt^2}$
#### Relationship Between Acceleration and Velocity Vectors
The Acceleration components represent the rate of change of the velocity vector with respect to time. 
	The relationship between the acceleration vector and the velocity vector depends on the type of motion.

The acceleration vector $\vec{a}(t)$ at any point can be decomposed into two components:
	[[#Tangential (i.e. Parallel) Acceleration|Tangential acceleration]] and [[#Normal (i.e. Perpendicular) Acceleration|normal (or centripetal) acceleration]]. 
		These components help describe how the velocity vector changes both in magnitude and direction.
I.e. In the general case, the acceleration vector can have both parallel (i.e. tangential) and perpendicular (i.e. normal) components relative to the velocity vector. 
##### Parallel Components I.e. Tangential Components
The component of acceleration that is parallel to the velocity vector. 
	This changes the speed (**magnitude** of the velocity) of the object.

If the acceleration vector is parallel (or anti-parallel) to the velocity vector, it means that the acceleration is affecting the magnitude of the velocity vector.
	I.e. Parallel/Tangential components **imply** Parallel/Tangential Acceleration.
		This is typical in cases of linear acceleration or deceleration.
###### Tangential (i.e. Parallel) Acceleration
Tangential acceleration, which is parallel to the velocity vector, changes the speed of the object.

Where $\hat{v}$ is the unit vector in the direction of the velocity vector $\vec{v}(t)$.
#### $\LARGE \vec{a}_{\parallel}(t) = \left( \frac{d|\vec{v}|}{dt} \right) \hat{v}$

***Example***: In 1D motion with constant acceleration, such as free fall under gravity (ignoring air resistance), the acceleration is in the same direction as the velocity.
##### Orthogonal Components I.e. Normal Components
The component of acceleration that is perpendicular to the velocity vector. 
	This changes the **direction** of the velocity vector without changing its magnitude.

If the acceleration vector is orthogonal (perpendicular) to the velocity vector, it means that the acceleration is affecting the direction of the velocity vector but not its magnitude.
	I.e. Normal/Orthogonal components **imply** Normal/Orthogonal Acceleration.
		This is typical in uniform circular motion, where the [[#Centripetal Acceleration|centripetal acceleration]] is always directed towards the center of the circular path and is perpendicular to the tangential velocity.
###### Normal (i.e. Perpendicular) Acceleration
Normal acceleration, which is perpendicular to the velocity vector, changes the direction of the velocity vector without changing its magnitude.

Where $\hat{n}$ is the unit vector pointing towards the [[Notion of Surface Curvature#Center of Curvature|center of the curvature]] of the path (perpendicular to $\hat{v}$ and $r$ is the [[Notion of Surface Curvature#Radius of Curvature|radius of curvature]].
	The normal (or centripetal) acceleration is directly related to the curvature of the path. 
		When an object moves along a curved path, the component of acceleration that is perpendicular to the velocity vector is the centripetal acceleration, which points towards the center of curvature.
#### $\LARGE \vec{a}_{\perp}(t) = \left( \frac{|\vec{v}|^2}{r} \right) \hat{n}$

***Example***: In uniform circular motion, the velocity vector is tangent to the [[#Circular Path|circular path]], and the acceleration vector ([[#Centripetal Acceleration|centripetal acceleration]]) is directed towards the center of the circle.
##### Ratio of the Components of the Acceleration Vector
###### The 2D ratio of the Acceleration Vector:

#### $\LARGE m_a = \frac{\frac{d^2y(t)}{dt^2}}{\frac{d^2x(t)}{dt^2}}$
###### The 3D ratio of the Acceleration Vector:

- **Ratio of $y$ component to $x$ component**:
    $\LARGE m_{a_{yx}} = \frac{\frac{d^2y(t)}{dt^2}}{\frac{d^2x(t)}{dt^2}}$
- **Ratio of $z$ component to $x$ component**: 
    $\LARGE m_{a_{zx}} = \frac{\frac{d^2z(t)}{dt^2}}{\frac{d^2x(t)}{dt^2}}$
- **Ratio of $z$ component to $y$ component**: 
	$\LARGE m_{a_{zy}} = \frac{\frac{d^2(t)}{dt^2}}{\frac{d^2y(t)}{dt^2}}$

This ratio describes:
###### Slope of the Acceleration Vector:
This ratio $m_{a}$​ represents the slope of the line formed by the acceleration vector components in the space. 
	It describes the direction of the acceleration in that space.
###### Direction of Acceleration
Just as the ratio of the velocity vector components gives the direction of the velocity (tangent to the path), the ratio of the acceleration vector components gives the direction of the acceleration.
###### Nature of Motion
The ratio can provide insights into how the acceleration is acting on the object. For example:
- If $m_{a}$​ is positive, the acceleration has components in the same direction as the respective coordinate axes.
- If $m_{a}$​ is negative, the acceleration has components in opposite directions along the coordinate axes.
- If $m_{a}$​ is zero, the acceleration is entirely in the $x$ direction.
- If $m_{a}$​ is undefined (i.e., the denominator is zero), the acceleration is entirely in the $y$ direction.
##### 1D Components of the Acceleration Vector
In 1D motion.
$\LARGE a(t) = \frac{dv(t)}{dt} = \frac{d^2x(t)}{dt^2}$
##### 2D Components of the Acceleration Vector
In 2D motion.
###### Unit Vector Form
#### $\LARGE \vec{a}(t) = \frac{d}{dt}(\frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j}) = \frac{d^2x(t)}{dt^2} \hat{i} + \frac{d^2y(t)}{dt^2} \hat{j}$
###### Column Vector Form
#### $\LARGE \vec{a}(t) = \begin{pmatrix} \frac{d^2x(t)}{dt^2} \\ \frac{d^2y(t)}{dt^2} \end{pmatrix}$

##### 3D Components of the Acceleration Vector
In 3D motion.
###### Unit Vector Form
#### $\LARGE \vec{a}(t) = \frac{d}{dt}(\frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} + \frac{dz(t)}{dt} \hat{k}) = \frac{d^2x(t)}{dt^2} \hat{i} + \frac{d^2y(t)}{dt^2} \hat{j} + \frac{d^2z(t)}{dt^2} \hat{k}$
###### Column Vector Form
#### $\LARGE \vec{a}(t) = \begin{pmatrix} \frac{d^2x(t)}{dt^2} \\ \frac{d^2y(t)}{dt^2} \\ \frac{d^2z(t)}{dt^2} \end{pmatrix}$

##### Example of Acceleration Vector
Let's consider an example in two-dimensional motion: 
Using the [[Derivatives#Power Rule|Power Rule of Differentiation]]
- **Position Vector**: Suppose the position vector of a particle is given by:
	$\LARGE \vec{r}(t) = t^2 \hat{i} + t^3 \hat{j}$
- **Velocity Vector**: The velocity vector is the first derivative of the position vector: 
	$\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{d}{dt}(t^2 \hat{i} + t^3 \hat{j}) = 2t \hat{i} + 3t^2 \hat{j}$
- **Acceleration Vector**: The acceleration vector is the first derivative of the velocity vector: 
	$\LARGE \vec{a}(t) = \frac{d\vec{v}(t)}{dt} = \frac{d}{dt}(2t \hat{i} + 3t^2 \hat{j}) = 2 \hat{i} + 6t \hat{j}$
#### Integral Example of Acceleration Vector with a Non-Zero Constant of Integration
Given the acceleration vector, we can integrate it to find the velocity and then integrate the velocity to find the position vector.
###### Acceleration Vector
Given:
#### $\LARGE \vec{a}(t) = 2 \hat{i} + 6t \hat{j}$
###### Velocity Vector
To find the velocity vector, integrate the acceleration vector with respect to time $t$:
#### $\LARGE \vec{v}(t) = \int \vec{a}(t) \, dt = \int (2 \hat{i} + 6t \hat{j}) \, dt = \int 2 \, dt \, \hat{i} + \int 6t \, dt \, \hat{j}$

1. Using the [[Integrals#Power Rule for Integration|power rule for integration]]:
	$\LARGE \vec{v}(t) = 2t \hat{i} + 3t^2 \hat{j} + \vec{v}_0$

	Where $\vec{v_{0}}$ is the [[Integrals#The Constant of Integration|constant of integration]] representing the initial velocity vector.

2. Let's assume a simple non-zero initial velocity vector, say $\vec{v_{0}}=\hat{i} + \hat{j}$.
		
	$\LARGE \vec{v}(t) = 2t \hat{i} + 3t^2 \hat{j} + (\hat{i} + \hat{j})$
		
3. Combining like terms, we get:

	$\LARGE \vec{v}(t) = (2t + 1) \hat{i} + (3t^2 + 1) \hat{j}$
###### Position Vector
To find the position vector, integrate the velocity vector with respect to time $t$:
#### $\LARGE \vec{r}(t) = \int \vec{v}(t) \, dt = \int ((2t + 1) \hat{i} + (3t^2 + 1) \hat{j}) \, dt = \int (2t + 1) \, dt \, \hat{i} + \int (3t^2 + 1) \, dt \, \hat{j}$
1. Using the power rule for integration:
	$\LARGE \vec{r}(t) = \left( t^2 + t \right) \hat{i} + \left( t^3 + t \right) \hat{j} + \vec{r}_0$
	
	Where $\vec{r_{0}}$ is the [[Integrals#The Constant of Integration|constant of integration]] representing the initial position vector.

2. Let's assume a simple non-zero initial position vector, say $\vec{r_{0}}=\hat{i} + 2\hat{j}$.
	
	$\LARGE \vec{r}(t) = (t^2 + t) \hat{i} + (t^3 + t) \hat{j} + (\hat{i} + 2 \hat{j})$

3. Combining like terms, we get:

	$\LARGE \vec{r}(t) = (t^2 + t + 1) \hat{i} + (t^3 + t + 2) \hat{j}$
#### Integral Example of Acceleration Vector with a Constant of Integration of Zero
Given the acceleration vector, we can integrate it to find the velocity and then integrate the velocity to find the position vector.
###### Acceleration Vector
Given:
#### $\LARGE \vec{a}(t) = 2 \hat{i} + 6t \hat{j}$
###### Velocity Vector
To find the velocity vector, integrate the acceleration vector with respect to time $t$:
#### $\LARGE \vec{v}(t) = \int \vec{a}(t) \, dt = \int (2 \hat{i} + 6t \hat{j}) \, dt = \int 2 \, dt \, \hat{i} + \int 6t \, dt \, \hat{j}$

1. Using the [[Integrals#Power Rule for Integration|power rule for integration]]:
	$\LARGE \vec{v}(t) = 2t \hat{i} + 3t^2 \hat{j} + \vec{v}_0$

	Where $\vec{v_{0}}$ is the [[Integrals#The Constant of Integration|constant of integration]] representing the initial velocity vector.

2. For simplicity, if we assume the initial velocity $\vec{v_{0}}=0$.
		$\LARGE \vec{v}(t) = 2t \hat{i} + 3t^2 \hat{j}$
###### Position Vector
To find the position vector, integrate the velocity vector with respect to time $t$:
#### $\LARGE \vec{r}(t) = \int \vec{v}(t) \, dt = \int (2t \hat{i} + 3t^2 \hat{j}) \, dt = \int 2t \, dt \, \hat{i} + \int 3t^2 \, dt \, \hat{j}$

1. Using the power rule for integration:
	$\LARGE \vec{r}(t) = t^2 \hat{i} + t^3 \hat{j} + \vec{r}_0$
	
	Where $\vec{r_{0}}$ is the [[Integrals#The Constant of Integration|constant of integration]] representing the initial position vector.

2. For simplicity, if we assume the initial velocity $\vec{r_{0}}=0$.
		$\LARGE \vec{r}(t) = t^2 \hat{i} + t^3 \hat{j}$
