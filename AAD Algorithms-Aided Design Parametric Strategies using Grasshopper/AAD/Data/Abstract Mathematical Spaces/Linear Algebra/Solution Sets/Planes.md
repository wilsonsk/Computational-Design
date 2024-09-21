# Planes
The functions that produce planes, are themselves solution sets, and each solution of the set is contained within the produced plane.
## Planes in the Space ($\mathbb{R}^3$)
### Normal [[Equations as Constraints|Equation]] of a Plane
The Normal Equation of the plane, $\LARGE \pi$ relates a Vector on the Plane $\LARGE \vec{x}$ (from a starting point $\LARGE x = (x, y, z)$ through $\LARGE x_0 = (x_0, y_0, z_0)$) and a Normal Vector $\LARGE \mathbf{n} = (a,b,c)$   orthogonal to the vector $\LARGE \vec{x}$ and the plane $\LARGE \pi$.

![[Pasted image 20240810055336.png]]
$$\LARGE ax + by + cz + d = 0$$
This function describes the solution set to the function which produces a plane.
	A plane $\LARGE \pi$ requires an initial point $\LARGE x_0=(x_0,y_0,z_0)$, a [[Partial Derivatives#Normal Vector to a 3D Surface|Normal Vector]] $\LARGE \vec{n}=(a,b,c)$ to the plane, and a terminating point $\LARGE x_0=(x_0,y_0,z_0)$ on the plane which combines with the initial point to form a perpendicular vector $\LARGE \mathbf{x}-\mathbf{x_0} = (x-x_0, y-y_0,z-z_0)$ (i.e. a vector on the plane itself).

The Normal Equation of the plane, $\LARGE \pi$ through $\LARGE x_0 = (x_0, y_0, z_0)$ and orthogonal to the vector $\LARGE \mathbf{n} = (a,b,c)$:
	$\LARGE \textcolor{green}{a, b,c}$ are all constants.
		These constants are the values of the calculated **partial derivatives** of a given point.
			$\LARGE \textcolor{red}{x,y,z}$ are all variables, i.e. the position values of the point. 
$$\LARGE \textcolor{green}{a}\textcolor{red}{x} + \textcolor{green}{b}\textcolor{red}{y} + \textcolor{green}{c}\textcolor{red}{z} + \textcolor{yellow}{d} = 0$$
$$\LARGE \text{Where } \textcolor{yellow}{d = -ax_0 - by_0 - cz_0}$$
$\LARGE d$ can be seen as the origin point of the normal vector $\LARGE \vec{n}$ and the vector on the plane $\LARGE \mathbf{x}-\mathbf{x_0}$. 
#### The Reasoning of the Normal Equation
If a point $\LARGE x_0=(x_0,y_0,z_0)$ belongs to the plane $\LARGE \pi$ then the vectors $\LARGE \vec{n}=(a,b,c)$ and $\LARGE \mathbf{x}-\mathbf{x_0} = (x-x_0, y-y_0,z-z_0)$ must be orthogonal.
	This means the [[Dot Product|dot product]] between the two vectors must be produce $\LARGE 0$.
		Where $\LARGE \textcolor{red}{d}$ contains the remaining terms that equate the equation to the dot product between the two vectors.
		
$$\LARGE (\textcolor{green}{a,b,c}) \cdot (\textcolor{red}{x}-x_0, \textcolor{red}{y} - y_0, \textcolor{red}{z}- z_0) = 0$$
$$\LARGE  \iff$$
$$\LARGE \textcolor{green}{a}\textcolor{red}{x}-\textcolor{yellow}{ax_0}+\textcolor{green}{b}\textcolor{red}{y}-\textcolor{yellow}{by_0} +\textcolor{green}{c}\textcolor{red}{z}-\textcolor{yellow}{cz_0}={0}$$
$$\LARGE  \iff$$
$$\LARGE \textcolor{green}{a}\textcolor{red}{x} +\textcolor{green}{b}\textcolor{red}{y}  +\textcolor{green}{c}\textcolor{red}{z} + \textcolor{yellow}{d}= 0$$
### Example of Deriving the Normal Equation for a Plane
Write the normal equation for the plane orthogonal to $\LARGE n= (-2,3,-5)$ and passing through the point $\LARGE P =(0,1,-3)$. 
#### Method 1: Using the Normal Equation
$$\LARGE Ax+ By+Cz+ D = 0$$
##### 1. Plug in the Scalars From the Normal Vector $\vec{n} = (-2,3,-5)$
$$\LARGE \textcolor{green}{-2}x+ \textcolor{green}{3}y+(\textcolor{green}{-5}z)+ D = 0$$
##### 2. Plug in the Coordinates of the "Origin" Point $P = (0,1,-3)$
$$\LARGE \textcolor{green}{-2}\cdot \textcolor{red}{0}+ \textcolor{green}{3}\cdot \textcolor{red}{1} +(\textcolor{green}{-5}\cdot(\textcolor{red}{-3}))+ D = 0$$
##### 3. Solve for $\LARGE D$
$$\LARGE 18+ D = 0$$
$$\LARGE D = -18$$
### Method 2: Using the Dot Product
##### 1. Compute the Dot Product of the Normal Vector and Any Vector $\vec{Px}$ on the Plane with an "Origin Point" $P = (0,1,-3)$ and End Point $x = (x, y, z)$
$$\LARGE 0 = \vec{n} \cdot \vec{Px}$$
$$\LARGE 0 = (-2,3,-5) \cdot (x,y-1,z+3)$$
$$\LARGE 0 = -2x + 3y - 3 -5z -15$$
$$\LARGE 0 = -2x + 3y -5z -18$$
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
### Example of Deriving the Parametric Equation of a Plane
Find the Parametric Equation for the plane in $\mathbb{R}$^3 that contains the points $P = (1,1,1)$, $Q=(-1,0,1)$ and $R = (5,6,7)$. 
	Check if the following points belong to this plane: $A = (-3,-1,1)$.
##### 1. Identify 2 Vectors between the 3 Points
Any of the three Points can be selected as the Origin Point of the 2 Vectors.
$$\LARGE \vec{PQ} = \vec{u} = \vec{Q} - \vec{P} = (-1,0,1) - (1,1,1) = (-2,-1,0)$$
$$\LARGE \vec{PR} = \vec{v} = \vec{R} - \vec{P} = (5,6,7) - (1,1,1) = (4,5,6)$$
##### 2. Write the Parametric Equation of the Plane
Where any Point on the Plane $\LARGE (x,y,z)$  **equals the starting Point plus the first parameter scaling the first vector plus the second parameter the second vector**.
$$\LARGE (x,y,z) = (x_0,y_0,z_0) + t\vec{u} + s\vec{v}, \quad t,s\in \mathbb{R}$$
$$\LARGE (x,y,z) = (1,1,1) + t(-2,-1,0) + s(4,5,6)$$
##### 3. Describe Each Variable Coordinate-Wise
Plug in the corresponding variables of the origin point and two vectors.
$$\LARGE \pi: \begin{Bmatrix} x = 1 - 2t + 4s \\ y = 1 - 1t + 5s \\ z = 1 + 0t + 6s\end{Bmatrix},$$
Each Column of this matrix is one of the two directional vectors $(\vec{u} = (-2,-1,0), \vec{v} = (4,5,6))$ existing on the Plane.
	Both of which have the origin point $P = (1,1,1)$ that is orthogonal to the plane. 
![[Pasted image 20240818132748.png]]
##### 4. Check if the Following Point Belongs to the Plane: $A = (-3,-1,1)$.
Plug in $\LARGE A$ into the "Any Point on the Plane" $\LARGE (x,y,z)$
	Plug in each solved Parameter.
		If there is a solution then the Point $A$ belongs in the plane.
$$\LARGE \pi: \begin{Bmatrix} -3 = 1 - 2t + 4s =  \textcolor{red}{1 - 2t + 4(0)= -4 = -2t = t =2}\\ -1 = 1 - 1t + 5s = \textcolor{red}{1 - 1(2) + 5(0) = 1-2+ 0 = -1}\\ 1 = 1 + 0t + 6s = \textcolor{red}{s = 0}\end{Bmatrix},$$
The Solution exists and therefore the Point $A$ belongs to this plane.
## Intercept Form
![[Pasted image 20240818115309.png]]
$$\LARGE \frac{x}{a} + \frac{y}{b} + \frac{z}{c} = 1$$
Where $\LARGE a$ is the $\LARGE x$-intercept.
	That is where the plane intersects the $\LARGE x$-axis (i.e. where $\LARGE y,z =0$)
		I.e. Where Plane intersects $\LARGE (a, 0, 0)$

Where $\LARGE b$ is the $\LARGE y$-intercept.
	That is where the plane intersects the $\LARGE y$-axis (i.e. where $\LARGE x,z =0$)
		I.e. Where Plane intersects  $\LARGE (0, b, 0)$

Where $\LARGE c$ is the $\LARGE z$-intercept.
	That is where the plane intersects the $\LARGE z$-axis (i.e. where $\LARGE x,y =0$)
		I.e. Where Plane intersects $\LARGE (0, 0, c)$
![[Pasted image 20240818120303.png]]
Rearranging the equation $\LARGE y=-x+1$:
$$\LARGE 1x + 1y + 0z = 1$$ Which means the coordinates of the $\LARGE \vec{n}= (1,1,0)$, thus no change in the $\LARGE z$-axis.
	Which means the normal vector is perpendicular to the $\LARGE z$-axis.
		Which also means that the normal vector is parallel to the $\LARGE x-y$ plane. 
			Therefore, the normal vector $\LARGE \vec{n}$ is orthogonal to the plane of the function $\LARGE y = -x+1$.
### Example of Deriving the Intercept Form of a Plane
Write the intercept equation for the plane orthogonal to $\LARGE n= (-2,3,-5)$ and passing through the point $\LARGE P =(0,1,-3)$. 
##### 1. Use the Normal Equation to [[#Example of Deriving the Normal Equation for a Plane|Derive Normal Form of the Plane]]
##### 2. Put All Unknowns on One Side and Constants on the other Side
$$\LARGE 2x - 3y + 5z = -18$$
##### 3. Get $1$ on the RHS by Dividing Both Sides of the Equation by $-18$
$$\LARGE \frac{2x}{-18} - \frac{3y}{-18} + \frac{5z}{-18} = \frac{-18}{-18}$$
$$\LARGE = \frac{x}{-9} + \frac{y}{6} + \frac{5}{-18}z = 1$$
$$\LARGE = \frac{x}{-9} + \frac{y}{6} + \frac{z}{-\frac{18}{5}} = 1$$
$$\LARGE = \frac{x}{-9} + \frac{y}{6} + \frac{z}{-3.6} = 1$$

## Converting the Parametric Equation to the Normal Equation
Using the following Parametric Equation, convert to the Normal Equation.
$$\LARGE \pi: \begin{Bmatrix} x = 1 - 2t + 4s \\ y = 1 - 1t + 5s \\ z = 1 + 0t + 6s\end{Bmatrix},$$
*Remember: Each Column of this matrix is one of the two directional vectors $(\vec{u} = (-2,-1,0), \vec{v} = (4,5,6))$ existing on the Plane.
	Both of which have the origin point $P = (1,1,1)$ that is orthogonal to the plane.*
![[Pasted image 20240818132752.png]]
##### 1. Compute the Normal Vector Using the Cross Product
Also remember that the vector that is normal to two vectors, *is* the cross product of the two vectors.

$$\LARGE \vec{n} = \vec{u} \times \vec{v}$$
$$\LARGE \left| \begin{matrix} \vec{i} \quad \quad \vec{j} \quad \quad \vec{k} \\ 1 \quad 0 \quad f_{x}'(a,b) \\ 0 \quad 1 \quad f'_{y}(a,b)\end{matrix} \right| =   = (-f'_{x}(a,b), -f'_{y}(a,b), 1)= \vec{n}$$
$$\LARGE = \vec{n} = \left| \begin{matrix} \vec{i} \quad \quad \vec{j} \quad \quad \vec{k} \\ \quad -2  \quad  -1   \quad 0 \quad \\ 4  \quad \quad 5  \quad \quad 6\end{matrix} \right| = (-6,12,-6)$$
##### 2. Scale the Normal Vector
$$\LARGE \vec{n} = (-6,12, -6) = -\frac{1}{6} \cdot \vec{n} =  (1, -2, 1)$$
##### 3. Convert to the Normal Equation
$$\LARGE \vec{n}=(A,B,C), \quad Ax+By+Cz+D = 0$$
###### Plug in the Variables of the Normal Vector into the Normal Equation
$$\LARGE \vec{n} = (1,-2,1)$$
$$\LARGE (1)x + (-2)y + (1)z + D  = 0$$
###### Solve for $D$ by Plugging in the "Origin Point" of the Directional and Normal Vectors
$$\LARGE P = (1,1,1)$$
$$\LARGE (1)(1) + (-2)(1) + (1)(1) + D = 0$$
$$\LARGE 0 + D = 0$$
$$\LARGE D = 0$$
##### 4. The Normal Equation
$$\LARGE x + (-2)y + z = 0$$

- - -
### The Tangent Plane (to a surface $z = f(x,y)$) Through a Point
*Remember to obtain the coordinates of a vector, take the difference of the terminating point and the origin.*
	The Normal Equation states: if a point $(x,y,z)$ exists on the plane $\pi$, then the [[Dot Product|dot product]] of the normal vector with the vector containing those initial points, is equal to $0$.
		Where $\LARGE \textcolor{red}{d}$ contains the remaining terms that equate the equation to the dot product between the two vectors.
![[Pasted image 20240810060854.png]]
$$\LARGE (\textcolor{red}{x,y,z}) \Leftrightarrow (x-a,y-b,z-\textcolor{green}{f(a,b)}) \cdot (\textcolor{green}{f'_x(a,b), f'_y(a,b)}, -1) = 0$$
$$\LARGE  = \text{ The Dot Product, } \textcolor{green}{f'_x(a,b)}(\textcolor{red}{x}-a) + \textcolor{green}{f'_y(a,b)}(\textcolor{red}{y}-b) - \textcolor{red}{z} + \textcolor{green}{f(a,b)} = 0$$
Where $\textcolor{green}{\text{Green Terms}}$ are the Constants of the Normal Equation.
Where $\textcolor{red}{\text{Red Terms}}$ are the Variable Coordinates of the Point of the Normal Equation. 
#### The Equation of the Tangent Plane is a Rearrangement of the Normal Equation
$$\LARGE \text{Rearranging the Previous Dot Product Equation:}$$
$$\LARGE \textcolor{green}{f'_x(a,b)}(\textcolor{red}{x}-a) + \textcolor{green}{f'_y(a,b)}(\textcolor{red}{y}-b) - (\textcolor{red}{z} + \textcolor{orange}{z}) + \textcolor{green}{f(a,b)} = 0 + \textcolor{orange}{z}$$
#### Tangent Plane to the Surface $z=f(x,y)$ in the point $(a,b,f(a,b))$:
$$\LARGE = \textcolor{red}{z} = \textcolor{green}{f(a,b)} + \textcolor{green}{\frac{\partial f}{\partial x}(a,b)} (\textcolor{red}{x}-a) + \textcolor{green}{\frac{\partial f}{\partial y}(a,b)}(\textcolor{red}{y}-b)$$
*Notice the comparison* between the [[Straight Lines#The Tangent Line Through a Point (on a Curve)|Tangent Line through the Point]] $(a,f(a))$, which resembles the [[Straight Lines#1. Standard Form of a Line|Standard Form of a Line]].
	Where the **partial derivatives** of the tangent plane equation and the **derivative** of the tangent line equation all are the slope $\LARGE m$. 
$$\LARGE \text{Tangent Plane } = \textcolor{red}{z} = \textcolor{green}{f(a,b)} + \textcolor{green}{f'_x(a,b)} (\textcolor{red}{x}-a) + \textcolor{green}{f'_y(a,b)}(\textcolor{red}{y}-b)$$
$$\LARGE \text{Tangent Line} = y = f(a) + f'(a)(x-a)$$
#### The Gradient as the Slope $\LARGE m$
The $1\times 2$ Vector that is composed of the Partial Derivatives for a given point, is itself the [[Gradients|Gradient]] of the function $\LARGE f$ at point $(a,b)$, $\LARGE  \nabla f(a,b) = \begin{bmatrix}(\frac{\partial f}{d x}(a,b),\frac{\partial f}{d y}(a,b)\end{bmatrix}$. 
	I.e. The scalars produced from the evaluated Partial Derivatives, are coordinates of the Gradient at point $(a,b)$. 

And the Increments $(x-a)$ and (y-b), in the $\LARGE x$ and $\LARGE y$ direction, can also be coordinates in some separate column vector (i.e. a $2 \times 1$ vector), $\LARGE \begin{bmatrix} x-a \\ y-b \end{bmatrix}$. 
	Therefore, the Tangent Plane Equation can be reconfigured.
$$\LARGE \text{Tangent Plane } z = f(a,b) + [f'_x(a,b),f'_y(a,b)] \cdot \begin{bmatrix} x-a \\ y-b \end{bmatrix}$$
$$\LARGE == z = f(a,b) + \nabla f(a,b) \cdot \begin{bmatrix} x-a \\ y-b\end{bmatrix}$$
$$\text{Compared to Standard Form of a Line } y = mx +b$$
		Where the two vectors are then arranged to produce the [[Dot Product|Dot Product]] between them. 
			And the result is the that the **Gradient** itself becomes the representation of the slope $\LARGE m$, and  the new $2 \times 1$ vector is the **increment**.  