# Projections
Projections as measurements (either scalar values or vector values) that describe the amount if any of a vector in the direction of another vector.
	A projection is NOT measuring the overlay of a vector or producing the overlay of a vector on another.
		It is describing the amount (magnitude) of one vector in the DIRECTION of another vector. 
###### [[#Scalar Projection|Scalar Projection]]
The result is a scalar (a single number).
	Provides the magnitude of the projection of $a$ onto the direction of $b$.
###### [[#Vector Projection|Vector Projection]]
The result is a vector.
	Provides the actual vector that represents the projection of $a$ onto $b$.
### The Vectors, $a$ and $b$
![[Pasted image 20240724132123.png]]
![[Pasted image 20240724132725.png]]
Vector $\mathbf{a}$ and vector $\mathbf{b}$ are positioned such that they both originate from the same point, typically the origin.
	The projection of $\mathbf{a}$ onto $\mathbf{b}$ is a vector that lies along $\mathbf{b}$ and represents the component of $\mathbf{a}$ in the direction of $\mathbf{b}$.

When visualized head-to-tail, the projection starts at the tail of $\mathbf{a}$ (the origin) and extends along $\mathbf{b}$, reaching the point defined by the projection formula. 
	This process effectively decomposes $\mathbf{a}$ into components parallel and orthogonal to $\mathbf{b}$.
### Connecting Projections and Dot Products
#### [[Dot Product|Dot Product]]
Measures how much one vector points in the direction of another vector.
	It is the product of the magnitudes of the two vectors and the cosine of the angle between them.
		The Dot Product *is* the [[#Scalar Projection (i.e. the Dot Product Dot Product )|Scalar Projection]].
##### Dot Product $a \cdot b$:
The dot product of two vectors $a$ and $b$ is defined as:

$$a \cdot b = a_1 b_1 + a_2 b_2 + \ldots + a_n b_n$$

This gives a scalar (a single number) that represents how much of $a$ is in the direction of $b$.
##### Self-Dot Product $b \cdot b$:
The dot product of $b$ with itself is:

$$b \cdot b = b_1^2 + b_2^2 + \ldots + b_n^2$$
This is the same as the square of the magnitude (length) of $b$.
##### Magnitude $\|b\|$:
The magnitude (or norm) of vector $b$ is denoted as $\|b\|$ and is defined as:

$$\|b\| = \sqrt{b_1^2 + b_2^2 + \ldots + b_n^2}$$
It represents the length of the vector $b$.
###### Projection
The projection operation uses the dot product to determine how much of one vector lies in the direction of another.
	The scalar projection gives a measure of this in terms of length, and the vector projection provides a vector in the direction of $\mathbf{b}$ with that length.
## Scalar Projection (i.e. the [[Dot Product|Dot Product]])
The scalar projection of a vector $\mathbf{a}$ onto a vector $\mathbf{b}$ is a measure of the magnitude of $\mathbf{a}$ in the direction of $\mathbf{b}$ 
	It is a scalar value (a single number) that tells you how much of $\mathbf{a}$ lies in the direction of $\mathbf{b}$.
		It gives a scalar value representing the length of the component of $\mathbf{a}$ in the direction of $\mathbf{b}$. 
			It does not overlay vectors but provides the magnitude of this alignment.
##### The scalar projection of $a$ onto $b$ is given by:
$$\LARGE \text{comp}_{b} a = \|a\| \cos \theta = \frac{a \cdot b}{\|b\|} = \mathbf{a} \cdot \mathbf{u_{b}}$$
where:
- $\|a\|$ is the magnitude of $a$,
- $\|b\|$ is the magnitude of $b$,
- $\theta$ is the angle between $a$ and $b$,
- $a \cdot b$ is the dot product of $a$ and $b$.
### Scalar Projection Formula
This formula is derived by using the definition of the dot product and isolating the component of $\mathbf{a}$ in the direction of $\mathbf{b}$.
###### Dot Product
The dot product $\mathbf{a} \cdot \mathbf{b}$ gives a measure of how much of $\mathbf{a}$ lies in the direction of $\mathbf{b}$.
   The dot product of $\mathbf{a}$ and $\mathbf{b}$ is given by:
$$\LARGE
   \mathbf{a} \cdot \mathbf{b} = \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta
$$
   where $\theta$ is the angle between $\mathbf{a}$ and $\mathbf{b}$.

To isolate the scalar projection component, we rearrange the dot product formula to solve for $\cos \theta$
   $$\LARGE 
   \cos \theta = \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{a}\| \|\mathbf{b}\|}
   $$
###### Magnitude of $\mathbf{b}$
Dividing by $\|\mathbf{b}\|$ normalizes this measure to the unit length of $\mathbf{b}$, effectively giving the length of the projection of $\mathbf{a}$ onto $\mathbf{b}$.
##### Formula of the Scalar Projection of $\mathbf{a}$ onto $\mathbf{b}$
Is the magnitude of $\mathbf{a}$ in the direction of $\mathbf{b}$.
	This is represented as:
$$\LARGE
\text{comp}_{\mathbf{b}} \mathbf{a} = \|\mathbf{a}\| \cos \theta
$$
Using the isolated $\cos \theta$ from the dot product definition, we substitute:
$$\LARGE
\text{comp}_{\mathbf{b}} \mathbf{a} = \|\mathbf{a}\| \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{a}\| \|\mathbf{b}\|} \right)
$$
Notice that $\|\mathbf{a}\|$ cancels out:
$$\LARGE
\text{comp}_{\mathbf{b}} \mathbf{a} = \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\|}
$$
## Vector Projection
The vector projection of a vector $a$ onto a vector $b$ not only tells you how much of $a$ lies in the direction of $b$, but also gives you the actual vector in the direction of $b$ that represents this component.
	It is a vector quantity.
		It gives a vector representing the component of $\mathbf{a}$ in the direction of $\mathbf{b}$. 
			It shows how $\mathbf{a}$ overlays onto $\mathbf{b}$ in both magnitude and direction.
				This is the actual vector that represents the component of $\mathbf{a}$ in the direction of $\mathbf{b}$.
					 It has both a direction (the same as $\mathbf{b}$) and a magnitude (the scalar projection).
						 The vector projection does not physically overlay one vector on top of another, but it does create a new vector that is **oriented** in the direction of the vector onto which we are projecting. 
							 This new vector has a magnitude that represents how much the original vector "covers" or aligns with the direction of the other vector, as if they were to be overlaid.

