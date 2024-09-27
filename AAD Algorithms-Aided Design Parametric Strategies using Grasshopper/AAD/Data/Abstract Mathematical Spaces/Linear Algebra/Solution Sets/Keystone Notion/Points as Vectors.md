# Points as Vectors
## Vectors
$$\LARGE \vec{v} = \mathbf{v} = (v_1, v_2, v_3) = \begin{bmatrix} v_1 \\ v_2 \\v_3 \end{bmatrix} = \begin{bmatrix} \Delta{v}_1 \\ \Delta v_2 \\ \Delta v_3 \end{bmatrix} = (v_1)\hat{i} + (v_2) \hat{j} + (v_3) \hat{k}$$
Abstract Mathematical Objects that contain two properties.
1. Direction
2. Magnitude
##### A Vectors as a List of Scalar Functions
$$\LARGE (v_1, v_2), \quad (v_1, v_2, v_3), \quad (v_1, v_2, \dots, v_n)$$
Where $\LARGE v_1, v_2, v_n$ are **[[#Component Scalar Functions of Vectors|component scalar functions]]**.
	Where **component scalar functions** are the coordinates that describe a "point".
##### A Vector as the Measure of Displacement
$$\LARGE \Delta{x}, \Delta{y}, \Delta{z}$$
Where what is being **displaced** are the "**points**" defined by the **component scalar functions**.
	More specifically, the scalars produced by the component scalar functions.

![[Pasted image 20240927062156.png|500]]
## Standard Unit Vectors (Basis Vectors)
Are the most fundamental Vectors, containing component scalar functions that always produce the same constant scalars depending on the Basis Vector.
$$\large \mathbf{e}_1 = \vec{e}_1 = \mathbf{i} = \hat{i} = (\hat{i}_1, \hat{i}_2, \hat{i}_3) = \begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \\ \hat{i}_3 \end{bmatrix} = \begin{bmatrix} \Delta\hat{i}_1 \\ \Delta\hat{i}_2 \\ \Delta\hat{i}_3 \end{bmatrix}$$
###### The Components Function of the Basis Vector, $\hat{i}$
$$\LARGE \hat{i} =  (\hat{i}_1 = 1, \space 
\hat{i}_2 = 0, \space \hat{i}_3 = 0) = \begin{bmatrix} 1 \\ 0 \\0 \end{bmatrix} = (1, 0, 0)$$
$$\large \mathbf{e}_2 = \vec{e}_2 = \mathbf{j} = \hat{j} = (\hat{j}_1, \hat{j}_2, \hat{j}_3) = \begin{bmatrix} \hat{j}_1 \\ \hat{j}_2 \\\hat{j}_3 \end{bmatrix}  = \begin{bmatrix} \Delta\hat{j}_1 \\ \Delta\hat{j}_2 \\ \Delta\hat{j}_3 \end{bmatrix}$$
$$\LARGE \hat{j} = (\hat{j}-1 = 0, \space \hat{j}_2 = 1, \space  \hat{j}_3=0) = \begin{bmatrix} 0 \\ 1 \\0 \end{bmatrix} = (0,1,0)$$
$$\large \mathbf{e}_3 = \vec{e}_3 = \mathbf{k} =  \hat{k} = (\hat{k}_1, \hat{k}_2, \hat{k}_3) = \begin{bmatrix} \hat{k}_1 \\ \hat{k}_2 \\\hat{k}_3 \end{bmatrix} = \begin{bmatrix} \Delta\hat{k}_1 \\ \Delta\hat{k}_2 \\ \Delta\hat{k}_3 \end{bmatrix}$$
$$\LARGE \hat{k} = (\hat{k}_1= 0,\space \hat{k}_2=0,\space \hat{k}_1=1)= \begin{bmatrix} 0 \\ 0 \\1 \end{bmatrix} = (0, 0, 1)$$
## Component Scalar Functions Scales the Basis Vectors
Each **Component Scalar Function** scales the **Standard Unit Vectors (i.e. the Basis Vectors)**.
$$\LARGE \vec{v} = \mathbf{v} = (v_1, v_2, v_3) = \begin{bmatrix} v_1 \\ v_2 \\v_3 \end{bmatrix} = \begin{bmatrix} \Delta{v}_1 \\ \Delta v_2 \\ \Delta v_3 \end{bmatrix} = (v_1)\hat{i} + (v_2) \hat{j} + (v_3) \hat{k}$$
$$\LARGE (v_1) \hat{i} = v_1\begin{bmatrix} \hat{i}_1 \\\hat{i}_2 \\ \hat{i}_3\end{bmatrix}, \quad (v_2) \hat{j} = v_2\begin{bmatrix} \hat{j}_1 \\\hat{j}_2 \\ \hat{j}_3\end{bmatrix}, \quad (v_3) \hat{k} = v_3\begin{bmatrix} \hat{k}_1 \\\hat{k}_2 \\ \hat{k}_3\end{bmatrix}$$
### Component Scalar Functions are Linear Transformations $T_A$
#### Linear Transformations
Linear transformation $T$ takes any vector and maps it to the new vector (or space).
$$\large T: \mathbb{R}^n \to \mathbb{R}^m, \quad Domain_T \subset \mathbb{R}^n,\quad  Codomain_T =\set{\mathbb{R}^m}, \quad Range_T \subset \mathbb{R}^m$$
- **$T$:** Refers to a linear transformation in a general sense.
- **$T_A$​:** Explicitly denotes the linear transformation associated with the matrix $A$. 
	- It’s a way to connect the transformation to its matrix representation.
#### The Linear Transformation of a Basis Vector is a Matrix, $A$ 
$$\LARGE T_{A}(\vec{e_1}) = A\vec{e_1}$$
$$\LARGE A = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix}, \quad \vec{e_1} = \begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \end{bmatrix} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \quad \vec{e}_2 = \begin{bmatrix} \hat{j}_1 \\ \hat{j}_2 \end{bmatrix} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}$$
$$\LARGE T_A(\vec{e_1}) = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix} \begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \end{bmatrix} = \begin{bmatrix} (a_{11} \cdot \hat{i}_1) + (a_{12} \cdot \hat{i}_2) \\ (a_{21} \cdot \hat{i}_1) + (a_{22} \cdot \hat{i}_2) \end{bmatrix}$$
$$\LARGE = T_A(\vec{e_1}) = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix} \begin{bmatrix} 1 \\ 0 \end{bmatrix} = \begin{bmatrix} (a_{11} \cdot 1) + (a_{12} \cdot 0) \\ (a_{21} \cdot 1) + (a_{22} \cdot 0) \end{bmatrix} = \begin{bmatrix} a_{11} \\ a_{21}\end{bmatrix}$$
$$\LARGE T_A(\vec{e_2}) = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix} \begin{bmatrix} \hat{j}_1 \\ \hat{j}_2 \end{bmatrix} = \begin{bmatrix} (a_{11} \cdot \hat{j}_1) + (a_{12} \cdot \hat{j}_2) \\ (a_{21} \cdot \hat{j}_1) + (a_{22} \cdot \hat{j}_2) \end{bmatrix}$$
$$\LARGE = T_A(\vec{e_2}) = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix} \begin{bmatrix} 0 \\ 1 \end{bmatrix} = \begin{bmatrix} (a_{11} \cdot 0) + (a_{12} \cdot 1) \\ (a_{21} \cdot 0) + (a_{22} \cdot 1) \end{bmatrix} = \begin{bmatrix} a_{12} \\ a_{22}\end{bmatrix}$$
#### Linearity Properties of Linear Transformations
##### The Output Value of a Transformation (i.e. the image) of a Sum of Values is Equal to the Sum of the Output Values
$$\LARGE T(\vec{x} + \vec{y} + \vec{z}) = T(\vec{x}) + T(\vec{y}) + T(\vec{z})$$
##### The Output Value of a Transformation (i.e. the image) of a Scaling of a Value is Equal to the Scaling of the Output Value of a Transformation 
$$\LARGE T(\alpha\vec{x}) = \alpha T(\vec{x}), \quad \text{Where $\alpha$ is a scalar}$$
##### The [[Linear Combinations|Linear Combinations]] of Vectors is Equal to the Linear Combination of the Images of the Vectors
$$\LARGE T(\alpha \vec{x} + \beta \vec{y}) = \alpha T(\vec{x}) + \beta T(\vec{y}), \quad \text{Where $\alpha$ and $\beta$ are are scalars}$$
## The Position Vector is an Image of a Linear Transformation of a Basis Vector 
At their core, coordinates $(x,y,z)$ represent a **linear combination** of the basis vectors in a given coordinate system.
	In standard 3D Cartesian space, any point $(x,y,z)$ can be written as:
