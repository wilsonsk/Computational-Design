# Law of Cosines
The Law of Cosines is a useful tool in vector mathematics for relating the lengths of vectors and the angle between them. 

## Law of Cosines in Geometry
The Law of Cosines in its standard form is used in a triangle to relate the lengths of its sides to the cosine of one of its angles.
	For a triangle with sides $a$, $b$, and $c$, and an angle $\theta$ opposite side $c$, the Law of Cosines states:
$$\LARGE 
c^2 = a^2 + b^2 - 2ab \cos \theta
$$
## Applying the Law of Cosines to Vectors
To apply the Law of Cosines to vectors, consider two vectors $\mathbf{a}$ and $\mathbf{b}$ with an angle $\theta$ between them. 
	We are interested in the distance between the points represented by these vectors in space.
#### 1. Representing Vectors as Points
Vectors $\mathbf{a}$ and $\mathbf{b}$ can be thought of as points in space originating from a common point (typically the origin). 
	The vector $\mathbf{a} - \mathbf{b}$ represents the vector pointing from $\mathbf{b}$ to $\mathbf{a}$.
		 For vectors $\mathbf{a}$ and $\mathbf{b}$, the Law of Cosines is applied to the vector $\mathbf{a} - \mathbf{b}$, representing the distance between the points in space defined by $\mathbf{a}$ and $\mathbf{b}$.
#### 2. Distance Between Two Vectors
The length of the vector $\mathbf{a} - \mathbf{b}$ is the Euclidean distance between the points represented by $\mathbf{a}$ and $\mathbf{b}$. 
	The squared distance is given by the dot product of $\mathbf{a} - \mathbf{b}$ with itself:
$$\LARGE 
\|\mathbf{a} - \mathbf{b}\|^2 = (\mathbf{a} - \mathbf{b}) \cdot (\mathbf{a} - \mathbf{b})
$$
This relationship helps derive the dot product formula, showing that the dot product measures the extent to which one vector projects onto another, scaled by the cosine of the angle between them.
#### 3. Expanding the Dot Product
We can expand this dot product using the distributive property:
$$\LARGE
(\mathbf{a} - \mathbf{b}) \cdot (\mathbf{a} - \mathbf{b}) = \mathbf{a} \cdot \mathbf{a} - 2\mathbf{a} \cdot \mathbf{b} + \mathbf{b} \cdot \mathbf{b}
$$
#### 4. Connecting to the Law of Cosines
Recall that the dot product of a vector with itself gives the square of its magnitude:
$$\LARGE
\mathbf{a} \cdot \mathbf{a} = \|\mathbf{a}\|^2
$$
$$\LARGE
\mathbf{b} \cdot \mathbf{b} = \|\mathbf{b}\|^2
$$
So, we have:
$$\LARGE
\|\mathbf{a} - \mathbf{b}\|^2 = \|\mathbf{a}\|^2 - 2\mathbf{a} \cdot \mathbf{b} + \|\mathbf{b}\|^2
$$
#### 5. Law of Cosines in Vector Form
From the geometric interpretation, the Law of Cosines states:
$$\LARGE
\|\mathbf{a} - \mathbf{b}\|^2 = \|\mathbf{a}\|^2 + \|\mathbf{b}\|^2 - 2\|\mathbf{a}\|\|\mathbf{b}\|\cos\theta
$$
By comparing the two expressions for $\|\mathbf{a} - \mathbf{b}\|^2$, we equate them:
$$\LARGE
\|\mathbf{a}\|^2 - 2\mathbf{a} \cdot \mathbf{b} + \|\mathbf{b}\|^2 = \|\mathbf{a}\|^2 + \|\mathbf{b}\|^2 - 2\|\mathbf{a}\|\|\mathbf{b}\|\cos\theta
$$
#### 6. Simplifying and Solving for the Dot Product
Cancel $\|\mathbf{a}\|^2$ and $\|\mathbf{b}\|^2$ on both sides:
$$\LARGE
-2\mathbf{a} \cdot \mathbf{b} = -2\|\mathbf{a}\|\|\mathbf{b}\|\cos\theta
$$
Divide by $-2$:
$$\LARGE
\mathbf{a} \cdot \mathbf{b} = \|\mathbf{a}\|\|\mathbf{b}\|\cos\theta
$$

