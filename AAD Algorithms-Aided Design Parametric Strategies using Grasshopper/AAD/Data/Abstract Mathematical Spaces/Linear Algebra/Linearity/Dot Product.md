# Dot Product
The dot product (also known as the scalar product) of two vectors results in a **scalar**, not a vector. However, the expression of the dot product can still be broken down in vector notation. Here's how it looks:

Given two vectors:
$$
\LARGE \mathbf{a} = [a_1, a_2, a_3] \quad \text{and} \quad \mathbf{b} = [b_1, b_2, b_3]
$$

The dot product is defined as:
$$
\LARGE \mathbf{a} \cdot \mathbf{b} = a_1 b_1 + a_2 b_2 + a_3 b_3
$$

In terms of vector components, if the vectors are in **3-dimensional space**, the dot product formula looks like:
$$
\LARGE \mathbf{a} \cdot \mathbf{b} = \sum_{i=1}^{3} a_i b_i
$$

In a more generalized form for **n-dimensional vectors**:
$$
\LARGE \mathbf{a} \cdot \mathbf{b} = \sum_{i=1}^{n} a_i b_i
$$
## Projections
In geometry and linear algebra, "projecting onto" a vector means that you are essentially "casting a shadow" of one vector onto another, or finding the component of one vector that lies along the direction of the other.
### What Does "Project Onto" Mean?
**Projection** in the context of vectors means "dropping" or "casting" one vector onto another as if you were shining a light perpendicular to the direction of the target vector.
	The shadow that the original vector "casts" onto the target vector is what we call the projection.
		When you **project** a vector $\vec{v}$ onto another vector $\vec{u}$, you are essentially finding the portion of $\vec{v}$ that lies along the direction of $\vec{u}$.
#### Visualizing the Projection as an Overlay
Think of **projection** as if you were shining a light onto v⃗\vec{v}v in such a way that the light is perpendicular to the vector n⃗\vec{n}n. 
	The shadow that v⃗\vec{v}v casts on the line in the direction of n⃗\vec{n}n is the **projection**.
		The projection is **literally the point on the line along n⃗\vec{n}n** that corresponds to the "drop-down" of v⃗\vec{v}v onto n⃗\vec{n}n.
			 In this sense, the projection "lays over" or "falls onto" the line defined by n⃗\vec{n}n.

### Step-by-Step: How to Project One Vector onto Another
- Suppose we have two vectors in 2D: v⃗=[x,y]\vec{v} = [x, y]v=[x,y] and n⃗=[a,b]\vec{n} = [a, b]n=[a,b].
- The **projection** of v⃗\vec{v}v onto n⃗\vec{n}n involves two steps:
    1. **Finding Alignment:** The first step is to calculate how much v⃗\vec{v}v "aligns" with n⃗\vec{n}n. This alignment is quantified by the **dot product**: n⃗⋅v⃗=a⋅x+b⋅y.\vec{n} \cdot \vec{v} = a \cdot x + b \cdot y.n⋅v=a⋅x+b⋅y. The dot product gives a scalar that tells you the "extent" to which v⃗\vec{v}v points in the direction of n⃗\vec{n}n.
    2. **Scaling to Find the Projection:** To get the actual projection vector, you scale the direction of n⃗\vec{n}n by this alignment. This gives you a new vector that lies directly **on** the line defined by n⃗\vec{n}n: Projn⃗v⃗=(n⃗⋅v⃗∥n⃗∥2)n⃗.\text{Proj}_{\vec{n}} \vec{v} = \left(\frac{\vec{n} \cdot \vec{v}}{\|\vec{n}\|^2}\right) \vec{n}.Projn​v=(∥n∥2n⋅v​)n. Here, n⃗⋅v⃗∥n⃗∥2\frac{\vec{n} \cdot \vec{v}}{\|\vec{n}\|^2}∥n∥2n⋅v​ is the scalar that scales the vector n⃗\vec{n}n to match the "shadow" cast by v⃗\vec{v}v.

### Geometric Interpretation
The dot product can also be expressed in terms of the magnitudes of the vectors and the cosine of the angle $\theta$ between them:
$$\LARGE 
\mathbf{a} \cdot \mathbf{b} = |\mathbf{a}| |\mathbf{b}| \cos \theta
$$
Where 
- $|\mathbf{a}|$ and $|\mathbf{b}|$ are the magnitudes (lengths) of vectors $\mathbf{a}$ and $\mathbf{b}$.
- $\LARGE \theta$ is the angle between them.
- $\LARGE \|\vec{a}\| \cos \theta$ represents the **length of the projection** of $\vec{b}$ onto the direction of $\vec{v}$.
	- Therefore, the dot product measures how much one vector "projects" onto another, scaled by the magnitude of the other vector.

