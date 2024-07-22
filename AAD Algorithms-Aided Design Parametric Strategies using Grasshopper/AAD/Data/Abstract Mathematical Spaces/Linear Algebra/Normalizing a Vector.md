# Normalizing a Vector
Normalizing a vector means scaling the vector so that its length (or magnitude) is equal to 1. 
	The resulting vector, called a unit vector, points in the same direction as the original vector but has a magnitude of 1.
		 This process is useful in many mathematical and physical applications where direction is important but the length of the vector should be standardized.

## Deriving the Equation for Normalizing a Vector

Suppose we have a vector $\mathbf{v} = (v_1, v_2, \ldots, v_n)$ in $n$-dimensional space. The steps to normalize this vector are as follows:

1. **Calculate the Magnitude of the Vector:**

   The magnitude (or length) of the vector $\mathbf{v}$, denoted as $\|\mathbf{v}\|$, is calculated using the Euclidean norm:

   $$\LARGE \|\mathbf{v}\| = \sqrt{v_1^2 + v_2^2 + \cdots + v_n^2}$$

2. **Divide Each Component by the Magnitude:**

   To create a unit vector $\mathbf{u}$ in the same direction as $\mathbf{v}$, divide each component of $\mathbf{v}$ by its magnitude $\|\mathbf{v}\|$:

$$\LARGE \mathbf{u} = \left( \frac{v_1}{\|\mathbf{v}\|}, \frac{v_2}{\|\mathbf{v}\|}, \ldots, \frac{v_n}{\|\mathbf{v}\|} \right)$$

   This ensures that the length of the new vector $\mathbf{u}$ is 1 while preserving the direction of $\mathbf{v}$.

### Example

Consider a vector $\mathbf{v} = (1, 2)$ in 2-dimensional space. 

1. **Calculate the Magnitude:**

   $$\|\mathbf{v}\| = \sqrt{1^2 + 2^2} = \sqrt{1 + 4} = \sqrt{5}$$

2. **Divide Each Component by the Magnitude:**

   $$\mathbf{u} = \left( \frac{1}{\sqrt{5}}, \frac{2}{\sqrt{5}} \right)$$

Thus, the normalized vector $\mathbf{u}$ has a magnitude of 1 and points in the same direction as $\mathbf{v}$.

#### Verification

To verify that $\mathbf{u}$ is indeed a unit vector, we can calculate its magnitude:

$$\|\mathbf{u}\| = \sqrt{\left( \frac{1}{\sqrt{5}} \right)^2 + \left( \frac{2}{\sqrt{5}} \right)^2} = \sqrt{ \frac{1}{5} + \frac{4}{5} } = \sqrt{1} = 1$$

Hence, $\mathbf{u}$ is a unit vector.
