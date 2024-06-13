---
up:
  - "[[Kinematics Analysis]]"
related: 
date created: 2024-06-08
---
# Non-Linear Motion
**Non-linear motion** refers to any type of motion that does not follow a straight line, meaning the path of the moving object is curved or involves changes in direction. 

This encompasses a wide range of motion types and can include motion in two or three dimensions.
	Non-linear motion is characterized by a changing velocity vector, which means both the magnitude and the direction of velocity can change over time.
### Key Characteristics of Non-linear Motion
#### Dimensions
Non-linear motion can occur in:
- **[[#Non-Linear Motion in 2D|Two Dimensions (2D)]]**: Motion occurs in a plane, requiring two coordinates to describe the position of the object.
- **Three Dimensions (3D)**: Motion occurs in space, requiring three coordinates to describe the position of the object.
#### Position
###### [[Components of Motion#Position Vector|Position Vector]]
The position of the object is described by a vector that changes with time. 
	In 2D, it is:
		$\LARGE \vec{r}(t) = x(t) \hat{i} + y(t) \hat{j}$
	In 3D, it is:
		$\LARGE \vec{r}(t) = x(t) \hat{i} + y(t) \hat{j} + z(t) \hat{k}$
#### Velocity
###### [[Components of Motion#Velocity Vector|Velocity Vector]]
The velocity vector also changes with time, reflecting changes in both speed and direction. 
	In 2D, it is:
		$\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j}$
	In 3D, it is:
		$\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} + \frac{dz(t)}{dt} \hat{k}$
#### Acceleration
- **Variable Acceleration**: Non-linear motion often involves acceleration that changes in both magnitude and direction. This means the object is not only speeding up or slowing down but also changing direction.
- **Centripetal Acceleration**: In circular motion, the acceleration is directed towards the center of the circle, causing the object to change direction continuously.
###### [[Components of Motion#Acceleration Vector|Acceleration Vector]]
The acceleration vector, $\vec{a}(t)$, is the derivative of the velocity vector, $\vec{v}(t)$, with respect to time. 
	It can be expressed as:
		$\LARGE \vec{a}(t) = \frac{d\vec{v}(t)}{dt}$
###### 2D Components
If the position vector is $\vec{r}(t) = x(t) \hat{i} + y(t) \hat{j}$​, the acceleration vector components are:
	$\LARGE \vec{a}(t) = \frac{d\vec{v}(t)}{dt} = \frac{d}{dt} \left( \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} \right) = \frac{d^2x(t)}{dt^2} \hat{i} + \frac{d^2y(t)}{dt^2} \hat{j}$
###### 3D Components
If the position vector is $\vec{r}(t) = x(t) \hat{i} + y(t) \hat{j} + z(t) \hat{k}$, the acceleration vector components are:
$\LARGE \vec{a}(t) = \frac{d\vec{v}(t)}{dt} = \frac{d}{dt} \left( \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} + \frac{dz(t)}{dt} \hat{k} \right) = \frac{d^2x(t)}{dt^2} \hat{i} + \frac{d^2y(t)}{dt^2} \hat{j} + \frac{d^2z(t)}{dt^2} \hat{k}$
### Types of Non-linear Motion
###### Projectile Motion
**Dimensions**: Typically in 2D.
**Acceleration**: Constant acceleration due to gravity acting downward.
**Position**:
	$\LARGE \vec{r}(t) = (v_0 \cos \theta) t \hat{i} + \left( (v_0 \sin \theta) t - \frac{1}{2} g t^2 \right) \hat{j}$
**Velocity**:
	$\LARGE \vec{v}(t) = (v_0 \cos \theta) \hat{i} + \left( (v_0 \sin \theta) - g t \right) \hat{j}$
###### Circular Motion:
**Dimensions**: Can be in 2D (circular path) or 3D (helical path).
**Acceleration**: Centripetal acceleration directed towards the center of the circle.
**Position**:
	$\LARGE \vec{r}(t) = R \cos(\omega t) \hat{i} + R \sin(\omega t) \hat{j}$