- It is a vector.
- It represents the component of $\mathbf{a}$ that lies in the direction of $\mathbf{b}$.
- It provides both the direction (same as $\mathbf{b}$) and the magnitude (length of the projection).
### Decomposing Vector $a$ into Components Relative to Vector $b$
Projections can be thought of as identifying the components of a vector in the direction of another vector. 
	When you project a vector a\mathbf{a}a onto another vector b\mathbf{b}b, you are essentially finding how much of a\mathbf{a}a lies in the direction of b\mathbf{b}b
		The projection of a vector a\mathbf{a}a onto another vector b\mathbf{b}b can be thought of in terms of breaking down a\mathbf{a}a into two components:
	1. **Parallel Component**: The part of a\mathbf{a}a that lies in the same direction as b\mathbf{b}b.
	2. **Orthogonal Component**: The part of a\mathbf{a}a that is perpendicular to b\mathbf{b}b.

The projection of vector $a$ onto vector $b$ is a way of expressing how much of vector $a$ points in the direction of vector $b$. The formula for the projection of $a$ onto $b$ is:

$$\text{proj}_{b} a = \left( \frac{a \cdot b}{b \cdot b} \right) b$$

### Vector Projection Formula
The vector projection formula can be derived from the geometric understanding of projecting one vector onto another. 
	It uses the scalar projection to find the length of the projection and scales the unit vector in the direction of $\mathbf{b}$ to produce a vector with the correct direction and magnitude.

The vector projection of a vector $\mathbf{a}$ onto another vector $\mathbf{b}$ provides a vector that represents how much of $\mathbf{a}$ lies in the direction of $\mathbf{b}$.

By combining these elements, the formula for the vector projection gives a vector that points in the direction of $\mathbf{b}$ and has a magnitude equal to the component of $\mathbf{a}$ in that direction.
- **Unit vector in the direction of $\mathbf{b}$**: $\hat{\mathbf{b}} = \frac{\mathbf{b}}{\|\mathbf{b}\|}$
- **$\mathbf{a} \cdot \mathbf{b}$**: This term measures how much $\mathbf{a}$ aligns with $\mathbf{b}$.
- **$\|\mathbf{b}\|^2$**: Normalizes the projection relative to the length of $\mathbf{b}$.
- **$\mathbf{b}$**: Provides the direction of the projection, scaled to represent the component of $\mathbf{a}$ in the direction of $\mathbf{b}$.
##### 1. Dot Product Definition
   The dot product of $\mathbf{a}$ and $\mathbf{b}$ is given by:
   $$
   \mathbf{a} \cdot \mathbf{b} = \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta
   $$
   where $\theta$ is the angle between $\mathbf{a}$ and $\mathbf{b}$.

##### 2. Scalar Projection
   The scalar projection of $\mathbf{a}$ onto $\mathbf{b}$ is:
   $$
   \text{comp}_{\mathbf{b}} \mathbf{a} = \|\mathbf{a}\| \cos \theta = \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\|}
   $$


