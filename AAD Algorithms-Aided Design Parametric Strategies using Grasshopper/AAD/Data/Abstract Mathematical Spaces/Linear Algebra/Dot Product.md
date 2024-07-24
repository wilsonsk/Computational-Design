# Dot Product (aka the [[Projection#Scalar Projection|Scalar Projection]])
The dot product (also known as the scalar product) of two vectors in Euclidean space has a geometric interpretation that connects it to the projection concept.
	When you take the dot product of two vectors, you are essentially measuring how much one vector projects onto another.
		The Dot Product measures the magnitude of $\mathbf{a}$ in the direction of $\mathbf{b}$ (or vice versa), scaled by the magnitude of $\mathbf{b}$.
			The dot product does not overlay one vector on top of another; instead, it provides a scalar value that quantifies how much one vector aligns with another vector.

- It is a single number (a scalar).
- It represents the length (or magnitude) of the projection of $\mathbf{a}$ onto $\mathbf{b}$.
- It tells you how much of $\mathbf{a}$ lies in the direction of $\mathbf{b}$.
- It does not give you the direction or the actual vector of the projection.
###### Components
**Dot Product $a \cdot b$** gives us a measure of how much one vector extends in the direction of another.
$$\LARGE a \cdot b$$
This measures how much $a$ goes in the direction of $b$. 
	If $a$ and $b$ are pointing in the same direction, the dot product is large and positive.
		 If they are perpendicular, the dot product is zero. 
			 If they are in opposite directions, the dot product is negative.
 
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
##### Inherent [[Projection|Projection]] (i.e. Scalar Projection)
The dot product inherently involves projection because it measures/quantifies how much one vector extends in the direction of another (i.e. measures the extent to which vectors align with each other).
	By incorporating the cosine of the angle between them, it captures the idea of projecting one vector onto the other.

The dot product does not overlay one vector on top of another; instead, it provides a scalar value that quantifies how much one vector aligns with another vector.

**Alignment**: The dot product is large and positive when vectors are pointing in the same direction, indicating a significant projection. 
- If $\cos \theta$ is positive (and thus the dot product), the vectors are pointing in roughly the same direction.
- **Orthogonality**:
	- If $\cos \theta$ is zero (and thus the dot product), the vectors are perpendicular (orthogonal) to each other, indicating no projection.
		- If $\mathbf{a} \cdot \mathbf{b} = 0$, this means that $\cos \theta = 0$ because neither $|\mathbf{a}|$ nor $|\mathbf{b}|$ are zero (assuming non-zero vectors). 
			- The cosine of $0$ implies that the angle $\theta$ between the vectors is $90^\circ$, indicating that $\mathbf{a}$ is perpendicular to $\mathbf{b}$.
				- The result of the dot product between two vectors is a scalar value that represents the magnitude of the projection of one vector onto another. 
					- When this dot product is zero, it indicates that there is no component of the first vector in the direction of the second vector. 
- **Opposition**:
	- If $\cos \theta$ is negative (and thus the dot product), the vectors are pointing in roughly opposite directions, indicating a projection in the negative direction.

**Magnitude of Projection**: The dot product $\mathbf{a} \cdot \mathbf{b}$ gives the product of the magnitude of $\mathbf{a}$ and the component of $\mathbf{b}$ that lies in the direction of $\mathbf{a}$.
	This component is often referred to as the projection of $\mathbf{b}$ onto $\mathbf{a}$.
$$\LARGE a \cdot b = \|a\| \|b\| \cos \theta$$
$$\LARGE \| a \| \cos \theta = \frac{a \cdot b}{\|b\|}$$$$\LARGE \text{proj}_{b} a = \|a\| \cos \theta$$
This scalar value represents the length of the component of $\mathbf{a}$ that lies in the direction of $\mathbf{b}$. 
	It tells you how much of $\mathbf{a}$ is in the direction of $\mathbf{b}$, but it does not provide the actual vector that represents this component.
	
## Geometric Interpretation
Consider two vectors $a$ and $b$ in a Euclidean space. 
	Let $\theta$ be the angle between them. 
		The geometric definition of the dot product involves the magnitudes (lengths) of these vectors and the cosine of the angle between them.
			When you take the dot product of two vectors, you are essentially measuring how much one vector projects onto another.
### Steps to Derive the Dot Product
1. **Definition of the Dot Product** The dot product of two vectors $a$ and $b$, written as $a \cdot b$, is defined as:$$a \cdot b = \|a\| \|b\| \cos \theta$$where:

- $|a|$ is the magnitude of $a$,
- $|b|$ is the magnitude of $b$,
- $\theta$ is the angle between $a$ and $b$.

This formula tells us that the dot product measures the magnitude of $\mathbf{a}$ in the direction of $\mathbf{b}$ (or vice versa), scaled by the magnitude of $\mathbf{b}$.
	The dot product inherently involves the concept of [[Projection|projection]]. 
		Which measures the extent to which one vector projects onto another.