**Velocity**: 
	$\LARGE \vec{v}(t) = -R \omega \sin(\omega t) \hat{i} + R \omega \cos(\omega t) \hat{j}$
**Acceleration**:
	$\LARGE \vec{a}(t) = -R \omega^2 \cos(\omega t) \hat{i} - R \omega^2 \sin(\omega t) \hat{j}$
###### Oscillatory Motion:
**Dimensions**: Typically in 1D or 2D.
**Acceleration**: Variable acceleration that changes direction, such as in simple harmonic motion.
**Position**:
	 $\LARGE x(t) = A \cos(\omega t + \phi)$
**Velocity**:
	$\LARGE v(t) = -A \omega \sin(\omega t + \phi)$
**Acceleration**:
	$\LARGE a(t) = -A \omega^2 \cos(\omega t + \phi)$
## Non-Linear Motion in 2D
![[Pasted image 20240608205940.png]]
Non-linear motion in 2D involves the movement of an object in a plane where the path is not a straight line. 

This type of motion can be understood and analyzed by breaking it down into components along two perpendicular axes, typically denoted as $x$ and $y$.
### Superposition Principle
The principle of superposition states that the net response caused by two or more forces is the sum of the responses that would have been caused by each force individually. 

In the context of motion, this means that the total motion can be considered as the vector sum of the individual motions along the $x$ and $y$ and $z$ axes.

I.e. The principle of superposition states that the motion in each dimension can be treated independently and then combined to get the resultant motion.
#### Application in Motion
When applied to kinematics, the superposition principle allows us to analyze the motion of an object in multiple dimensions by breaking it down into simpler, independent motions along each coordinate axis. 

