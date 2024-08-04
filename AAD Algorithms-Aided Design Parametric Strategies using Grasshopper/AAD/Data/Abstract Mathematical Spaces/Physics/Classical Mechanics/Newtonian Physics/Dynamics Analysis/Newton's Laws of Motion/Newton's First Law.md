---
up:
  - "[[Newtonian Mechanics]]"
related:
  - "[[Dynamics Analysis]]"
  - "[[Statics Analysis]]"
  - "[[Newton's Second Law]]"
  - "[[Newton's Third Law]]"
date created: 2024-05-03
---
# Newton's First Law (i.e. the Law of Inertia)
**"Every body continues in its state of rest, or of [[Uniform Motion|uniform motion]] in a straight line, unless it is compelled to change that state by forces impressed upon it.**"
	I.e. "A body at rest will remain at rest unless acted on by an unbalanced force. A body in motion continues in motion with the same speed and in the same direction unless acted upon by an unbalanced force."

I.e. Things don't change their motion on their own. 
	If something is sitting still, it won't start moving unless something pushes or pulls on it. 
		If something is already moving, it will keep moving in the same way (same speed and direction) until something makes it speed up, slow down, or change direction.
			 This means that objects naturally resist changes to their motion unless a force acts on them.

![[Pasted image 20240525095654.png]]

This law, also sometimes called the "law of inertia", means that bodies maintain their current velocity unless a force is applied to change that velocity. 
	If an object is at rest with zero velocity it will remain at rest until some force begins to change that velocity, and if an object is moving at a set speed and in a set direction it will remain at that same velocity until some force acts on it to change its velocity.
## Inertia
Inertia is the tendency of objects in motion to stay in motion and objects at rest to stay at rest, unless a force causes its speed or direction to change. 
	I.e. The tendency of an object to resist changes in their state of motion. 
		The greater the inertia, the more force is required to change the object's state of motion (either to start moving, stop moving, or change direction).

Inertia is a general property of matter that describes an object's resistance to changes in its state of motion. In linear motion, it’s reflected in an object's mass. 
	The greater the mass, the greater the inertia.
### Moment of Inertia
The moment of inertia ($I$) is a specific measure of an object's resistance to changes in its rotational motion around an axis. It depends on the mass distribution relative to that axis.
	The moment of inertia is a key factor in rotational dynamics and is analogous to mass in linear motion.

