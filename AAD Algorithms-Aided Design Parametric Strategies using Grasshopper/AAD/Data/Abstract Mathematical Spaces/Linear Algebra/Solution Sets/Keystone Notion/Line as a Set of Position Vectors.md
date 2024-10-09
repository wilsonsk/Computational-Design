---
up:
  - "[[Points as Position Vectors]]"
---
# [[Straight Lines|Line]] as a Set of Position Vectors
Remember that [[Points as Position Vectors|Points are Position Vectors]].
## Representations of a Line
### The Derivation of the Normal Line Equation 
The equation of a line in 2D space is a **formal constraint** that describes a **set of values**, and **geometrically** defines those set of points to lie on a line 2D space.
$$\LARGE ax + by + c= 0$$
The coefficients $a$ and $b$ act as **weights** that combine the standard basis vectors $\hat{i} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}$ and $\hat{j} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}$.


The line itself is all the points $(x,y)$ that satisfy the equation $ax+by=c$.
	The line equation imposes a **linear constraint** on the coordinates $(x,y)$ of points. 
		In vector terms, this constraint defines a **subspace** of the 2D space — specifically, a 1-dimensional line.
#### Origin in Vector Spaces
The standard form of the line equation can be understood as derived from the **[[Data/Abstract Mathematical Spaces/Linear Algebra/Linearity/Dot Product|dot product]]** of vectors. 
	This implies that the line equation is rooted in the geometry of vector spaces.
	    The line equation can be seen as expressing the fact that all points on the line have a **constant projection** onto the normal vector $[a,b]$.
		    This highlights that the line equation is inherently about the relationship between vectors and their directions, i.e., the constraints imposed on a vector's coordinates to lie on a line.

The coefficients $a$ and $b$ act as **weights** that combine the standard basis vectors $\hat{i} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}$ and $\hat{j} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}$.
	This combination defines the line's normal vector $\vec{n}$, which is central to understanding the line's orientation.
##### Geometric Implications of the Components
###### $\LARGE a$ and $\LARGE b$
They define the direction orthogonal (perpendicular) to the line. 
	The ratio $\LARGE \frac{a}{b}$​ gives the slope of the line when $b \neq 0$.
		 Geometrically, these coefficients indicate how the line changes as you move along the $x$ or $y$ directions.
###### $\LARGE c$
This shifts the line in the direction of the normal vector.
	If you change $c$ while keeping $a$ and $b$ constant, you’re moving the line along the direction perpendicular to its orientation.

### A Shift in Perspective
The coordinates $(x,y)$ represent a point in a plane. 

$\LARGE x,y$ are both **scalars**.
	But what are they scaling?