$$\LARGE \vec{r} = x \vec{i} + y \vec{j} + z \vec{k}$$

The coordinates $(x, y, z)$ are **not just static values**; they represent the **weights** in the linear combination of whatever the basis vectors are after the transformation $\LARGE T_A$​.
	In other words, the coordinates themselves remain the same numbers, but their interpretation is deeply connected to the basis vectors they're scaling. 
		Thus, the "coordinates" depend on the basis of the space, which may be transformed by $T_A$​.

Thus, your intuition is correct: **coordinate points** can be viewed fundamentally as 
$$\LARGE T_A(x \vec{e}_1) = x T_A(\vec{e}_1), \quad T_A(y\vec{e}_2) = y T_A(\vec{e}_2),\quad T_A(z \vec{e}_3) = z T_A(\vec{e}_3)$$
$$\LARGE T(x \vec{e}_1 + y \vec{e}_2) = x T(\vec{e}_1) + y T(\vec{e}_2)$$
$$\LARGE \quad \text{Where $x, y, z$ are a scalars}$$
This expression ties the coordinates directly to the transformed basis vectors, embodying how points and vectors "live" in the transformed space.



where i⃗=(1,0,0)\vec{i} = (1, 0, 0)i=(1,0,0), j⃗=(0,1,0)\vec{j} = (0, 1, 0)j​=(0,1,0), and k⃗=(0,0,1)\vec{k} = (0, 0, 1)k=(0,0,1) are the standard basis vectors.
#### Applying Linearity
### The Linear Combination of an Image of a Linear Transformation of a Basis Vector 
$$\LARGE T(x \vec{e}_1 + y \vec{e}_2) = x T(\vec{e}_1) + y T(\vec{e}_2), \quad \text{Where $x$ and $y$ are scalars}$$


## Points as Position Vectors

![[Pasted image 20240927064406.png|200]] ![[Pasted image 20240927064312.png|200]]
###### A Point/Position Vector
$$\LARGE \vec{x} = \mathbf{x} = (x_1, x_2, x_3) = (x, y, z) = \begin{bmatrix} x \\ y \\ z\end{bmatrix} = \begin{bmatrix} \Delta x_1 \\ \Delta x_2 \\\Delta x_3\end{bmatrix} = (x)\hat{i} + (y)\hat{j} + (z)\hat{k}$$



