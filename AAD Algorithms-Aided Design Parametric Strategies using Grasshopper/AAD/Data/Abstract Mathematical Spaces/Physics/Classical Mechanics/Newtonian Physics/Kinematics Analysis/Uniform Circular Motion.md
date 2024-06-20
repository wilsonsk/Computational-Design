---
up:
  - "[[Circular Motion]]"
related: 
date created: 2024-06-18
---
# Uniform Circular Motion
Defined by a constant [[Circular Motion#Newton's Second Law Angular Velocity Angular Velocity ($ omega$)|Angular Velocity]].
##### Angular Velocity
$$\LARGE \omega(t) = \lim_{\triangle t \rightarrow 0}{\triangle \phi \over \triangle t} = \frac{d\phi}{dt} = \phi'(t) = \dot{\phi}$$
##### Angular Acceleration
$$\LARGE \alpha(t) = \frac{d\omega}{dt} = \frac{d^2\phi}{dt^2} = \dot{\omega} = \ddot{\phi}$$
## Constant Angular Velocity
$$\LARGE \omega = \omega_{0}$$
Meaning that $\LARGE \omega$ is a constant, $\LARGE \omega_{0}$.
	Remember that the [[Derivatives#Derivative of a Constant is Zero|derivative of a constant is zero]].
		Therefore, the [[Circular Motion#Newton's Second Law Angular Acceleration Angular Acceleration ($ alpha$)|Angular Acceleration]], $\LARGE \alpha = 0$.
	Remember that the [[Integrals#Constant Rule|integral of a constant is a linear function]].
		Therefore, the [[Circular Motion#Angular Position $ LARGE phi$|Angular Position]], $\LARGE \phi = \omega_{0} t + \phi_{0}$.
### Integrating to and from a Constant Angular Velocity
##### Integrating Angular Acceleration to Get Angular Velocity
If $\LARGE \alpha=0$, then the Integral of $\LARGE \alpha$ is the constant, $\LARGE \omega_{0}$.
$$\LARGE \omega = \int \alpha dt = \omega_{0}$$
##### Integrating Angular Velocity to Get Angular Position
If Angular Velocity, $\LARGE \omega_{0}$ is a constant.
$$\LARGE \phi = \int \omega dt = \omega_{0}t + \phi_{0}$$Where $\LARGE \phi_{0}$ is the [[Integrals#The Constant of Integration|Integration Constant]], which is the initial value of the angular position.
![[Pasted image 20240618133842.png]]
Where $\LARGE \omega$ is a constant, $\LARGE \omega_{0}=2$
	And $\LARGE \phi$ is a linear function that scales the constant $\LARGE \omega_{0}$ with time, $t$ starting at the initial Angular Position.
		After a full rotation, $\LARGE 2\pi$, the initial position changes. 
#### Compared to 1D Uniform Motion (non-circular)
Both are almost the same due to the 1 dimensional aspect.
	Except that in Circular Uniform Motion, we are using the effective coordinates.
		I.e. [[Circular Motion#Polar Coordinates|Polar Coordinates]].
###### Acceleration
$$\LARGE a = 0$$
###### Velocity
$$\LARGE v= {dx\over dt} = \text{const } v_{0}$$
###### Position
$$\LARGE x = v_{0} + x_{0}$$
Where $\LARGE x_{0}$ is the Integration Constant, that is, it is the initial position.

Therefore, sometimes, for position, it is more useful to utilize the Cartesian Coordinates system, that both motions share.
	Which makes the functions of position are [[Circular Motion#Period ($T$) and Frequency ($f$)|periodic]].
![[Pasted image 20240618134241.png]]
Remember, $\LARGE x = r \space \cos \phi$ , $\LARGE y = r \space \sin \phi$ and  but in the example above, we are using a unit circle.
	Therefore, the radius, $r=1$
## Constant [[Circular Motion#Newton's Second Law Angular Acceleration Angular Acceleration ($ alpha$)|Angular Acceleration]]
$$\LARGE \alpha = \alpha_{0}$$
Meaning that $\LARGE \alpha$ is a constant, $\LARGE \alpha_{0}$
	Remember that the [[Integrals#Constant Rule|integral of a constant is a linear function]].
		Therefore, the Angular Velocity, $\LARGE \omega = \alpha_{0} t + \omega_{0}$.
	Remember that the [[Integrals#Patterns of Integrals of Function Types|Integral of a Linear Function is a Quadratic Function]].
		Therefore, the Angular Velocity, $\LARGE \omega = \alpha_{0} t + \omega_{0}$.
### Integrating from a Constant Angular Acceleration
##### Integrating Angular Acceleration to Get Angular Velocity
If $\LARGE \alpha=\alpha_{0}$, then the Integral of $\LARGE \alpha_{0}$ is a Linear Function.
$$\LARGE \omega = \int \alpha dt = \alpha t + \omega_{0}$$
##### Integrating [[Circular Motion#Newton's Second Law Angular Velocity Angular Velocity ($ omega$)|Angular Velocity]] to Get [[Circular Motion#Angular Position $ LARGE phi$|Angular Position]]
If Angular Velocity, $\LARGE \omega$ is a Linear Function, the Integral of $\LARGE \omega$ is a Quadratic Function.
$$\LARGE \phi = \int \omega dt = \frac{1}{2}\alpha_{0}t^2 + \omega_{0}t + \phi_{0}$$
