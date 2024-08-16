# Planes
The functions that produce planes, are themselves solution sets, and each solution of the set is contained within the produced plane.
## Planes in the Space ($\mathbb{R}^3$)
### Normal Equation of a Plane
![[Pasted image 20240810055336.png]]
$$\LARGE ax + by + cz + d = 0$$
This function describes the solution set to the function which produces a plane.
	A plane $\LARGE \pi$ requires an initial point $\LARGE x_0=(x_0,y_0,z_0)$, a [[Partial Derivatives#Normal Vector to a 3D Surface|Normal Vector]] $\LARGE \vec{n}=(a,b,c)$ to the plane, and a terminating point $\LARGE x_0=(x_0,y_0,z_0)$ on the plane which combines with the initial point to form a perpendicular vector $\LARGE \mathbf{x}-\mathbf{x_0} = (x-x_0, y-y_0,z-z_0)$ (i.e. a vector on the plane itself).

The Normal Equation of the plane, $\LARGE \pi$ through $\LARGE x_0 = (x_0, y_0, z_0)$ and orthogonal to the vector $\LARGE \mathbf{n} = (a,b,c)$:
	$\LARGE a, b,c, d$ are all constants.
		These constants are the values of the calculated **partial derivatives** of a given point.
			$\LARGE x,y,z$ are all variables, i.e. the position values of the point. 
$$\LARGE ax + by + cz + d = 0$$
$$\LARGE \text{Where } \textcolor{red}{d = -ax_0 - by_0 - cz_0}$$
#### The Reasoning of the Normal Equation
If a point $\LARGE x_0=(x_0,y_0,z_0)$ belongs to the plane $\LARGE \pi$ then the vectors $\LARGE \vec{n}=(a,b,c)$ and $\LARGE \mathbf{x}-\mathbf{x_0} = (x-x_0, y-y_0,z-z_0)$ must be orthogonal.
	This means the [[Dot Product|dot product]] between the two vectors must be produce $\LARGE 0$.
		Where $\LARGE \textcolor{red}{d}$ contains the remaining terms that equate the equation to the dot product between the two vectors.
		
$$\LARGE (a,b,c) \cdot (x-x_0, y-y_0,z-z_0) = 0$$
$$\LARGE  \iff$$
$$\LARGE  ax\textcolor{red}{-ax_0} + by\textcolor{red}{-by_0}+cz-\textcolor{red}{cz_0} = 0$$
$$\LARGE  \iff$$
$$\LARGE ax+by+cz+\textcolor{red}{d} = 0$$
### Point Vector Form of a Plane (i.e. Parametric Equation)
![[Pasted image 20240815060854.png]]
A Parametric equation that utilizes a two parameters $\LARGE t,s \in \mathbb{R}$.
	Where any point on the line $\LARGE \mathbf{x}$ can be described as a Linear Combination of the initial point $\LARGE x_0$ and the parameters $\LARGE t, s$ [[Scaling|scaling]] the [[Partial Derivatives#Direction Vector in the Plane $y = b$|Direction Vectors]] $\LARGE \vec{v} = (v_1, v_2)$ and $\LARGE \vec{u} = (u_1, u_2)$ that generate the plane.
		*Remember that any pair of linearly independent functions generate a plane and can thus access any point on that plane.*
$$\LARGE \mathbf{x} = x_0 + t\vec{v} +s\vec{u}, \quad t,s \in \mathbb{R}$$
#### Point Vector Form "Coordinate-Wise"
This form describes the same Point Vector Form equation, but substitutes the coordinates of a point and vector with the corresponding variables.
$$\LARGE (x,y,z) = (x_0,y_0,z_0) + t(v_1,v_2,v_3) + s(u_1,u_2,u_3), \quad t,s \in \mathbb{R}$$
##### Coordinate-Wise in Three Rows
A Linear System of Equations that gives the coordinates of any point on the plane, $\LARGE pi$.
	One **row** for each coordinate. 
$$\LARGE \pi:\begin{Bmatrix} x = x_0 + v_1t + u_1s \\ y = y_0 + v_2t + u_2s \\ z = z_0 + v_3t + u_3s \end{Bmatrix}, \quad t,s \in \mathbb{R}$$