##### 3. Express $\mathbf{b}$ in terms of its unit vector
To project onto a unit vector in the direction of $\mathbf{b}$, first normalize $\mathbf{b}$ by dividing it by its magnitude $\|\mathbf{b}\|$:
   - The unit vector in the direction of $\mathbf{b}$ is:
     $$
     \hat{\mathbf{b}} = \frac{\mathbf{b}}{\|\mathbf{b}\|}
     $$
A. **Compute the Magnitude of $\mathbf{b}$**:
The magnitude (or length) of $\mathbf{b}$ is found using the Euclidean norm: 
$$\|\mathbf{b}\| = \sqrt{b_x^2 + b_y^2 + b_z^2}$$
	This operation sums the squares of the components of $\mathbf{b}$ and then takes the square root. The result is the length of $\mathbf{b}$.
B. **Normalize $\mathbf{b}$**:
Divide each component of $\mathbf{b}$ by its magnitude to obtain the unit vector $\mathbf{u_b}$​: 
$$\mathbf{u_b} = \frac{\mathbf{b}}{\|\mathbf{b}\|} = \left( \frac{b_x}{\|\mathbf{b}\|}, \frac{b_y}{\|\mathbf{b}\|}, \frac{b_z}{\|\mathbf{b}\|} \right)$$
	This operation scales $\mathbf{b}$ so that its length becomes 1, effectively orienting the direction of $\mathbf{b}$ without changing its direction.
##### 4. Multiply the Scalar Projection by the Unit Vector
The scalar projection of $\mathbf{a}$ onto $\mathbf{b}$ tells us how much of $\mathbf{a}$ lies in the direction of $\mathbf{b}$. 
	However, it only gives us a magnitude, not a direction. 
		To get the actual vector that represents this projection, we need to scale this magnitude by a vector that points in the direction of $\mathbf{b}$. 
			This is where the unit vector $\hat{\mathbf{b}}$ comes in.

To convert the scalar projection into a vector in the direction of $\mathbf{b}$, we multiply the scalar projection by the unit vector in the direction of $\mathbf{b}$.
   - The vector projection of $\mathbf{a}$ onto $\mathbf{b}$ is obtained by scaling the unit vector $\hat{\mathbf{b}}$ by the scalar projection $\text{comp}_{\mathbf{b}} \mathbf{a}$:
$$\LARGE \text{proj}_{\mathbf{b}} \mathbf{a} = (\mathbf{a} \cdot \mathbf{u_{b}})\mathbf{u_{b}} = \left(\frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\|}\right) \left(\frac{\mathbf{b}}{\|\mathbf{b}\|}\right) = \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\|} \right) \hat{\mathbf{b}}$$
A. **Compute the Dot Product**:
The dot product of $\mathbf{a}$ and the unit vector $\mathbf{u_b}$​ is calculated as:
$$\LARGE \mathbf{a} \cdot \mathbf{u_b} = a_x u_x + a_y u_y + a_z u_z$$​
$$\text{Substituting } \mathbf{u_b} = \left( \frac{b_x}{\|\mathbf{b}\|}, \frac{b_y}{\|\mathbf{b}\|}, \frac{b_z}{\|\mathbf{b}\|} \right)$$

$$\LARGE \text{We get } \mathbf{a} \cdot \mathbf{u_b} = a_x \frac{b_x}{\|\mathbf{b}\|} + a_y \frac{b_y}{\|\mathbf{b}\|} + a_z \frac{b_z}{\|\mathbf{b}\|}$$
This operation scales the components of $\mathbf{a}$ by the corresponding components of the unit vector $\mathbf{u_b}$ and sums the results.
	The result is the magnitude of the projection of $\mathbf{a}$ onto $\mathbf{b}$.

##### 5. Substitute the Unit Vector $\hat{\mathbf{b}}$
   - Replace $\hat{\mathbf{b}}$ with $\frac{\mathbf{b}}{\|\mathbf{b}\|}$:
