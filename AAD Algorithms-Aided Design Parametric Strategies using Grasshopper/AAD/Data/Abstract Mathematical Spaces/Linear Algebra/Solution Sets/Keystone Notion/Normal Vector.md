# Normal Vector $[a,b]$
See [[Data/Abstract Mathematical Spaces/Linear Algebra/Linearity/Dot Product#Projections of the Standard Form Line Equation $ax+by=c$|Dot Product]]

The Normal Vector is a vector that is **perpendicular** to the line.
	Its components $a$ and $b$ describe its direction in the coordinate plane.

Exists for every point on the line, and the constant $c$ in the line equation $ax+by=c$ is related to the line's perpendicular distance from the origin. 
	This vector is constant for the entire line—it does not change for different points on the line.

In the standard form equation of a line the coefficients $a$ and $b$ together define the direction of this normal vector.
	Since the normal vector is perpendicular to the line, it provides the orientation of the line in the 2D plane.
		For any point $(x,y)$ on the line, the normal vector $[a,b]$ is the same.
			 It specifies the direction that is orthogonal (perpendicular) to the line, irrespective of where you are on the line.
##### Origin of the Normal Vector
By convention, we visualize the normal vector as **originating from the origin** $(0,0)$. 
	It points in the direction specified by the components $a$ and $b$, but **its location is independent of the line itself**.
		 This vector serves to define the line's orientation (i.e., the direction perpendicular to the line).
##### Length of the Normal Vector
The length (magnitude) of the normal vector is $\LARGE \sqrt{a^2 + b^2}$​.
	This length is used to normalize distances in some geometric calculations, such as finding the perpendicular distance of the line from the origin.
##### Direction of the Normal Vector 
If you draw the normal vector $[a,b]$ starting from the origin, the line $ax+by=c$ will be positioned at a perpendicular distance $d$ from the origin, along the direction of this normal vector.

- - -
## Slope of a Line and the Normal Vector
The slope $\LARGE -\frac{a}{b}$​ arises from the **ratio** of the components of the normal vector. 
	This ratio determines how the line behaves in space.
		If the normal vector $[a,b]$ changes direction (i.e., if the values of $a$ and $b$ change), the slope of the line changes accordingly.
#### The Slope
In Standard Form, $a,b$ identify how much $x,y$ have been scaled by.
- $a$: Determines how much the $x$-component is scaled.
- $b$: Determines how much the $y$-component is scaled.

The coefficients $a$ and $b$ also define the **normal vector** $[a,b]$.
	This vector points in the direction **perpendicular** to the line.
$$\LARGE ax +by = c \quad \to \quad by=−ax+c$$
$$\LARGE \equiv y = -\frac{a}{b}x + \frac{c}{d}$$
$$\LARGE \text{Where, } \quad m = -\frac{a}{b}$$
The slope $\LARGE m = -\frac{a}{b}$​ represents the **ratio** of the change in $y$ to the change in $x$ for the direction along the line.
	This ratio is essentially describing how steep the line is.
		It tells us that for every unit of change in the $x$-direction, the line changes $\LARGE -\frac{a}{b}$ units in the $y$-direction.

This ratio is fundamental because it expresses the **directionality** of the line. 
	The normal vector $[a,b]$ dictates the line’s orientation, while the slope $-\frac{a}{b}$​ describes how the line rises or falls as you move along the $x$-axis.