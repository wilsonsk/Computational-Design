# Projections
###### [[#Scalar Projection|Scalar Projection]]
The result is a scalar (a single number).
	Provides the magnitude of the projection of $a$ onto the direction of $b$.
###### [[#Vector Projection|Vector Projection]]
The result is a vector.
	Provides the actual vector that represents the projection of $a$ onto $b$.
##### Connecting Projections and Dot Products
#### [[Dot Product|Dot Product]]
Measures how much one vector points in the direction of another vector.
	It is the product of the magnitudes of the two vectors and the cosine of the angle between them.
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
## Scalar Projection
The scalar projection of a vector $\mathbf{a}$ onto a vector $\mathbf{b}$ is a measure of the magnitude of $\mathbf{a}$ in the direction of $\mathbf{b}$ 
	It is a scalar value (a single number) that tells you how much of $\mathbf{a}$ lies in the direction of $\mathbf{b}$.
##### The scalar projection of $a$ onto $b$ is given by:
$$\LARGE \text{comp}_{b} a = \|a\| \cos \theta = \frac{a \cdot b}{\|b\|}$$
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
   - The unit vector in the direction of $\mathbf{b}$ is:
     $$
     \hat{\mathbf{b}} = \frac{\mathbf{b}}{\|\mathbf{b}\|}
     $$

##### 4. Multiply the Scalar Projection by the Unit Vector
The scalar projection of $\mathbf{a}$ onto $\mathbf{b}$ tells us how much of $\mathbf{a}$ lies in the direction of $\mathbf{b}$. 
	However, it only gives us a magnitude, not a direction. 
		To get the actual vector that represents this projection, we need to scale this magnitude by a vector that points in the direction of $\mathbf{b}$. 
			This is where the unit vector $\hat{\mathbf{b}}$ comes in.

To convert the scalar projection into a vector in the direction of $\mathbf{b}$, we multiply the scalar projection by the unit vector in the direction of $\mathbf{b}$.
   - The vector projection of $\mathbf{a}$ onto $\mathbf{b}$ is obtained by scaling the unit vector $\hat{\mathbf{b}}$ by the scalar projection $\text{comp}_{\mathbf{b}} \mathbf{a}$:
     $$
     \text{proj}_{\mathbf{b}} \mathbf{a} = \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\|} \right) \hat{\mathbf{b}}
     $$

##### 5. Substitute the Unit Vector $\hat{\mathbf{b}}$
   - Replace $\hat{\mathbf{b}}$ with $\frac{\mathbf{b}}{\|\mathbf{b}\|}$:
     $$
     \text{proj}_{\mathbf{b}} \mathbf{a} = \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\|} \right) \left( \frac{\mathbf{b}}{\|\mathbf{b}\|} \right)
     $$

##### 6. Simplify the Expression
   - Multiply the scalars together:
   $$\LARGE \text{proj}_{\mathbf{b}} \mathbf{a} = \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\| \cdot \| \mathbf{b} \|} \right) \mathbf{b}$$
   where the [[#Self-Dot Product $b cdot b$|Self Dot Product]] of $b$ is $\|b\| \cdot \| b \|$
$$\LARGE = \text{proj}_{\mathbf{b}} \mathbf{a} = \left( \frac{\mathbf{a} \cdot \mathbf{b}}{\|\mathbf{b}\|^2} \right) \mathbf{b}$$

### Projection Calculation
The term $\frac{a \cdot b}{b \cdot b}$ is a scalar that tells us how much of $a$ lies in the direction of $b$.
	By multiplying this scalar by $b$, we get the vector projection of $a$ onto $b$, which lies in the direction of $b$ and has a length proportional to how much $a$ points in the direction of $b$.