$\LARGE I = {L \over \omega}$
	Where $I$ is the [[Moment|Moment]] of inertia.
	Where $L$ is [[Newton's Second Law#Angular Momentum|angular momentum]].
	Where $\omega$ is [[Newton's Second Law#Angular Velocity|angular velocity]].
##### Calculating Moment of Inertia ($I$)
Given angular momentum, you differentiate it to find angular velocity and then use that to find the moment of inertia.
![[Pasted image 20240802055712.png|300]]
## Mass
Is the quantitative measure of inertia, a fundamental property of all matter.
	Mass directly quantifies the amount of inertia an object has. 
		The more mass an object has, the greater its inertia, and therefore the more it resists changes to its motion.
			The greater the mass, the greater the inertia, and the more force is required to change the object's state of motion.

$\LARGE m = {\rho \over V}$
Where $m$ is mass.
	Where $\rho$ is **density**.
	Where $V$ is **volume**.

[[Newton's Second Law|Newton's second law of motion]], $F = ma$, further illustrates the role of mass in inertia. 
	It states that the force ($F$) required to accelerate an object is equal to the mass ($m$) of the object times its acceleration ($a$).

## Newton's Universal Law of Gravitational Force
The gravitational force between two masses is given by Newton's law of universal gravitation:
$$\LARGE F =\pm G \frac{m_1 m_2}{r^2} \cdot e_{m_{1}m_{2}}$$

where:
- $F$ is the gravitational force between the two masses,
- $G$ is the gravitational constant ($6.67430 \times 10^{-11} \, \text{m}^3 \text{kg}^{-1} \text{s}^{-2}$),
- $m_1$​ and $m_2$ are the masses of the two objects,
- $r$ is the distance between the centers of the two masses.
- $e$ is the standard unit vector that connects the two objects.
### [[Weight and Gravity#Falling Gravity *as* Constant Acceleration|Gravity]] as [[Newton's Second Law#Acceleration|Acceleration]] 
On Earth, the value of gravity is $\large 9.8 m/s^{2}$ 
**Acceleration Due to Gravity ($g$)**

For an object near the Earth's surface, the Earth can be considered as one mass ($m_1 = M_{\text{Earth}}$) and the object as the other mass ($m_2 = m$). The distance $r$ is approximately the radius of the Earth ($R_{\text{Earth}}$).

Substituting these into the gravitational force equation:

$$\LARGE F = \frac{G M_{\text{Earth}} m}{R_{\text{Earth}}^2}$$​

According to Newton's second law of motion ($F = m \cdot a$), the force $F$ acting on an object of mass $m$ can also be written as:

$$\LARGE F = m \cdot g$$
Equating the two expressions for $F$:

Cancel the mass $m$ from both sides:
$$\LARGE g = \frac{G M_{\text{Earth}}}{R_{\text{Earth}}^2}$$
Here, $g$ is the acceleration due to gravity at the surface of the Earth. Plugging in the known values for the gravitational constant $G$, the mass of the Earth $M_{\text{Earth}}$, and the radius of the Earth $R_{\text{Earth}}$:

$$\LARGE G \approx 6.67430 \times 10^{-11} \, \text{m}^3 \text{kg}^{-1} \text{s}^{-2}G≈6.67430×10−11m3kg−1s−2$$
$$\LARGE M_{\text{Earth}} \approx 5.972 \times 10^{24} \, \text{kg}$$
$$\LARGE R_{\text{Earth}} \approx 6.371 \times 10^6 \, \text{m}$$
Substituting these values:
$$\LARGE g = \frac{(6.67430 \times 10^{-11}) \cdot (5.972 \times 10^{24})}{(6.371 \times 10^6)^2} \approx 9.8 \, \text{m/s}^2$$

## Force *of* [[Weight and Gravity#Falling Force *of* Gravity *as* Weight|Gravity as Weight]] (an Approximation)
$$\LARGE F_{\text{gravity}} = m \cdot - g \space \text{ where } g = 9.8 \mathbf{m}/\mathbf{s^2}$$
## [[Weight and Gravity#Weight (i.e. the "downward" Force acting on an Object due to Gravity)|Weight]]
Refers to the force acting on the object due to acceleration of gravity.
	Some standard textbooks define weight as a vector quantity, the gravitational force acting on the object. Others define weight as a scalar quantity, the magnitude of the gravitational force. 
	
$\LARGE W = mg$
Where $W$ is weight.
	Where $m$ is mass.
	Where $g$ is constant [[Newton's Second Law#Acceleration|acceleration]] due to gravity (in the negative z direction).

## Density
Density is a substance's mass per unit of volume.

$\LARGE \rho = m \times V$
Where $m$ is mass.
	Where $\rho$ is **density**.
	Where $V$ is **volume**.
## Volume
Is the amount of three-dimensional space occupied by matter or enclosed by a surface.

$\LARGE V = {\rho \over m}$
Where $m$ is mass.
	Where $\rho$ is **density**.
	Where $V$ is **volume**.
## Net Forces
It is important to note that the **net force** is what will cause a change in [[Newton's Second Law#Velocity|velocity]]. 
	The net force is the sum of all forces acting on the body. 
		*For example*, we can imagine gently pushing on the rock in the figure above and observing that the rock does not move. 
			This is because we will have a friction force equal in magnitude and opposite in direction opposing our gentle pushing force. 
				The sum of these two forces will be equal to zero, therefore the net force is zero and the change in velocity is zero.
## [[Euclidean Transformations#Rotations|Rotational]] [[Newton's Second Law#Motion|Motion]]
Newton's first law also applies to [[Statics Analysis#Moments (i.e. Torque)|moments]] and rotational velocities.
	A body will maintain it's current rotational velocity until a net moment is exerted to change that rotational velocity.
		 This can be seen in things like toy tops, flywheels, stationary bikes, and other objects that will continue spinning once started until brakes or friction stop them.