Consider that they are scaling some [[Points as Position Vectors#Standard Unit Vectors (Basis Vectors)|standard unit]] that defines the plane itself.
	These standard units are vectors, that is [[Points as Position Vectors#Cartesian Vector Form (i.e. Scalar Basis Form)|Standard Basis Vectors]].
		Where a Basis Vector exists for each [[Axes and Dimensions|dimension]] in a space.
			So each "coordinate" of a dimension, scales a corresponding Basis Vector (of that dimension).
$$\LARGE x = x \cdot \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \quad y = y \cdot \begin{bmatrix} 0 \\1 \end{bmatrix}$$
From this understanding, we can now see that points, which can be represented by coordinates, are fundamentally a scaling of a standard unit vector. 
	Therefore, each coordinate of a dimension **is** a actually a vector.
$$\LARGE x = \begin{bmatrix} x \cdot 1 \\ x \cdot 0 \end{bmatrix}, \quad y = \begin{bmatrix}  y \cdot0 \\  y \cdot1 \end{bmatrix}$$
The coefficients $y$ and $x$ act as **weights** that combine the standard basis vectors $\hat{i} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}$ and $\hat{j} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}$.

This implies that a point itself is a vector.
	Which itself is containing the "coordinates" as component vectors.
		This point as a vector is called a [[Points as Position Vectors|position vector]].
$$\LARGE \vec{r} = \begin{bmatrix} x \\ y \end{bmatrix} =  x \hat{i} + y \hat{j}$$

- - - 
## Line Represented as a Set of Position Vectors
Remember that [[Points as Position Vectors|Points are Position Vectors]].

A **position vector** $\vec{r} = x \hat{i} + y \hat{j}$ represents a point $(x,y)$ on the line.
	It originates at the origin and points to the location $(x,y)$ in the coordinate system.

Consider **every point** $(x,y)$ on the line as being represented by a **[[#Position Vectors, $ vec{r}$, are Cartesian Vectors|position vector]]**:
$$\LARGE \vec{r} = \begin{bmatrix} x \\ y \end{bmatrix} =  x \hat{i} + y \hat{j}$$
Here, $x$ and $y$ are the coordinates of the point, and $\hat{i}$ and $\hat{j}$​ are the unit vectors along the $x$- and $y$-axes, respectively.
###### Origin of the Position Vector of a Point (on a line)
Just like the normal vector, the position vector is drawn **from the origin** to the point on the line. 
	This is a standard way to represent points in vector analysis.
		 The vector $[x,y]$ gives the coordinates of the point in relation to the origin.
### Defining a Line as a Set of Points
A line in 2D can be described using an equation, often in its **standard form**:
$$\LARGE ax+by + c=0$$
This equation represents the set of all points $(x,y)$ that lie on the line. 
	For every pair $(x,y)$ that satisfies this equation, there is a **position vector** pointing to that location in the coordinate system.

The coefficients $a$ and $b$ define a constraint that **scales** the contributions from the $x$- and $y$-axes to equal a constant $c$.
	This equation is essentially "balancing" the combination of the dimensions $x$ and $y$ in relation to the line's orientation and position.

The **line** itself can then be thought of as the collection (or set) of **all such position vectors that satisfy the equation** $ax+by=c$.
	In other words, the **line is the set of all vectors $\vec{r}$ whose components $(x,y)$ make the equation true**.

- - -
### The Relationship Between the Forms of a Position Vector and Normal Form of a Line
The **position vector** and the **equation of a line in normal form** share a similar structure, and this similarity is deeply rooted in their relationship with the **origin**. Let's break this down to clarify the connection.
- When you have a **position vector** \( \vec{r} = x \hat{i} + y \hat{j} \), it inherently describes a point's position starting from the origin. In essence, it expresses a **linear combination** of the unit vectors \( \hat{i} \) and \( \hat{j} \) scaled by \( x \) and \( y \), respectively.
- Similarly, the **line equation** \( Ax + By = 0 \) can be viewed as a linear relationship between the coordinates \( x \) and \( y \). In this case, the coefficients \( A \) and \( B \) indicate the direction of the normal vector to the line.
- The forms appear similar because, in both cases:
  - The **position vector** \( x \hat{i} + y \hat{j} \) implies a direction and magnitude relative to the origin.
  - The line equation \( Ax + By = 0 \) describes all the points \( (x, y) \) that lie along a line passing through the origin. This line can be characterized by vectors that, when scaled, also represent directions relative to the origin.

**Connection When \( C = 0 \):**
- When the constant \( C = 0 \) in the line equation \( Ax + By + C = 0 \), the line **must pass through the origin**. 
- The similarity in form between the position vector \( x \hat{i} + y \hat{j} \) and the line equation \( Ax + By = 0 \) arises because they both involve linear combinations of the coordinate directions \( \hat{i} \) and \( \hat{j} \) relative to the origin.
- When C=0C = 0C=0 in the equation Ax+By=0Ax + By = 0Ax+By=0, the line does indeed pass through the origin. This is because when x=0x = 0x=0 and y=0y = 0y=0, the equation is satisfied, confirming that the origin (0,0)(0, 0)(0,0) lies on the line. So the line intersects the origin when C=0C = 0C=0.
And then let's say the equation is AX plus BY equals some scalar, a real number. Then that means that you would, to even out the equation, you're always trying to get a zero on the right-hand side, so that...”
By moving everything to one side and setting the equation to zero, Ax+By−D=0Ax + By - D = 0Ax+By−D=0, where DDD is some real number, you simplify the process of finding the intercepts and analyzing the line's properties. This form also makes it easier to apply certain linear algebra techniques, like matrix operations, to analyze or solve systems of equations.


When D≠0D \neq 0D=0 in the equation Ax+By=DAx + By = DAx+By=D, you can rewrite it as Ax+By−D=0Ax + By - D = 0Ax+By−D=0 to balance the equation. Here, DDD becomes part of the constant term CCC in the standard form Ax+By+C=0Ax + By + C = 0Ax+By+C=0. The value of DDD affects the position of the line relative to the origin. If D=0D = 0D=0, the line passes through the

“In the way that someone would derive the graph of an equation of a line in this form by looking at it would just be to mentally know that you would be trying to isolate x or y on either side of the equation so that you could find the y or x intercept.”

00:17

###### ChatGPT said:

ChatGPT

Yes, that's a good approach! To graph a line from an equation in the form Ax+By+C=0Ax + By + C = 0Ax+By+C=0, you can rearrange it to find the yyy-intercept and xxx-intercept. For example, you can solve for yyy to get it into the slope-intercept form:
##### Slope
The slope of the line given by Ax+By=0Ax + By = 0Ax+By=0 is the negative ratio of the coefficients: −AB-\frac{A}{B}−BA​. This ratio represents the change in yyy for a given change in xxx, which is the definition of slope. These coefficients, AAA and BBB, indeed scale the basis vectors in the vector form of the equation, determining the direction and steepness of the line. So, the slope is directly related to how these scalars affect the line's orientation.


“What is b in slope-intercept form relative to the normal equation? Is b really the c value from the normal equation?”
Yes, that's right! In the slope-intercept form of a linear equation, y=mx+by = mx + by=mx+b, the bbb represents the y-intercept, which is the point where the line crosses the y-axis.

In the standard form of a linear equation, Ax+By+C=0Ax + By + C = 0Ax+By+C=0, you can rearrange it to slope-intercept form:

By=−Ax−C.By = -Ax - C.By=−Ax−C.

y=−ABx−CB.y = -\frac{A}{B}x - \frac{C}{B}.y=−BA​x−BC​.

In this form, −CB-\frac{C}{B}−BC​ is equivalent to bbb in the slope-intercept equation. So yes, bbb in the slope-intercept form corresponds to (-\fr
- - -
### The Normal Equation of a Line as a Dot Product
A line $ax+by + c=0$ as a set of position vectors that have a perpendicular distance from origin along the normal vector that is given by c over the magnitude of the [[Normal Vector|normal vector]].

Where $a,b$, and $c$ are constants, and $(x,y)$ are coordinates in the 2D plane.
	$c$ is a constant that determines the line's position relative to the origin.
		This equation defines a relationship between $x$ and $y$ that all points on the line satisfy. 
			Geometrically, $(a,b)$ represents a vector perpendicular (normal) to the line, and $c$ determines the line's distance from the origin.

The line equation $ax+by=c$ tells us that for every point on the line, the projection of the position vector $[x,y]$ onto the [[Normal Vector]] $[a,b]$ is a constant $c$.

**The left-hand side of the standard form equation of a line can be rewritten** using the **dot product**:
### $$\LARGE ax + by = [a, b] \cdot [x, y] = 0$$
$$\text{This means that the point $[x,y]$ lies on the line that is perpendicular to the normal vector.}$$

$$\LARGE \vec{n} = [a, b] \quad \text{and} \quad \vec{r} = [x, y]= x\hat{i} + y\hat{j}$$
$$\LARGE \mathbf{n} \cdot \mathbf{r} = n_1 r_1 + n_2 r_2 = ax + by$$
$$\LARGE \text{Because $ax+ by =0$}, \quad \vec{n} \cdot \vec{r} = [a, b] \cdot [x, y] = 0$$
The coefficients $a$ and $b$ act as **weights** that combine components of the position vector.
	Which themselves are the linear combinations of $x,y$ with standard basis vectors $\LARGE \hat{i}, \hat{j}$.
$$\LARGE \vec{r} = [x, y]= x\hat{i} + y\hat{j}$$
$$x \hat{i} = x \cdot\begin{bmatrix} 1 \\ 0 \end{bmatrix}, \quad y\hat{j} = y \cdot \begin{bmatrix} 0 \\ 1 \end{bmatrix}$$
 $$x = \begin{bmatrix} x \cdot 1 \\ x \cdot 0 \end{bmatrix}, \quad y = \begin{bmatrix}  y \cdot0 \\  y \cdot1 \end{bmatrix}$$

The coefficients $a$ and $b$ in the standard form describe how much the x and $y$ components are "scaled" or weighted to define the line’s orientation.

This expression represents the **[[Data/Abstract Mathematical Spaces/Linear Algebra/Linearity/Dot Product#Projections of the Standard Form Line Equation $ax+by=c$|projections]]** of the vector $[x,y]$ onto the normal vector $[a,b]$.
	The line equation $ax+by=c$ states that, for all points $(x,y)$ on the line, this projection is **constant** and equal to $c$.
		This combination defines the line's normal vector $\vec{n}$, which is central to understanding the line's orientation.

The [[Normal Vector|normal vector]] $[a,b]$ is **perpendicular** to the line. 
	The dot product $[a,b] \cdot [x,y]$ measures how much the vector $[x,y]$ aligns with (or projects onto) this normal vector.

The line equation $ax+by=c$ tells us that for all position vectors $\vec{r}$ on the line, the dot product with the normal vector $\vec{n} = a \hat{i} + b \hat{j}$ is constant:
$$\LARGE \vec{n} \cdot \vec{r} = c$$
- This means that the [[Data/Abstract Mathematical Spaces/Linear Algebra/Linearity/Dot Product#Projections of the Standard Form Line Equation $ax+by=c$|projection]] of any point $\vec{r}$ onto the normal vector $\vec{n}$ is fixed, implying that all such points lie on a line orthogonal to $\vec{n}$.

- - -
#### The Dot Product as a Scalar Function
This is a scalar value:
$$\LARGE \text{Because $ax+ by + c= 0 \quad$ and $ \quad \vec{n} \cdot \vec{r} = [a, b] \cdot [x, y] = ax + by$}$$
$$\LARGE \text{Then, $\quad \vec{n} \cdot \vec{r} = [a, b] \cdot [x, y] = 0$}$$
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
#### $c$ is a Translational Term
##### What $c$ Represents Geometrically
The constant $c$ can be thought of as controlling the line’s "offset" from the origin.

The constant $c$ represents the **signed distance** of the line from the origin.
	That is, it affects the **position** of the line relative to the origin.
		When $c=0$ the line passes through the origin.
			When $c \neq 0$, the line is positioned at some perpendicular distance from the origin.
				I.e. If $c \neq 0$, the line is **shifted** in space.

$\LARGE c$ is a **scalar** that helps determines the **perpendicular distance (along the normal vector) of the line to the origin**.
	I.e. How far the line is positioned from the origin as measured along this Normal Vector. 
		Since the normal vector $[a,b]$ originates from the origin, $c$ can be seen as controlling the line's **offset** along the direction of this normal vector.

When we say the line "projects" onto the normal vector, we mean that the entire line is positioned in such a way that if you were to "drop a perpendicular" from every point on the line to the direction of the normal vector, the distance measured would be proportional to $c$.
	This "projection" is why $c$ acts as a measure of the **perpendicular distance** from the origin to the line:

The constant $c$ determines **where** this line is positioned relative to the origin $(0,0)$ and the direction defined by the normal vector.
	The value $c$ tells us how far along this direction the line is from the origin.
		This means the line is positioned such that every point on it maintains a fixed perpendicular distance from the origin, as dictated by the value of $c$.
#### Visualizing the Projection and $c$
Imagine that the normal vector starts at the origin and points outwards. 
	The line $ax+by=c$ **is positioned somewhere *along* this normal direction**.

Imagine you have the normal vector $[a,b]$ originating from the origin, as an arrow pointing perpendicular to the line.
	If you "walk" along the line, the normal vector always points in the same direction, indicating the orientation of the line in the plane.
		The value of $c$ effectively "shifts" the line along the direction of the normal vector.
			 A larger $|c|$ moves the line further away from the origin, while a smaller $∣c∣$ brings it closer.
#### Distance Interpretation
The constant $c$ **specifies how far the line is from the origin** along the direction of the normal vector.
	It does **not** represent a physical point but rather a scalar that determines the line’s position relative to the origin.

The value of $c$ is related to the **signed perpendicular distance** of the line from the origin.
	Specifically, the **distance** $d$ from the origin to the line $ax+by=c$ is: 
$$\LARGE d = \frac{|c|}{\sqrt{a^2 + b^2}}$$
Where: 
- The term $\sqrt{a^2 + b^2}$​ is the length (or magnitude) of the normal vector $[a,b]$.
- The ratio $\LARGE \frac{|c|}{\sqrt{a^2 + b^2}}$​ normalizes $c$ by the length of the normal vector to get the actual perpendicular distance from the origin to the line.

This distance is measured **along the normal vector** $(a,b)$, which is orthogonal to the line.
	The sign of $c$ indicates on which side of the origin the line lies relative to the normal vector's direction.
		When $c=0$, the line passes through the origin.
			When $c \neq 0$, the line is **shifted** in space to be at a fixed perpendicular distance from the origin, proportional to the value of $c$.
- - - 

## The Relationship Between the Slope of a Line, [[Normal Vector|Normal Vector]] and Direction Vector
### Slope of a Line and the Normal Vector
The slope $\LARGE -\frac{a}{b}$​ arises from the **ratio** of the components of the normal vector. 
	This ratio determines how the line behaves in space.
		If the normal vector $[a,b]$ changes direction (i.e., if the values of $a$ and $b$ change), the slope of the line changes accordingly.

This ratio is fundamental because it expresses the **directionality** of the line. 
	The normal vector $[a,b]$ dictates the line’s orientation, while the slope $-\frac{a}{b}$​ describes how the line rises or falls as you move along the $x$-axis.
### The Direction Vector of a Line, (i.e. the negation of a one component of the Normal Vector), $\LARGE [b,−a]$ or $\LARGE [-b, a]$
The vector $[b,−a]$ is perpendicular to $[a,b]$ because their dot product equals zero:
$$\LARGE [a, b] \cdot [b, -a] = ab - ab = 0$$
This confirms that $[b,−a]$ is indeed a direction vector along the line.

The direction vector $[b,−a]$ **represents how you move along the line**.
The line’s direction vector, is tangent to the line:
	It points in the **direction of the line**, meaning the vector indicates the line's slope or direction of travel).
		The Direction Vector is therefore **perpendicular** to the normal vector just is the line itself.
			If $[a,b]$ is the normal vector, a direction vector $\LARGE \vec{d}$ for the line can be given by swapping and negating one of the components:
				$\LARGE [b,−a]$ or $\LARGE [-b, a]$ Either of these vectors points along the line.
#### A Fixed Ratio
This condition enforces a specific **linear relationship** between $x$ and $y$, which describes the line’s slope and orientation.

For the direction vector $[b,−a]$:
- The **change in $y$** corresponds to $−a$ (the second component).
- The **change in $x$** corresponds to $b$ (the first component).

The equation $\LARGE [a, b] \cdot [x, y] = 0$, does **not** imply that $\LARGE x=b$ and $\LARGE y=−a$. 
	The equation $\LARGE [a, b] \cdot [x, y] = 0$ is a **linear relationship** between $x$ and $y$.
		This equation means that the coordinates $x$ and $u$ must satisfy the **linear equation** $ax+by=0$ to lie on the line.
			This condition does **not** restrict $x$ and $y$ to specific values like $x=b$ and $y=−a$.
				 Instead, it means that the ratio $\LARGE \frac{x}{y}$​ is fixed based on $a$ and $b$. 
					Specifically, if $b \neq 0$, you can express this relationship as:
					$$\LARGE y=\frac{-a}{b}x$$
The point $(x,y)$ can take various values as long as this **proportionality** is satisfied.

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
### The Direction Vector and the Slope
A direction vector $[b,−a]$ describes the direction in which the line runs.
	The components of this vector show how far you move horizontally ($x$-axis) and vertically ($y$-axis) as you traverse the line. 
		The ratio of these movements ($\LARGE \frac{\Delta y}{\Delta x} = -\frac{a}{b}$​) is precisely the line's slope.
#### Why the Direction Vector Encodes the Slope
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

- - -
## Linking Lines to [[Points as Position Vectors#$ text{ textcolor{green}{Linear Transformation} textcolor{violet}{Applied to the Basis Vectors}}$ (Low Level)|Linear Transformations]]
Consider again: 
$$\LARGE ax + by = [a, b] \cdot [x, y] = c$$
$$\LARGE \vec{n} = [a, b] \quad \text{and} \quad \vec{r} = [x, y]= x\hat{i} + y\hat{j}$$
$$\LARGE \mathbf{n} \cdot \mathbf{r} = n_1 r_1 + n_2 r_2 = ax + by$$
$$\LARGE \text{Because $ax+ by =c$}, \quad \vec{n} \cdot \vec{r} = [a, b] \cdot [x, y] = c$$
Where $\LARGE c$ is a [[#The Dot Product as a Scalar Function|Scalar Value]].

You can think of the Standard Form of line equation as the result of a **linear transformation** applied to the vector.
$$\LARGE \vec{r} = \begin{bmatrix} x \\ y \end{bmatrix}$$
$$\LARGE T(\vec{r}) = \begin{bmatrix} a & b \end{bmatrix} \cdot \vec{r}$$
This transformation "[[Data/Abstract Mathematical Spaces/Linear Algebra/Linearity/Dot Product#Projections of the Standard Form Line Equation $ax+by=c$|projects]]" $\vec{r}$ onto the direction of $\vec{n}$.
	The line itself is the set of all vectors $\vec{r}$ that, under this transformation, yield the constant value $c$. 
		This perspective shows that the line equation is tied to the concept of **projection** in vector spaces.
### A Linear Map from Vectors to Scalars (i.e. A Scalar Function)
The dot product with a fixed vector $[ab]$ can be interpreted as a linear map from vectors in $\mathbb{R}^2$ to scalars in $\mathbb{R}$:
$$\LARGE T(\vec{r}) = \begin{bmatrix} a & b \end{bmatrix} \cdot \vec{r}$$
Where $\vec{v} = [x \, y]$.
	This operation maps the vector $\vec{v}$ to a scalar, and it is **linear** because it satisfies the properties of linearity (additivity and scalar multiplication).

If you think of this dot product as a **linear map**, it can be interpreted as **extracting a certain "projection" or "component"** of the vector $[xy]$ in the direction of the fixed vector $[a \, b]$.
	In this sense, the dot product acts like a **transformation** that compresses the information of the vector $[xy]$ into a single scalar, $c$.

That is, the Linear Map takes a vector as an input and returns a scalar value that itself represents the position of that vector along its corresponding normal vector.
	This scalar position value is critical to determining the distance of the initial line from the origin. 
- - - 
## Interpreting the Line Equation as a [[Points as Position Vectors#$ text{ textcolor{green}{Linear Transformation} textcolor{violet}{Applied to the Basis Vectors}}$ (Low Level)|Linear Transformation]]
**Linear transformations** and **projections** are deeply intertwined with the nature of lines, and the dot product encapsulates this relationship by projecting vectors onto a specific direction (the normal vector), defining the linear relationship that gives rise to the line equation 

This projection perspective shows why lines in 2D space have such a strong connection to linear transformations. 
	When you apply a linear transformation to a vector space (like a rotation or scaling), the set of points that form a line (as defined by a constant projection) transforms in a way that preserves linearity, resulting in another line in the transformed space.

The core idea is that the line equation can be seen as a **linear transformation** of the vector $\vec{r} = \begin{bmatrix} x \\ y \end{bmatrix}$ into a scalar value.
$$\LARGE ax + by = c$$
###### Line as a Linear Constraint
The line equation represents a constraint on vectors $\vec{r} = \begin{bmatrix} x \\ y \end{bmatrix}$ in 2D space. 
	This constraint can be viewed as a **projection** onto the normal vector, indicating that all points on the line share a specific linear relationship.
###### Linear Transformation
The operation takes the vector $\vec{r} = \begin{bmatrix} x \\ y \end{bmatrix}$ and maps it to a **scalar** in $\mathbb{R}$. 
	The dot product is a specific type of linear transformation that projects one vector (in this case, $\vec{r}$) onto another fixed vector (here, the normal vector $[a, b]$).

The line equation can be seen as a result of a **linear transformation** (dot product) applied to the position vector $\vec{r}$. 
	This transformation projects the vector onto the normal vector $[a, b]$ and yields a scalar $c$.

The line itself is the set of all vectors in 2D that, under this projection, produce the same scalar value $c$. 
	Thus, the line equation is fundamentally tied to the concept of projection and linear maps in vector spaces.
###### Resulting Line
The line equation $ax + by = c$ defines the set of all vectors $\vec{r}$ in $\mathbb{R}^2$ that, when transformed by this operation, yield the constant scalar $c$.
	This is why we can think of the line as a collection of vectors that satisfy this specific projection relationship.
### The Line as a Projection
The dot product $\begin{bmatrix} a & b \end{bmatrix} \cdot \begin{bmatrix} x \\ y \end{bmatrix} = ax + by$ can be interpreted as projecting the vector $\vec{r} = \begin{bmatrix} x \\ y \end{bmatrix}$ onto the **fixed direction** of the vector $[a, b]$.
###### Geometric Projection
In geometric terms, this operation "compresses" the 2D vector $\vec{r}$ onto the line defined by the normal vector $[a, b]$.
	The resulting scalar $c$ is the length of this projection, scaled by the magnitude of the normal vector $[a, b]$.
#### Linear Map from Vectors to Scalars
By interpreting the dot product as a linear map, we see that the line equation $ax + by = c$  is not just a constraint on coordinates but describes the set of vectors whose linear transformation (projection onto $[a, b]$) results in the constant scalar $c$.
	This is the essence of what the line represents: it is the collection of vectors that satisfy this particular linear mapping.

The dot product $T(\vec{r}) = \begin{bmatrix} a & b \end{bmatrix} \cdot \vec{r}$ is a **linear map** from the 2D vector space $\mathbb{R}^2$ to the scalar field $\mathbb{R}$. 
	This mapping is linear because it respects the properties of linearity (additivity and scalar multiplication):
		  **Additivity:** $T(\vec{r}_1 + \vec{r}_2) = T(\vec{r}_1) + T(\vec{r}_2)$.
		  **Scalar Multiplication:** $T(c\vec{r}) = cT(\vec{r})$.
#### Extracting the Projection
When you perform the dot product $T(\vec{r}) = \begin{bmatrix} a & b \end{bmatrix} \cdot \vec{r}$, you are essentially extracting the **component** of the vector $\vec{r}$ that lies in the direction of $[a, b]$. 
	This is the **projection** of $\vec{r}$ onto the normal vector.
		The result, a scalar $c$, "compresses" the information of the vector $[x, y]$ into a single number that reflects how much of $\vec{r}$ aligns with the normal vector $[a, b]$.
#### Connecting to Linear Transformations and Lines
**Linear Transformation:** Viewing the line equation $ax + by = c$ as a **linear map** helps us understand the line as a set of all vectors whose projection onto a fixed direction (given by $[a, b]$) results in a constant value $c$.

**Transformation of Space:** If we were to apply a different **linear transformation** (e.g., a matrix $A$) to the entire space, the set of vectors satisfying $ax + by = c$ would transform correspondingly.
	This is why lines map to other lines under linear transformations: the relationship $ax + by = c$ changes but maintains its linearity in the transformed space.
#### How the Concepts Link Together




