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
###### [[Static Equilibrium#Position Vectors|Position Vector]]: 
The position of the object is described by a vector that changes with time. 
	In 2D, it is:
		$\LARGE \vec{r}(t) = x(t) \hat{i} + y(t) \hat{j}$
	In 3D, it is:
		$\LARGE \vec{r}(t) = x(t) \hat{i} + y(t) \hat{j} + z(t) \hat{k}$
#### Velocity
###### Velocity Vector:
The velocity vector also changes with time, reflecting changes in both speed and direction. 
	In 2D, it is:
		$\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j}$
	In 3D, it is:
		$\LARGE \vec{v}(t) = \frac{d\vec{r}(t)}{dt} = \frac{dx(t)}{dt} \hat{i} + \frac{dy(t)}{dt} \hat{j} + \frac{dz(t)}{dt} \hat{k}$
#### Acceleration
- **Variable Acceleration**: Non-linear motion often involves acceleration that changes in both magnitude and direction. This means the object is not only speeding up or slowing down but also changing direction.
- **Centripetal Acceleration**: In circular motion, the acceleration is directed towards the center of the circle, causing the object to change direction continuously.
###### Acceleration Vector
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
###### Projectile Motion:
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