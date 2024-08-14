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
$$\LARGE (a,b,c) \cdot (x-x_0, y-y_0,z-z_0) = 0$$
$$\LARGE  \iff$$
$$\LARGE  ax\textcolor{red}{-ax_0} + by\textcolor{red}{-by_0}+cz-\textcolor{red}{cz_0} = 0$$
$$\LARGE  \iff$$
$$\LARGE ax+by+cz+\textcolor{red}{d} = 0$$