The overall motion is then obtained by vectorially adding these independent motions.
##### Key Concepts
###### Independence of Components
Motion along one axis does not affect motion along another axis.
For example, in 2D motion, the motion along the $x$ axis and $y$ axis can be treated separately.
###### Additive Nature
The total motion is the vector sum of the individual motions along each axis.
### Applying Superposition to 2D Motion
![[Pasted image 20240609153727.png]]
#### 2D [[Components of Motion|Components of Motion]]
In 2D projectile motion, the motion can be decomposed into horizontal (x-axis) and vertical (y-axis) components.
#### Horizontal Motion (x axis)
###### Given Acceleration in the Horizontal Direction 
The horizontal motion is typically uniform motion with constant velocity because there is no acceleration in the horizontal direction (assuming no air resistance).
#### $\LARGE \vec{a_{0}} =\begin{pmatrix} 0 \\ -g \\ 0\end{pmatrix}$
Therefore:
#### $\LARGE a_{x} = 0$
###### Velocity in the Horizontal Direction
Obtained by Integrating Acceleration.
The [[Integrals#Integral of Zero|integral of 0]] with respect to time $t$ is a constant, which represents the initial velocity, $\vec{v_0x}$.
	This is because there is no change in the quantity we are integrating.
		And therefore, whatever the initial condition (i.e. velocity) is, that is what remains and stays constant. 
#### $\LARGE v_{x}(t) = \int a_{x}dt = \int 0dt = C$
Here, $C$ is the constant of integration.
	This constant represents the initial velocity of the object, denoted as $v_{0x}$​.
		 It signifies that the velocity remains constant over time because there is no acceleration to change it.
			 Thus we write:
				 $\LARGE v_{x}(t) = v_{0x}$
#### $\LARGE v_{x}(t) = v_{0x}$

Therefore:
#### $\LARGE \vec{v_{0}} =\begin{pmatrix} v_{0x} \\ 0 \\ 0\end{pmatrix}$

***Note***: If the velocity was in the $y$ direction and there was no acceleration in that direction, the velocity would remain constant over time. 

	$v_{y}(t) = \int a_{y}dt = \int 0dt = C$

	 $v_{y}(t) = v_{0y}$
###### Position in the Horizontal Direction
Obtained by Integrating Velocity.
Is a constant velocity.
#### $\LARGE r_{0} = x(t) = v_{0x}t = h$

Therefore:

#### $\LARGE \vec{r_{0}} =\begin{pmatrix} 0 \\ h \\ 0\end{pmatrix}$

#### Vertical Motion (y-axis):
###### Given Acceleration in the Vertical Direction
The vertical motion is influenced by gravity, leading to [[Uniform Acceleration|uniform accelerated motion]].
#### $\LARGE \vec{a_{0}} =\begin{pmatrix} 0 \\ -g \\ 0\end{pmatrix}$

###### Velocity in the Vertical Direction
Obtained by Integrating Acceleration.
	Decreasing linearly.
If:
#### $\LARGE a_{y} = -g$

Recall that acceleration is the rate of change of velocity:
#### $\LARGE a_{y} = {dv_{y} \over dt}$

Therefore:
#### $\LARGE = {dv_{y} \over dt} = -g$

[[Integrals#Power Rule for Integration|Integrate]] to find $\LARGE v_{y}(t)$:
#### $\LARGE v_{y}(t) = \int {dv_{y} \over dt} dt = \int -gdt$

***Important***: Remember that when [[Integrals#Constant Rule|integrating a constant]] with respect to $t$, you simply multiply the constant by $t$.
	In this case $-g$ is the constant. 
		Therefore 

The left side integrates to $v_{y}(t)$, and the right side integrates to $-gt$, plus a constant of integration, $C$:
#### $\LARGE v_{y}(t) = -gt + C$

$\LARGE −gt$ represents the change in velocity due to gravity in the $y$ direction over time $t$.

$C$ is just the initial velocity in the vertical, $y$ direction at $t=0$.
	Therefore 
		$\LARGE C = v_{0y}$

Therefore:
#### $\LARGE v_{y}(t) = v_{0y} -gt$

Therefore:
#### $\LARGE \vec{v} = \int a(t)dt =\begin{pmatrix} v_{0x} \\ -gt \\ 0\end{pmatrix}$
*The function is plotted here.*
	Where $-g$ is the slope applied to the linear function, $v_{y}(t) = v_{0y} -gt$.
	The velocity in the x direction is constant.
![[Pasted image 20240612223120.png]]

###### Position in the Vertical Direction
Obtained by Integrating Velocity.
	Is a constant acceleration.
#### $\LARGE y_{t} = v_{0y}t - {1\over2}gt^{2} + h$

Therefore:
#### $\LARGE \vec{r} = \int v(t)dt =\begin{pmatrix} v_{0t} \\ {1\over 2}-gt^{2} + h \\ 0\end{pmatrix}$

#### Combining the Components
By treating the horizontal and vertical motions independently, we can use the principle of superposition to combine them and get the overall motion in 2D.
##### Position Vector
The position vector is the integral of the velocity vector:
	Where each component of the vector is a scalar.
#### $\LARGE \vec{r}(t) = \begin{pmatrix} x(t) \\ y(t) \end{pmatrix} = \int \vec{v}(t)dt = \begin{pmatrix} v_{0x} t \\ -\frac{1}{2}gt^2 + v_{0y}t + h \end{pmatrix}$

This shows that the horizontal position $x(t) = v_{0x}t$ increases linearly with time, while the vertical position $v_{0y} t - \frac{1}{2} g t^2 + h$ follows a parabolic path due to the influence of gravity.
##### Velocity Vector
The velocity vector is the combination of the horizontal and vertical components:
#### $\LARGE \vec{v}(t) = \begin{pmatrix} v_x(t) \\ v_y(t) \end{pmatrix} = \begin{pmatrix} v_{0x} \\ -gt + v_{0y} \end{pmatrix}$

This shows that the horizontal component of velocity $v_{0x}$​ remains constant, while the vertical component $v_{0y} - gt$ decreases linearly due to gravity.
##### Acceleration Vector
This represents the constant acceleration due to gravity in the negative $y$ direction.
#### $\LARGE \vec{a}(t) = \begin{pmatrix} a_x(t) \\ a_y(t) \end{pmatrix} = \begin{pmatrix} 0 \\ -g \end{pmatrix}$
