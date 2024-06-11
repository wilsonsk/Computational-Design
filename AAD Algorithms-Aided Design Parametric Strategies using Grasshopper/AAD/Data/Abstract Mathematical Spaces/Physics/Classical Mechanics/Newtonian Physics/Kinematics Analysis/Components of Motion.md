# Components of Motion
## Position
Position refers to the specific location of an object in space at a given point in time.
	It is described relative to a reference point, typically called the origin, in a coordinate system.
#### Change of Position as Displacement
When we derive the kinematic equations from the basic principles of motion, we integrate acceleration to find velocity and then integrate velocity to find displacement.
#### Position as Vector Components $x(t)$, $y(t)$, $z(t)$ 
Are the scalar components of the position vector.
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
## [[Newton's Second Law#Velocity|Velocity]]
### [[Linear Motion#1D Motion Newton's Second Law Velocity Velocity|Velocity in Linear Motion]]
### [[Non-Linear Motion#Velocity|Velocity in Non-Linear Motion]]

#### Velocity Vector
The velocity vector represents the rate of change of the position vector with respect to time.
	It indicates how fast and in which direction an object's position is changing.

***Remember***: The components of the Velocity Vector are themselves, scalars.
	These scalar components scale the basis vectors (i.e. standard  unit vectors) to define the direction and magnitude of the vectors in each dimension.
	
**Mathematical Definition**:
The velocity vector $\vec{v}(t)$ is the first derivative of the position vector $\vec{r}(t)$ with respect to time: 
$\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt}$

**Components**:
In one-dimensional motion: 
$\LARGE v(t) = \frac{dx(t)}{dt}$

In two-dimensional motion: 
###### Unit Vector Form
#### $\LARGE\vec{v}(t) = \frac{d}{dt}(x(t) \hat{i} + y(t) \hat{j}) = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j}$
###### Column Vector Form
$\LARGE \vec{v}(t) = \begin{pmatrix} \frac{dx(t)}{dt} \\ \frac{dy(t)}{dt} \end{pmatrix}$

In three-dimensional motion: 
###### Unit Vector Form
#### $\LARGE\vec{v}(t) = \frac{d}{dt}(x(t) \hat{i} + y(t) \hat{j} + z(t) \hat{k}) = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} + \frac{dz(t)}{dt} \hat{k}$
###### Column Vector Form
#### $\LARGE \vec{v}(t) = \begin{pmatrix} \frac{dx(t)}{dt} \\ \frac{dy(t)}{dt} \\ \frac{dy(t)}{dt} \end{pmatrix}$
###### Example of Acceleration Vector
Let's consider an example in two-dimensional motion:
- **Position Vector**: Suppose the position vector of a particle is given by: $\vec{r}(t) = t^2 \hat{i} + t^3 \hat{j}$
- **Velocity Vector**: The velocity vector is the first derivative of the position vector: $\vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{d}{dt}(t^2 \hat{i} + t^3 \hat{j}) = 2t \hat{i} + 3t^2 \hat{j}$
## [[Newton's Second Law#Acceleration|Acceleration]]
### [[Linear Motion#1D Motion Newton's Second Law Acceleration |Acceleration in Linear Motion]]
### [[Non-Linear Motion#Acceleration|Acceleration in Non-Linear Motion]]
#### Acceleration Vector
![[Pasted image 20240606124505.png|500]]
The acceleration vector represents the rate of change of the velocity vector with respect to time. 
	It indicates how fast and in which direction an object's velocity is changing.
Acceleration is **orthogonal** to the tangential velocity vector. 

***Remember***: The components of the Velocity Vector are themselves, scalars.
	These scalar components scale the basis vectors (i.e. standard  unit vectors) to define the direction and magnitude of the vectors in each dimension.

**Mathematical Definition**:
The acceleration vector $\vec{a}(t)$ is the first derivative of the velocity vector $\vec{v}(t)$ with respect to time, or equivalently, the second derivative of the position vector $\vec{r}(t)$ with respect to time: 
$\LARGE\vec{a}(t) = \frac{d\vec{v}(t)}{dt} = \frac{d^2\vec{r}(t)}{dt^2}$

**Components**:
In one-dimensional motion: 
$\LARGE a(t) = \frac{dv(t)}{dt} = \frac{d^2x(t)}{dt^2}$

In two-dimensional motion: 
###### Unit Vector Form
#### $\LARGE \vec{a}(t) = \frac{d}{dt}(\frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j}) = \frac{d^2x(t)}{dt^2} \hat{i} + \frac{d^2y(t)}{dt^2} \hat{j}$
###### Column Vector Form
#### $\LARGE \vec{a}(t) = \begin{pmatrix} \frac{d^2x(t)}{dt^2} \\ \frac{d^2y(t)}{dt^2} \end{pmatrix}$

In three-dimensional motion: 
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