2. **[[Projection#Scalar Projection|Scalar Projection]]** The projection of $a$ onto $b$ (or vice versa) helps to understand the dot product. 
	1. The projection of $a$ onto the direction of $b$ is given by the component of $a$ that lies along $b$. This projection is:$$\LARGE \| a \| \cos \theta = \frac{a \cdot b}{\|b\|}$$$$\LARGE \text{proj}_{b} a = \|a\| \cos \theta$$

4. **Using Projections** If we project $a$ onto $b$, the length of this projection is $|a| \cos \theta$. This projection is then scaled by the magnitude of $b$ to give the dot product:$$a \cdot b = \|b\| \times (\|a\| \cos \theta)$$
5. Thus:$$a \cdot b = \|a\| \|b\| \cos \theta$$
## Algebraic Interpretation

1. **Component Form of Vectors**:
   - Consider two vectors $\mathbf{a}$ and $\mathbf{b}$ in $n$-dimensional space.
   - We represent them in component form as:
     $$
     \mathbf{a} = (a_1, a_2, \ldots, a_n)
     $$
     $$
     \mathbf{b} = (b_1, b_2, \ldots, b_n)
     $$

### Definition of Dot Product in Component Form

2. **Definition of Dot Product in Component Form**:
   - The dot product of $\mathbf{a}$ and $\mathbf{b}$ in $n$-dimensional space is defined as:
     $$
     \mathbf{a} \cdot \mathbf{b} = a_1 b_1 + a_2 b_2 + \ldots + a_n b_n
     $$
   - This is a purely algebraic definition that provides a way to combine two vectors to get a scalar.
### Connection to Geometry

3. **Connection to Geometry using the [[Law of Cosines|Law of Cosines]]**:
   - To understand the geometric interpretation of the dot product, we use the Law of Cosines.
	   - The Law of Cosines relates the lengths of the sides of a triangle to the cosine of one of its angles.
   - For vectors $\mathbf{a}$ and $\mathbf{b}$, the Law of Cosines in the plane spanned by these vectors states:
     $$
     \|\mathbf{a} - \mathbf{b}\|^2 = \|\mathbf{a}\|^2 + \|\mathbf{b}\|^2 - 2 \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta
     $$
   - Here, $\theta$ is the angle between $\mathbf{a}$ and $\mathbf{b}$, and $\|\mathbf{a} - \mathbf{b}\|$ is the Euclidean distance between the points represented by $\mathbf{a}$ and $\mathbf{b}$.
### Expressing the Distance Squared
4. **Expressing the Distance Squared**:
   - The squared distance between $\mathbf{a}$ and $\mathbf{b}$ in terms of components is:
     $$
     \|\mathbf{a} - \mathbf{b}\|^2 = (a_1 - b_1)^2 + (a_2 - b_2)^2 + \ldots + (a_n - b_n)^2
     $$
### Expanding the Distance Squared
5. **Expanding the Distance Squared**:
   - When we expand the expression for $\|\mathbf{a} - \mathbf{b}\|^2$, we get:
     $$
     \|\mathbf{a} - \mathbf{b}\|^2 = (a_1 - b_1)^2 + (a_2 - b_2)^2 + \ldots + (a_n - b_n)^2
     $$
   - Expanding each term, we get:
     $$
     \|\mathbf{a} - \mathbf{b}\|^2 = a_1^2 - 2a_1b_1 + b_1^2 + a_2^2 - 2a_2b_2 + b_2^2 + \ldots + a_n^2 - 2a_nb_n + b_n^2
     $$
### Grouping Terms
6. **Grouping Terms**:
   - We can group the terms to show the sum of the squares of the individual components and the product terms:
     $$
     \|\mathbf{a} - \mathbf{b}\|^2 = (a_1^2 + a_2^2 + \ldots + a_n^2) + (b_1^2 + b_2^2 + \ldots + b_n^2) - 2 (a_1b_1 + a_2b_2 + \ldots + a_nb_n)
     $$
### Equating Both Expressions
7. **Equating Both Expressions**:
   - From the geometric interpretation using the Law of Cosines, we know:
     $$
     \|\mathbf{a} - \mathbf{b}\|^2 = \|\mathbf{a}\|^2 + \|\mathbf{b}\|^2 - 2 \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta
     $$
   - From the algebraic expansion, we have:
     $$
     \|\mathbf{a} - \mathbf{b}\|^2 = (a_1^2 + a_2^2 + \ldots + a_n^2) + (b_1^2 + b_2^2 + \ldots + b_n^2) - 2 (a_1b_1 + a_2b_2 + \ldots + a_nb_n)
     $$
### Simplifying the Equation
8. **Simplifying the Equation**:
   - Equating these two expressions for $\|\mathbf{a} - \mathbf{b}\|^2$, we get:
     $$
     \|\mathbf{a}\|^2 + \|\mathbf{b}\|^2 - 2 \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta = (a_1^2 + a_2^2 + \ldots + a_n^2) + (b_1^2 + b_2^2 + \ldots + b_n^2) - 2 (a_1b_1 + a_2b_2 + \ldots + a_nb_n)
     $$
### Canceling Common Terms
9. **Canceling Common Terms**:
   - The terms $\|\mathbf{a}\|^2$ and $\|\mathbf{b}\|^2$ appear on both sides of the equation and can be canceled out:
     $$
     -2 \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta = -2 (a_1b_1 + a_2b_2 + \ldots + a_nb_n)
     $$
### Final Simplification
10. **Final Simplification**:
    - Dividing both sides by $-2$, we obtain:
      $$
      \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta = a_1 b_1 + a_2 b_2 + \ldots + a_n b_n
      $$
### Conclusion
11. **Conclusion**:
    - Thus, we have derived the dot product equation from both geometric and algebraic perspectives:
      $$
      \mathbf{a} \cdot \mathbf{b} = \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta
      $$
    - This shows how the dot product encapsulates the geometric idea of projection and the angle between two vectors.