This expression represents the **length of the projection** of $\vec{v}$ onto $\vec{u}$.
	Therefore, the dot product measures how much one vector "projects" onto another, scaled by the magnitude of the other vector.
### Projections of the Standard Form Line Equation $ax+by=c$
$$\LARGE ax+by=c.$$
Where:
	- $a,b$, and $c$ are constants or coefficients that determine the orientation of the line in the 2D space.
	- $(x,y)$ are coordinates in the 2D plane.
	- **$c$:** This constant shifts the line's position relative to the origin.

Here:
- $[a, b]$ is the **normal vector** to the line.
- $(x,y)$ is the coordinate of any point on the line, and can be seen as a [[[Points as Vectors#Position Vectors, $ vec{r}$, are Cartesian Vectors|position vector]], $\vec{r}$.
#### The Normal Vector $[a,b]$
The Normal Vector is a vector that is **perpendicular** to the line.
	Its components $a$ and $b$ describe its direction in the coordinate plane.

Exists for every point on the line, and the constant $c$ in the line equation $ax+by=c$ is related to the line's perpendicular distance from the origin. 
	This vector is constant for the entire line—it does not change for different points on the line.

In the standard form equation of a line the coefficients $a$ and $b$ together define the direction of this normal vector.
	Since the normal vector is perpendicular to the line, it provides the orientation of the line in the 2D plane.
		For any point $(x,y)$ on the line, the normal vector $[a,b]$ is the same.
			 It specifies the direction that is orthogonal (perpendicular) to the line, irrespective of where you are on the line.
###### Origin of the Normal Vector
By convention, we visualize the normal vector as **originating from the origin** $(0,0)$. 
	It points in the direction specified by the components $a$ and $b$, but **its location is independent of the line itself**.
		 This vector serves to define the line's orientation (i.e., the direction perpendicular to the line).
###### Length of the Normal Vector
The length (magnitude) of the normal vector is $\LARGE \sqrt{a^2 + b^2}$​.
	This length is used to normalize distances in some geometric calculations, such as finding the perpendicular distance of the line from the origin.
#### [[Line as a Set of Position Vectors|A Line as a Set of Position Vectors]]
A **position vector** $\vec{r} = x \hat{i} + y \hat{j}$ represents a point $(x,y)$ on the line.
	It originates at the origin and points to the location $(x,y)$ in the coordinate system.

Consider **every point** $(x,y)$ on the line as being represented by a **[[#Position Vectors, $ vec{r}$, are Cartesian Vectors|position vector]]**:
$$\LARGE \vec{r} = x \hat{i} + y \hat{j}$$
The line equation $ax+by=c$ tells us that for all position vectors $\vec{r}$ on the line, the dot product with the normal vector $\vec{n} = a \hat{i} + b \hat{j}$ is constant:
$$\LARGE \vec{n} \cdot \vec{r} = c$$
- This means that the projection of any point $\vec{r}$ onto the normal vector $\vec{n}$ is fixed, implying that all such points lie on a line orthogonal to $\vec{n}$.
###### Origin of the Position Vector of a Point (on a line)
Just like the normal vector, the position vector is drawn **from the origin** to the point on the line. 
	This is a standard way to represent points in vector analysis.
		 The vector $[x,y]$ gives the coordinates of the point in relation to the origin.
### The Standard Form of a Line as a Dot Product
A line $ax+by =c$ as a set of position vectors that have a perpendicular distance from origin along the normal vector that is given by c over the magnitude of the normal vector.

The line equation $ax+by=c$ tells us that for every point on the line, the projection of the position vector $[x,y]$ onto the normal vector $[a,b]$ is a constant $c$.

The left-hand side of the standard form equation of a line can be rewritten using the **dot product**:
$$\LARGE \mathbf{n} \cdot \mathbf{r} = n_1 r_1 + n_2 r_2 + n_3 r_3$$
$$\LARGE \vec{n} = [a, b] \quad \text{and} \quad \vec{r} = [x, y]$$
$$\LARGE [a, b] \cdot [x, y] = ax + by$$
$$\LARGE \text{Because $ax+ by =c$}, \quad \vec{n} \cdot \vec{r} = [a, b] \cdot [x, y] = c$$
This expression represents the **projection** of the vector $[x,y]$ onto the normal vector $[a,b]$.
	The line equation $ax+by=c$ states that, for all points $(x,y)$ on the line, this projection is **constant** and equal to $c$.

The normal vector $[a,b]$ is **perpendicular** to the line. 
	The dot product $[a,b] \cdot [x,y]$ measures how much the vector $[x,y]$ aligns with (or projects onto) this normal vector.
#### A Scalar is Produced
This is a scalar value:
$$\LARGE \text{Because $ax+ by =c \quad$ and $ \quad \vec{n} \cdot \vec{r} = [a, b] \cdot [x, y] = ax + by$}$$
$$\LARGE \text{Then, $\quad \vec{n} \cdot \vec{r} = [a, b] \cdot [x, y] = c$}$$
$$\LARGE \text{Where $c$ is a scalar value}$$
The scalar is produced because the **dot product** is designed to extract the magnitude of one vector's projection onto another vector.
	The line equation then specifies that this projection has a constant value, $c$, for every point on the line.

For any point $(x,y)$ in the plane, the projection of the vector $[x,y]$ onto $[a,b]$ gives you a scalar.
	 The line equation $ax+by=c$ tells us that this scalar is constant for every point on the line.
		  This is why the normal vector $[a,b]$ is so important—it defines the line's orientation and the "fixed" nature of the projection that characterizes the line.

The equation $ax+by=c$ sets this projection to a fixed value, $c$. 
	This fixed value means that **every point** $(x,y)$ that lies on the line **has the same "amount" of projection in the direction of the normal vector $[a,b]$**.
		In other words, if you take any point $(x,y)$ on the line, project it onto the normal vector, and measure this projection's length, it will always equal $c$.

This is a measurement of how much of the position vector $\vec{r} = \begin{bmatrix} x \\ y \end{bmatrix}$ "aligns" with the normal vector $\vec{n}$.
	The constant $c$ determines at what point along this normal direction the line crosses.

When we perform the dot product $a \cdot x + b \cdot y$, what we're doing is measuring **how much** of the vector $[x,y]$ lies in the direction of the vector $[a, b]$.
	The **dot product** operation combines the coordinates of $[x,y]$ with the coordinates of $[a,b]$ to produce a single number, $c$ reflecting this "amount" of projection.
		This implies that for every point $(x,y)$ on the line, this projection is **constant** (equal to $c$).
#### What $c$ Represents Geometrically
$\LARGE c$ is a **scalar distance along the normal vector** that determines the **perpendicular distance**of the line.
	I.e. How far the line is positioned from the origin as measured along this Normal Vector. 
		Since the normal vector $[a,b]$ originates from the origin, $c$ can be seen as controlling the line's **offset** along the direction of this normal vector.

When we say the line "projects" onto the normal vector, we mean that the entire line is positioned in such a way that if you were to "drop a perpendicular" from every point on the line to the direction of the normal vector, the distance measured would be proportional to $c$.
	This "projection" is why $c$ acts as a measure of the **perpendicular distance** from the origin to the line:

The constant $c$ determines **where** this line is positioned relative to the origin $(0,0)$ and the direction defined by the normal vector.
	The value $c$ tells us how far along this direction the line is from the origin.
		This means the line is positioned such that every point on it maintains a fixed perpendicular distance from the origin, as dictated by the value of $c$.
##### Visualizing the Projection and $c$
Imagine that the normal vector starts at the origin and points outwards. 
	The line $ax+by=c$ **is positioned somewhere *along* this normal direction**.

Imagine you have the normal vector $[a,b]$ originating from the origin, as an arrow pointing perpendicular to the line.
	If you "walk" along the line, the normal vector always points in the same direction, indicating the orientation of the line in the plane.
		The value of $c$ effectively "shifts" the line along the direction of the normal vector.
			 A larger $|c|$ moves the line further away from the origin, while a smaller $∣c∣$ brings it closer.
###### Distance Interpretation
The constant $c$ **specifies how far the line is from the origin** along the direction of the normal vector.
	It does **not** represent a physical point but rather a scalar that determines the line’s position relative to the origin.

The value of $c$ is related to the **perpendicular distance** of the line from the origin.
	Specifically, the **distance** $d$ from the origin to the line $ax+by=c$ is: 
$$\LARGE d = \frac{|c|}{\sqrt{a^2 + b^2}}$$
Where: 
- The term $\sqrt{a^2 + b^2}$​ is the length (or magnitude) of the normal vector $[a,b]$.
- The ratio $\LARGE \frac{|c|}{\sqrt{a^2 + b^2}}$​ normalizes $c$ by the length of the normal vector to get the actual perpendicular distance from the origin to the line.
###### Direction of the Normal Vector 
If you draw the normal vector $[a,b]$ starting from the origin, the line $ax+by=c$ will be positioned at a perpendicular distance $d$ from the origin, along the direction of this normal vector.
### Slope of a Line and the Normal Vector
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
#### The Direction Vector of a Line, (i.e. the negation of a one component of the Normal Vector), $\LARGE [b,−a]$ or $\LARGE [-b, a]$
The vector $[b,−a]$ is perpendicular to $[a,b]$ because their dot product equals zero:
$$\LARGE [a, b] \cdot [b, -a] = ab - ab = 0$$
This confirms that $[b,−a]$ is indeed a direction vector along the line.

The direction vector $[b,−a]$ **represents how you move along the line**.
The line’s direction vector, is tangent to the line:
	It points in the **direction of the line**, meaning the vector indicates the line's slope or direction of travel).
		The Direction Vector is therefore **perpendicular** to the normal vector just is the line itself.
			If $[a,b]$ is the normal vector, a direction vector $\LARGE \vec{d}$ for the line can be given by swapping and negating one of the components:
				$\LARGE [b,−a]$ or $\LARGE [-b, a]$ Either of these vectors points along the line.

For the direction vector $[b,−a]$:
- The **change in $y$** corresponds to $−a$ (the second component).
- The **change in $x$** corresponds to $b$ (the first component).

The ratio of these changes gives the slope: 
$$\LARGE m = \frac{\text{change in } y}{\text{change in } x} = \frac{-a}{b}.$$
##### Connecting the Scaling to the Direction Vector
In the standard form, $ax+by=c$, the coefficients $a$ and $b$ scale the $x$ and $y$ terms to define the line's orientation.
	These coefficients determine **how steep** the line is and thus influence the direction vector.
##### Scaling and the Direction Vector
Since the line’s direction vector is $[b,−a]$, the coefficients $a$ and $b$ directly dictate the **ratio** of change between $x$ and $y$ as you move along the line:
    If you increase the scalar $x$ by some amount $\LARGE \Delta x = b$, the corresponding change in $y$ would be $\LARGE \Delta y = -a$.
##### Direction Vector as a Reflection of Scaling
The direction vector $[b,−a]$ captures how much you move in the $x$ and $y$ directions relative to each other, based on the line’s orientation given by the normal vector $[a,b]$.
	Thus, the coefficients $a$ and $b$ inherently encode the "steepness" of the line:
	    The slope of the line is $\LARGE -\frac{a}{b}$​, which comes directly from the ratio of the components in the direction vector $[b,−a]$.
##### Direction Vector as a Reflection of the Influence of the Normal Vector's Components
$$\LARGE ax +by = c$$
$$\LARGE \vec{d} = [b, -a], \quad \vec{n} = [a, b], \quad m = \frac{-a}{b} =  \frac{\Delta y}{\Delta x}$$
$$\LARGE \text{Where }\quad \vec{d}= b\hat{i} + -a \hat{j} \quad \vec{n}= a\hat{i} + b \hat{j}$$
###### Influence of $b$ Component
As it is associated with $y$ in the normal vector, it becomes the change in $x$ in the direction vector.
###### Influence of $−a$ Component
As it is associated with $x$ in the normal vector, it becomes the change in $y$ in the direction vector.
##### The Direction Vector and the Slope
A direction vector $[b,−a]$ describes the direction in which the line runs.
	The components of this vector show how far you move horizontally ($x$-axis) and vertically ($y$-axis) as you traverse the line. 
		The ratio of these movements ($\LARGE \frac{\Delta y}{\Delta x} = -\frac{a}{b}$​) is precisely the line's slope.
##### Why the Direction Vector Encodes the Slope
The line's slope tells you how steep the line is, which means how much it rises or falls as you move horizontally.
	The direction vector $[b,−a]$ provides this directional information:
	    If you were to move along the direction vector from one point on the line to another, you would be following the line's slope.
		    The direction vector's components directly reflect the line's change in $y$ relative to a change in $x$, thus encoding the slope.
#### Fundamental Geometric Insight
The **normal vector** $[a,b]$ provides the direction that is perpendicular to the line. 
	The **slope** $\LARGE -\frac{a}{b}$ is a manifestation of this perpendicular relationship. It indicates how the line "falls off" relative to the x-axis as you move along it.
		The relationship between the normal vector and the slope is geometric: the normal vector's components $a$ and $b$ give the "rise" and "run" of a vector that is **orthogonal** to the line's direction.
			Inversely, knowing the slope $m$ gives information about the direction of the normal vector.
				 If the slope of a line is $m$, the normal vector can be constructed as $[m,−1]$ or any scalar multiple of this vector, such as $\LARGE [a, b] = [-b, a]$