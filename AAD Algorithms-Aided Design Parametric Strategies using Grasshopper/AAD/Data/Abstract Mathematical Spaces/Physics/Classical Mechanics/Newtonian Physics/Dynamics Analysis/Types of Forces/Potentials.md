# Potentials
## Potential Function, $U(r)$
In classical mechanics, the potential function $U(r)$ is related to the force $F(r)$ through the negative gradient of the potential. 
	Is **not** a Vector, but is a [[Mapping#Scalar Functions as a Subset of Functions|Scalar Function]] of a [[Data/Abstract Mathematical Spaces/Physics/Classical Mechanics/Newtonian Physics/Kinematics Analysis/Components of Motion#Position|position]], that has a (negative) gradient gives rise to the force as a scalar.
		This relationship between the Force and the Potential is given by the equation:
$$\LARGE F(r) = -\nabla U(r) =-\left( \frac{\partial U}{\partial x}, \frac{\partial U}{\partial y}, \frac{\partial U}{\partial z} \right) =  -\frac{dU(z)}{dz}$$
Where:
	The functon $U(r)$ is indirectly defined - that is - it must be "found" from the Force. 
		I.e. Set the two equations for force equal to each other. 
	And the [[Data/Abstract Mathematical Spaces/Physics/Analysis/Multivariable Calculus/Gradients#*Note Nabla Operator ($ nabla$)*|nabla]] represents a [[Data/Abstract Mathematical Spaces/Physics/Analysis/Multivariable Calculus/Gradients|gradient]].
	This nabla is defined on the $U(r)$ function.
		Therefore, it is the gradient of $U(r)$.
### How to Find the Potential ($U(r)$)
##### Need the Position to Calculate the Potential

##### 1. Start with the Force Function
Suppose you have a force function $F(r)$. 
	For simplicity, let's consider a one-dimensional case where the force is a function of $x$, denoted as $F(x)$.
##### 2. Integrate the Force Function (as instructed by the nabla)
The potential energy function $U(x)$ is obtained by integrating the force function with respect to the position variable $x$:
$$\LARGE F(x) = -\nabla U(x) = -\int F(x) \, dx$$
## Potential Energy, $U(r)$
The potential energy $U(r)$ represents the energy associated with the position of an object in a force field, and it is a scalar function. 
	The force $F(r)$ is then derived from this potential energy as the spatial rate of change (gradient) of the potential energy, with a negative sign indicating that the force acts in the direction of decreasing potential energy.
### Potential Energy for Force of Gravity of an Object
$$\LARGE U(r) = mgz$$
Here, $m$ is the mass of the object, $g$ is the acceleration due to gravity, and $z$ is the height above a reference point (typically the Earth's surface). 
	This expression for potential energy assumes a uniform gravitational field, which is a good approximation near the Earth's surface.
		The Potential that corresponds to the Force of Gravity for an object.
			The gradient of $mgz$, has [[Data/Abstract Mathematical Spaces/Physics/Analysis/Multivariable Calculus/Partial Derivatives|partial derivative]] of 0 for the $x$, and $y$.
#### Deriving the Potential Energy of Gravity
Let's go through the derivation of the potential energy function $U(z)$ for the simplified case where the gravitational force is given by $F = mg$. This is typically used near the Earth's surface where the gravitational field is approximately uniform.

1. **Start with the Force Function**:
   The gravitational force near the Earth's surface is:
$$F = -mg$$
   Here, $m$ is the mass of the object, $g$ is the acceleration due to gravity, and the negative sign indicates that the force is directed downward.

2. **Relate the Force to the Potential Energy**:
   $$F_r = -\nabla U(r)$$
    Set the two expressions for the force equal to each other:
	    In this case, since $F = -mg$, we have:
$$\LARGE F= -mg = -\frac{dU(z)}{dz}$$
   The relationship between the force $F$ and the potential energy $U$ is given by:
$$\LARGE F = -\frac{dU(z)}{dz} = -\left( \frac{\partial U}{\partial x}, \frac{\partial U}{\partial y}, \frac{\partial U}{\partial z} \right) = -(0, 0, mg)$$
3. **Integrate the Force to Find the Potential Energy**:
   To find $U(z)$, integrate both sides with respect to $z$:
	   Remove the negative signs (they cancel each other out):
$$-mg = -\frac{dU}{dz}$$​
$$\LARGE = mg = \frac{dU(z)}{dz}$$
   Integrating both sides:
$$\LARGE U(z) = \int mg \, dz$$
4. **Perform the Integration**:
   The integral of a constant $mg$ with respect to $z$ is:
$$\LARGE U(z) = mgz + C$$
   
   Here, $C$ is the constant of integration.

5. **Determine the Constant of Integration**:
   The constant $C$ is typically chosen based on a reference point. 
	   For gravitational potential energy near the Earth's surface, we often set the potential energy to be zero at $z = 0$. 
		   Therefore, $C = 0$.
			   So, we have:
$$\LARGE U(z) = mgz$$
The potential energy $U(z)$ for an object of mass $m$ at a height $z$ near the Earth's surface is:

### Potential Energy for Force of Gravity of an Object on Inclined Plane
$$\LARGE \text{Resultant Force, } F_H = mg\sin(\alpha)e_s$$
The potential energy function $U(s)$ for an object on an inclined plane where the resultant force is given by:
$$
F_H = mg\sin(\alpha)e_s
$$
Where:
	$\alpha$ is the angle of inclination, and $e_s$ is the unit vector along the inclined plane.
##### 1. Understand the Force Function
The component of gravitational force acting parallel to the inclined plane is:

$$
F_H = mg\sin(\alpha)
$$

where:
- $m$ is the mass of the object,
- $g$ is the acceleration due to gravity,
- $\alpha$ is the angle of the inclined plane,
- $F_H$ is the force component along the plane.
##### 2. Relate Force to Potential Energy
The relationship between the force $F_H$ and the potential energy $U(s)$ along the plane is given by:

$$
F_H = -\frac{dU(s)}{ds}
$$

Here, $s$ is the distance along the inclined plane.
##### 3. Set Up the Equation
Set Force Equations Equal
$$\LARGE F_H = mg\sin(\alpha)e_s = -\frac{dU(s)}{ds}$$

$$
mg\sin(\alpha) = -\frac{dU(s)}{ds}
$$

##### 4. Integrate to Find the Potential Energy
Integrate both sides with respect to $s$ to find $U(s)$:

$$
-\int mg\sin(\alpha) \, ds = \int \frac{dU(s)}{ds} \, ds
$$

This simplifies to:

$$
-mg\sin(\alpha) \int ds = \int dU(s)
$$

##### 5. Perform the Integration

Since $mg\sin(\alpha)$ is a constant with respect to $s$:

$$
-mg\sin(\alpha) s = U(s) + C
$$

Rearranging to solve for $U(s)$:

$$
U(s) = -mg\sin(\alpha) s + C
$$

##### 6. Determine the Constant of Integration
The constant $C$ is typically chosen based on a reference point. We can set the potential energy to be zero at a specific point along the inclined plane. For simplicity, let's choose $s = 0$ as our reference point:

$$
U(0) = 0
$$

Substitute $s = 0$ into the potential energy equation:

$$
0 = -mg\sin(\alpha) \cdot 0 + C
$$

So, $C = 0$.
##### Final Potential Energy Function

Thus, the potential energy function $U(s)$ for an object on an inclined plane is:

$$
U(s) = -mg\sin(\alpha) s
$$

### Potential Energy for Universal Force of Gravity (of an Object)


$$\LARGE \text{Univ. Law of Gravity, } F_g = \pm \gamma \frac{m_1m_2}{r_{12}^2}e_{12}$$