$$\LARGE \text{proj}_{\mathbf{b}} \mathbf{a} = \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\|} \right) \left( \frac{\mathbf{b}}{\|\mathbf{b}\|} \right)$$
##### 6. Simplify the Expression
   - Multiply the scalars together:
   $$\LARGE \text{proj}_{\mathbf{b}} \mathbf{a} = \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\| \cdot \| \mathbf{b} \|} \right) \mathbf{b}$$
   where the [[#Self-Dot Product $b cdot b$|Self Dot Product]] of $b$ is $\|b\| \cdot \| b \|$
$$\LARGE = \text{proj}_{\mathbf{b}} \mathbf{a} = \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\|^2} \right) \mathbf{b}$$
- The projection of $\mathbf{a}$ onto $\mathbf{b}$, denoted as $\text{Proj}_{\mathbf{b}} \mathbf{a}$, is a vector that lies along the direction of $\mathbf{b}$.
- This projection vector represents the component of $\mathbf{a}$ that is in the same direction as $\mathbf{b}$.
### Projection Calculation
The term $\LARGE \frac{a \cdot b}{b \cdot b}$ is a scalar that tells us how much of $a$ lies in the direction of $b$.
	By multiplying this scalar by $b$, we get the vector projection of $a$ onto $b$, which lies in the direction of $b$ and has a length proportional to how much $a$ points in the direction of $b$.
## Parallel Projection
The parallel projection of $\mathbf{a}$ onto $\mathbf{b}$ is given by:
 $$\text{Proj}_{\mathbf{b}} \mathbf{a} = \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\mathbf{b} \cdot \mathbf{b}} \right) \mathbf{b}$$ 
 Here, $\mathbf{a} \cdot \mathbf{b}$ represents the dot product, and $\mathbf{b} \cdot \mathbf{b}$ is the square of the magnitude of $\mathbf{b}$.
## Perpendicular Projection
I.e. The **component of a vector $\vec{A}$** that is **parallel to vector $b$**
	 I.e. The line/vector that would be **adjacent** vector $\vec{A}$.
		Which is found by  
			If $\large |\vec{A_{||_{b}}}| = |\vec{A}|\cos\theta$  where $\theta$ is the angle between the vector, $\vec{A}$ and its parallel projection, $\vec{A_{||_{a}}}$ 
				Then $\large \vec{\hat{u_{a}}} \cdot \vec{A_{||_{b}}} = \vec{\hat{u_{b}}}|\vec{A}| \cos \theta$ (*see the above* [[#Geometric Interpretation|Geometric Interpretation of Dot Product]])
					Remember the norm or magnitude of a unit vector, $\vec{\hat{U}}$, is 1.  
						$\vec{\hat{u_{b}}}|\vec{A}| == 1 \times |\vec{A}| = |\vec{A}|$
							Therefore,
								Projection of A onto line $\vec{\hat{u_{b}}}$ is
								 $\large \vec{A_{||}} = |\vec{A}|\cos \theta$ which was identified originally.
									Therefore, because the two "left-hand sides" of the equations are equal.
###### The Parallel Projection (magnitude) of **vector $\vec{A}$ *onto* line $\hat{u}$**=
	 $\large |\vec{A_{||_{b}}}| = \vec{\hat{u_{b}}} \cdot \vec{A_{||_{b}}}$ 
###### Vector or component form of the Parallel Projection of **vector $\vec{A}$ *onto* vector $b$** =
$\large \vec{A_{||_{b}}} = |\vec{A}|\cos\theta\times \hat{u_{b}}$  
$\large == \vec{A_{||_{b}}} = (\vec{\hat{u_{b}}} \cdot \vec{A})\vec{\hat{u_{b}}}$
The **perpendicular/orthogonal projection**.
- I.e. The **component of a vector $\vec{A}$** that is **perpendicular to Vector $b$**.
	-  I.e. The line/vector that would be **opposite** vector $\vec{A}$.
		 $\large \vec{A} = \vec{A_{||}} + \vec{A_{\perp}}$ because these are the "components" of vector $\vec{A}$
			 Therefore,
				 $\large \vec{A_{\perp}} =  \vec{A} - \vec{A_{||}}$ 
				 
To find the perpendicular projection, subtract the parallel projection from $\mathbf{a}$: $$\text{Perpendicular Projection} = \mathbf{a} - \text{Proj}_{\mathbf{b}} \mathbf{a}$$Substituting the parallel projection, we get: 
$$\text{Perpendicular Projection} = \mathbf{a} - \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\mathbf{b} \cdot \mathbf{b}} \right) \mathbf{b}$$
### Alignment
#### Perpendicularity (Orthogonality):
Two vectors $\mathbf{a}$ and $\mathbf{b}$ are perpendicular if their dot product is zero: 
$$\mathbf{a} \cdot \mathbf{b} = 0$$

When this dot product is zero, it indicates that there is no component of the first vector in the direction of the second vector. 
#### Parallelism (i.e. Alignment)
Two vectors $\mathbf{a}$ and $\mathbf{b}$ are parallel if one is a scalar multiple of the other:
$$\mathbf{a} = k \mathbf{b} \quad \text{for some scalar}$$
Alternatively, their cross product should be zero:
$$\mathbf{a} \times \mathbf{b} = \mathbf{0}$$
