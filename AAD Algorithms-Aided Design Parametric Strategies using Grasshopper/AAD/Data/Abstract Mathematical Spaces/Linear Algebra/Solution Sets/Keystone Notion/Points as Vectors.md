# Points as Vectors
A concept called Cartesian Vectors.
## Vectors
$$\LARGE \vec{v} = \mathbf{v} = (v_1, v_2, v_3) = \begin{bmatrix} v_1 \\ v_2 \\v_3 \end{bmatrix} = \begin{bmatrix} \Delta{v}_1 \\ \Delta v_2 \\ \Delta v_3 \end{bmatrix} = (v_1)\hat{i} + (v_2) \hat{j} + (v_3) \hat{k}$$
Abstract Mathematical Objects that contain two properties.
1. Direction
2. Magnitude
### Vectors Representation
##### A Vector as the Measure of Displacement
$$\LARGE \Delta{x}, \Delta{y}, \Delta{z}$$
Where what is being **displaced** are the "**points**" defined by the **component scalar functions**.
	More specifically, the scalars produced by the component scalar functions.

![[Pasted image 20240927062156.png|500]]
#### A Vector as a Tuples of Scalars (i.e. Coordinates)
$$\LARGE (v_1, v_2), \quad (v_1, v_2, v_3), \quad (v_1, v_2, \dots, v_n)$$
Where $\LARGE v_1, v_2, v_n$ are **[[#Component Scalar Functions of Vectors|component scalar functions]]**.
	Where **component scalar functions** are the coordinates that describe a "point".
#### A Vectors as a Linear Combination of Basis Vectors (i.e. Scaled Standard Unit Vectors)
$$\LARGE \vec{v} = \mathbf{v} = T_A(v_1,v_2,v_3) = (v_1)\hat{i} + (v_2) \hat{j} + (v_3) \hat{k}$$
Where $T_A$ is a Linear Transformation (i.e. a Vector-Valued Function).
	$T_A$ is composed of scalar-valued functions, $\LARGE (v_1)\hat{i}, \space (v_2) \hat{j}, \space (v_3) \hat{k}$.

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
## Cartesian Vectors
A Cartesian vector is a vector that is expressed in terms of its components along the Cartesian coordinate axes.
	In three-dimensional space, these components are along the $x$-axis, $y$-axis, and $z$-axis, represented by the unit vectors $\LARGE \vec{i} = (1, 0, 0), \vec{j} = (0, 1, 0), \vec{k} = (0, 0, 1)$.
		Cartesian vectors can represent various quantities, such as displacement, force, velocity, or acceleration, not just the position of a point.
##### Cartesian Vector Representation
A  $\LARGE \vec{r}$ in 3D space is often written as:
$$\LARGE \vec{r} = x \vec{i} + y \vec{j} + z \vec{k}$$
where:
- $x$, $y$, and $z$ are the **scalar components** of the vector, representing how much the vector extends in the direction of each of the Cartesian axes.
- The vector $\vec{r}$ originates from the origin and points to the location defined by the coordinates $(x, y, z)$.
### Position Vectors are Cartesian Vectors
When a Cartesian vector specifically represents the location of a point relative to the origin, it is called a **position vector**. 
	In other words, a position vector is a Cartesian vector **whose purpose is to describe a point's position in space**.
		**Not All Cartesian Vectors are Position Vectors:** Cartesian vectors can represent many other things (e.g., velocity, acceleration). 
			A vector like $\vec{v} = 3 \vec{i} + 4 \vec{j} - 2 \vec{k}$ could describe a [[Newton's Second Law#Velocity|Velocity]] or [[Newton's Second Law#Force|force]], and its interpretation depends on the context in which it's used.

A **position vector** specifically represents the location of a point in space **relative to the origin** of a coordinate system.
	This vector originates from the origin (0, 0, 0) and points to the location $(x, y, z)$.
		Its primary role is to "locate" a point in space using the Cartesian coordinate system.
			When you represent a point $(x,y,z)$ in a vector space, you are scaling the basis vectors $\vec{i}, \vec{j}, \vec{k}$ by the coordinates ,$x,y$, and $z$.

For a point $(x,y,z)$ in 3D space, the position vector is typically expressed as
$$\LARGE \vec{r} = x \vec{i} + y \vec{j} + z \vec{k}$$
## Mapping Coordinates to Position Vectors, Linear Transformations $T_A$
### Linear Transformation $T$, a [[Abstract Mathematical Spaces#Higher-Level Structures (Not Higher-Level Sets)|Vector-Valued Function]] 
Linear transformation $T$ takes any vector and maps it to the new vector (or space).
	This is a **vector-valued function** because its output is a vector in 3D space, constructed as a linear combination of the basis vectors $\LARGE \hat{i}, \hat{j}, \hat{k}$.
		The transformation $T$ takes a tuple of coordinates $(x,y,z)$ and returns a vector in space: 
$$\LARGE T(\vec{v}) = T(v_1,v_2,v_3) = T(x, y, z) = x \hat{i} + y \hat{j} + z \hat{k}$$
$$\LARGE T: \mathbb{R}^n \to \mathbb{R}^m, \quad T : (\vec{e_1}, \vec{e_2}, \vec{e_3}) \to T_A(\vec{e_1}) + T_A(\vec{e_2}) + T_A(\vec{e_3})$$
$$\LARGE Domain_{\space T} \subset \mathbb{R}^n,\quad  Codomain_{\space T} =\set{\mathbb{R}^m}, \quad Range_{\space T} \subset \mathbb{R}^m$$
- **$T$:** Refers to a linear transformation in a general sense.
- **$T_A$​:** Explicitly denotes the linear transformation associated with the matrix $A$. 
	- It’s a way to connect the transformation to its matrix representation.
#### The Linear Transformation of the Vector $\vec{v}$ as a Whole
The expression $\LARGE T_A(\vec{v})$ involves a **linear combination** of the input vector's components $(v_1, v_2, \dots, v_n​$)$ scaled by the elements of matrix $A$.
	Each row of $T_A(\vec{v})$ corresponds to a linear combination that represents a vector in $\LARGE \mathbb{R}^m$.

Each entry in the output vector can be broken down into a linear combination of the basis vectors in the output space:
$$\LARGE T_A(\vec{v}) = \sum_{i=1}^{m} \left( \sum_{j=1}^{n} a_{ij}v_j \right) \hat{e}_i$$
Here:
- **$\LARGE a_{ij}v_j$:** Represents the scaling of the $j$-th input component by the matrix element $a_{ij}$​.
- **$\LARGE \hat{e}_i$​:** Represents the standard basis vector in the output space ($\LARGE \mathbb{R}^m$).

$$\LARGE T : (\vec{v}) \to T_A(\vec{v})$$
$$\LARGE T_{A}(\vec{v}) = \begin{bmatrix} T_1(\vec{v}) \\ T_2(\vec{v}) \\ T_3(\vec{v}) \end{bmatrix}$$
Each $\LARGE T_i(\vec{v})$ is a **scalar component function** defined by the linear combination:
$$\LARGE T_i(\vec{v}) = a_{i1}v_1 + a_{i2}v_2 + \dots + a_{in}v_n$$
In this form, $T_A$​ produces an **output vector** whose components are scalar functions of the input coordinates.
	These scalar functions depend on both the matrix $A$ (through its entries $\LARGE a_{ij}$​) and the input vector $\LARGE \vec{v}$.
##### The Linear Transformation of a Basis Vector ***is*** a Matrix, $A$ 
The matrix $A$ containing $(x, y, z)$ defines a **linear transformation** because the resulting vector $T_A(\vec{v})$is a linear combination of the coordinates $x,y,z$ and the input vector's components.
	This setup aligns with the idea of a **vector-valued function**, where the output is a vector, and the function maps input vectors to other vectors through linear combinations involving $x,y,z$.

Suppose $\LARGE A$ is an $\LARGE m \times n$ matrix:
$$\LARGE A = \begin{bmatrix} a_{11} & a_{12} & \dots & a_{1n} \\ a_{21} & a_{22} & \dots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \dots & a_{mn} \end{bmatrix}$$

When this matrix acts on the vector $\LARGE\vec{v} = \begin{bmatrix} v_1 \\ v_2 \\ \dots \\ v_n \end{bmatrix}$,the result is:
$$\LARGE T_A(\vec{v}) = A \vec{v} = \begin{bmatrix} a_{11}v_1 + a_{12}v_2 + \dots + a_{1n}v_n \\ a_{21}v_1 + a_{22}v_2 + \dots + a_{2n}v_n \\ \vdots \\ a_{m1}v_1 + a_{m2}v_2 + \dots + a_{mn}v_n \end{bmatrix}$$
Suppose A is a **diagonal matrix** of the form:

$$\LARGE A = \begin{bmatrix} x & 0 & 0 \\ 0 & y & 0 \\ 0 & 0 & z \end{bmatrix}$$
Then, for an input vector $\LARGE \vec{v} = \begin{bmatrix} v_1 \\ v_2 \\ v_3 \end{bmatrix}$

$$\LARGE T_A(\vec{v}) = A \vec{v} = \begin{bmatrix} x \cdot v_1 \\ y \cdot v_2 \\ z \cdot v_3 \end{bmatrix}$$
Now, let’s express this in terms of the basis vectors:
$$\LARGE T_A(\vec{v}) = (x \cdot v_1) \hat{e}_1 + (y \cdot v_2) \hat{e}_2 + (z \cdot v_3) \hat{e}_3$$
Here:
- $\LARGE x \cdot v_1​$ scales the basis vector $\LARGE \hat{e}_1$,
- $\LARGE y \cdot v_2$ scales the basis vector $\LARGE \hat{e}_2$​,
- $\LARGE z \cdot v_3$​ scales the basis vector $\LARGE \hat{e}_3$​.
##### Each Component $\LARGE T_A(\vec{e_1}), T_A(\vec{e_2}), T_A(\vec{e_3})$ is itself a Linear Transformation/Vector Function
$$\LARGE T : (\vec{e_1}, \vec{e_2}, \vec{e_3}) \to T_A(\vec{e_1}) + T_A(\vec{e_2}) + T_A(\vec{e_3})$$
$$\LARGE T_{A}(\vec{e_1}) = A\vec{e_1}, \quad T_{A}(\vec{e_2}) = A\vec{e_2}, \quad T_{A}(\vec{e_3}) = A\vec{e_3}$$
$$\LARGE A = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix}, \quad \vec{e_1} = \begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \end{bmatrix} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \quad \vec{e}_2 = \begin{bmatrix} \hat{j}_1 \\ \hat{j}_2 \end{bmatrix} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}$$
$$\LARGE T_A(\vec{e_1}) = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix} \begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \end{bmatrix} = \begin{bmatrix} (a_{11} \cdot \hat{i}_1) + (a_{12} \cdot \hat{i}_2) \\ (a_{21} \cdot \hat{i}_1) + (a_{22} \cdot \hat{i}_2) \end{bmatrix}$$
$$\LARGE = T_A(\vec{e_1}) = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix} \begin{bmatrix} 1 \\ 0 \end{bmatrix} = \begin{bmatrix} (a_{11} \cdot 1) + (a_{12} \cdot 0) \\ (a_{21} \cdot 1) + (a_{22} \cdot 0) \end{bmatrix} = \begin{bmatrix} a_{11} \\ a_{21}\end{bmatrix}$$
$$\LARGE T_A(\vec{e_2}) = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix} \begin{bmatrix} \hat{j}_1 \\ \hat{j}_2 \end{bmatrix} = \begin{bmatrix} (a_{11} \cdot \hat{j}_1) + (a_{12} \cdot \hat{j}_2) \\ (a_{21} \cdot \hat{j}_1) + (a_{22} \cdot \hat{j}_2) \end{bmatrix}$$
$$\LARGE = T_A(\vec{e_2}) = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix} \begin{bmatrix} 0 \\ 1 \end{bmatrix} = \begin{bmatrix} (a_{11} \cdot 0) + (a_{12} \cdot 1) \\ (a_{21} \cdot 0) + (a_{22} \cdot 1) \end{bmatrix} = \begin{bmatrix} a_{12} \\ a_{22}\end{bmatrix}$$

#### Matrix $A$ as the Coordinates of a Vector $\large (x,y,z)$
$$\LARGE A = \begin{bmatrix} a_{11} \quad a_{12} \quad a_{13} \\ a_{21} \quad a_{22} \quad a_{23} \\ a_{31} \quad a_{32} \quad a_{33} \end{bmatrix} = \begin{bmatrix} x \quad 0 \quad 0 \\ 0 \quad y \quad 0 \\ 0 \quad 0 \quad z \end{bmatrix}$$
##### Again, Each $\LARGE T_A(\vec{\hat{i}}), T_A(\vec{\hat{j}}), T_A(\vec{\hat{k}})$ is itself a Linear Transformation/Vector Function
This diagonal matrix $A$ would then linearly scale each of the standard basis vectors $\hat{i}, \hat{j}, \hat{k}$ by the coordinates $x,y,z$ when applied to them: 
$$\large T_A(\vec{\hat{i}}) = A \vec{\hat{i}} = \begin{bmatrix} x & 0 & 0 \\ 0 & y & 0 \\ 0 & 0 & z \end{bmatrix} \begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \\ \hat{i}_3 \end{bmatrix} = \begin{bmatrix} (x \cdot \hat{i}_1) + (0 \cdot \hat{i}_1) +(0 \cdot \hat{i}_1) \\ (0 \cdot \hat{i}_2) + (y \cdot \hat{i}_2) +(0 \cdot \hat{i}_2) \\(0 \cdot \hat{i}_3) + (0 \cdot \hat{i}_3) +(z \cdot \hat{i}_3) \end{bmatrix}  =\begin{bmatrix} x \\ 0 \\ 0 \end{bmatrix}$$
$$\LARGE T_A(\vec{\hat{j}}) = A \vec{\hat{j}} = \begin{bmatrix} x & 0 & 0 \\ 0 & y & 0 \\ 0 & 0 & z \end{bmatrix} \begin{bmatrix} \hat{j}_1 \\ \hat{j}_2 \\ \hat{j}_3 \end{bmatrix} = \begin{bmatrix} 0 \cdot \hat{j}_1\\ y \cdot \hat{j}_2 \\ 0 \cdot \hat{j}_3 \end{bmatrix} = \begin{bmatrix} 0 \\ y \\ 0 \end{bmatrix}$$
$$\LARGE T_A(\vec{\hat{k}}) = A \vec{\hat{k}} = \begin{bmatrix} x & 0 & 0 \\ 0 & y & 0 \\ 0 & 0 & z \end{bmatrix} \begin{bmatrix} \hat{k}_1 \\ \hat{k}_2 \\ \hat{k}_3 \end{bmatrix} = \begin{bmatrix} 0 \cdot \hat{k}_1\\ 0 \cdot \hat{k}_2 \\ z \cdot \hat{k}_3 \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \\ z \end{bmatrix}$$
This, again, is a linear transformation and results in a new vector-valued output.
### The Component Scalar Functions of the Linear Transformation/Vector Function
#### Components of the Whole $T_A(\vec{v})$
$$\LARGE T_A(\vec{v}) = A \vec{v} = \begin{bmatrix} a_{11}v_1 + a_{12}v_2 + \dots + a_{1n}v_n \\ a_{21}v_1 + a_{22}v_2 + \dots + a_{2n}v_n \\ \vdots \\ a_{m1}v_1 + a_{m2}v_2 + \dots + a_{mn}v_n \end{bmatrix}$$
- Each **entry** in the resulting vector $\LARGE T_A(\vec{v})$ is a **linear combination** of the coordinates $v_1, v_2, \dots, v_n$​ of the input vector $\vec{v}$, scaled by the elements of the matrix $A$.

The **$\LARGE \textcolor{violet}{\text{Scalar-Valued Functions}}$** in this context are the individual linear combinations for each row in the resulting vector.
$$\LARGE T_{A}(\vec{v}) = \begin{bmatrix} T_1(\vec{v}) \\ T_2(\vec{v}) \\ T_3(\vec{v}) \end{bmatrix}$$
###### The first component (or "scalar function") is: 
$$\LARGE \textcolor{violet}{T_1(\vec{v}) = a_{11}v_1 + a_{12}v_2 + \dots + a_{1n}v_n}$$
###### The second component is:
$$\LARGE \textcolor{violet}{T_2(\vec{v}) = a_{21}v_1 + a_{22}v_2 + \dots + a_{2n}v_n}$$
###### Generally, the $i$-th component of the vector $T_A(\vec{v})$ is:
$$\LARGE \textcolor{violet}{T_i(\vec{v}) = a_{i1}v_1 + a_{i2}v_2 + \dots + a_{in}v_n}$$

These are **scalar-valued functions** of the coordinates $v_1, v_2, \dots, v_n$. 
	They represent how the linear transformation combines and scales the input coordinates to produce each component of the output vector.
#### The Scalar Component Functions $T_A(v_1), T_A(v_2), T_A(v_3)$
Where before, the Component Functions themselves were considered vector functions, due to their return type.
	When only one value is non-zero, then the function is taken as a scalar function producing only that one non-zero value.

The Component Scalar Functions are expressed in the $\LARGE T_A(\vec{\hat{i}}), T_A(\vec{\hat{j}}), T_A(\vec{\hat{k}})$.
	Specifically as the Linear Combinations that exist in the **Rows** of the transformation.
		So despite $\LARGE T_A(\vec{\hat{i}}), T_A(\vec{\hat{j}}), T_A(\vec{\hat{k}})$ being themselves Vector-Valued Functions (just as $T_A(\vec{v})$ as a whole Transformation of the vector containing those basis vectors), each is composed of $\LARGE \textcolor{violet}{\text{Scalar-Valued Functions}}$.
$$\LARGE T_A(\vec{i}) = \begin{bmatrix} \textcolor{violet}{T_{1_{_A}}(\vec{i}_1)} \\ \textcolor{violet}{T_{2_A}(\vec{i}_2)} \\ \textcolor{violet}{T_{3_A}(\vec{i}_3)} \end{bmatrix}$$
$$\large \textcolor{violet}{T_{1_A}(\vec{\hat{i}_1})} = A \vec{\hat{i}} = \begin{bmatrix} x & 0 & 0 \\ 0 & y & 0 \\ 0 & 0 & z \end{bmatrix} \begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \\ \hat{i}_3 \end{bmatrix} = \begin{bmatrix} \textcolor{violet}{(x \cdot \hat{i}_1) + (0 \cdot \hat{i}_1) +(0 \cdot \hat{i}_1) }\\ \textcolor{violet}{ (0 \cdot \hat{i}_2) + (y \cdot \hat{i}_2) +(0 \cdot \hat{i}_2)} \\ \textcolor{violet}{(0 \cdot \hat{i}_3) + (0 \cdot \hat{i}_3) +(z \cdot \hat{i}_3)} \end{bmatrix}  =\begin{bmatrix} x \\ 0 \\ 0 \end{bmatrix}$$
$$\LARGE = \textcolor{violet}{T_{1_A}(\vec{\hat{i}_1})} = x$$
$$\LARGE \textcolor{violet}{T_{2_A}(\vec{\hat{i}_2})} =\begin{bmatrix} 0 \cdot \hat{j}_1\\ y \cdot \hat{j}_2 \\ 0 \cdot \hat{j}_3 \end{bmatrix} = \begin{bmatrix} 0 \\ y \\ 0 \end{bmatrix}, \quad \textcolor{violet}{T_{2_A}(\vec{\hat{i}_2})} = y$$
$$\LARGE \textcolor{violet}{T_{3_A}(\vec{\hat{i}_3})} = \begin{bmatrix} 0 \cdot \hat{k}_1\\ 0 \cdot \hat{k}_2 \\ z \cdot \hat{k}_3 \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \\ z \end{bmatrix}, \quad \textcolor{violet}{T_{3_A}(\vec{\hat{i}_3})} = z$$
#### Linearity Properties of Linear Transformations
##### The Output Value of a Transformation (i.e. the image) of a Sum of Values is Equal to the Sum of the Output Values
$$\LARGE T(\vec{x} + \vec{y} + \vec{z}) = T(\vec{x}) + T(\vec{y}) + T(\vec{z})$$
##### The Output Value of a Transformation (i.e. the image) of a Scaling of a Value is Equal to the Scaling of the Output Value of a Transformation 
$$\LARGE T(\alpha\vec{x}) = \alpha T(\vec{x}), \quad \text{Where $\alpha$ is a scalar}$$
##### The [[Linear Combinations|Linear Combinations]] of Vectors is Equal to the Linear Combination of the Images of the Vectors
$$\LARGE T(\alpha \vec{x} + \beta \vec{y}) = \alpha T(\vec{x}) + \beta T(\vec{y}), \quad \text{Where $\alpha$ and $\beta$ are are scalars}$$
### The Position Vector is an Image of a Linear Transformation of a Basis Vector 
When you represent a point $(x,y,z)$ in a vector space, you are scaling the basis vectors $\vec{i}, \vec{j}, \vec{k}$ by the coordinates ,$x,y$, and $z$.
	This process can be seen as a **linear transformation** where the coordinates $(x, y, z)$ serve as the "inputs" that scale the basis vectors.

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
### 1. **Coordinates as Scaled Unit Basis Vectors:**

When you express a point (x,y,z)(x, y, z)(x,y,z) in 3D space, what you are doing is representing that point as a linear combination of the standard basis vectors e⃗1=(1,0,0)\vec{e}_1 = (1, 0, 0)e1​=(1,0,0), e⃗2=(0,1,0)\vec{e}_2 = (0, 1, 0)e2​=(0,1,0), and e⃗3=(0,0,1)\vec{e}_3 = (0, 0, 1)e3​=(0,0,1):

r⃗=xe⃗1+ye⃗2+ze⃗3.\vec{r} = x \vec{e}_1 + y \vec{e}_2 + z \vec{e}_3.r=xe1​+ye2​+ze3​.

Here’s the interpretation:

- **x⋅e⃗1x \cdot \vec{e}_1x⋅e1​:** This is a vector that points in the direction of the xxx-axis, scaled by the amount xxx.
- **y⋅e⃗2y \cdot \vec{e}_2y⋅e2​:** This is a vector that points in the direction of the yyy-axis, scaled by the amount yyy.
- **z⋅e⃗3z \cdot \vec{e}_3z⋅e3​:** This is a vector that points in the direction of the zzz-axis, scaled by the amount zzz.

In this sense, the coordinates (x,y,z)(x, y, z)(x,y,z) are indeed the **scalars** that multiply the **unit basis vectors** to position the point in space.

### 2. **The Linear Combination as a Position Vector:**

The expression:

r⃗=xe⃗1+ye⃗2+ze⃗3,\vec{r} = x \vec{e}_1 + y \vec{e}_2 + z \vec{e}_3,r=xe1​+ye2​+ze3​,

is a **position vector** that extends from the origin to the point (x,y,z)(x, y, z)(x,y,z) in 3D space. The coordinates x,y,zx, y, zx,y,z are the **scalars** that determine how much each basis vector contributes to the vector's direction and magnitude.

### 3. **Scaling as a Linear Transformation:**

The act of forming the vector xe⃗1+ye⃗2+ze⃗3x \vec{e}_1 + y \vec{e}_2 + z \vec{e}_3xe1​+ye2​+ze3​ from the coordinates (x,y,z)(x, y, z)(x,y,z) **is inherently a linear process**:

- A **linear transformation** can be understood as any process that involves scaling and combining basis vectors. In this case, the "transformation" takes the coordinates (x,y,z)(x, y, z)(x,y,z) and produces the position vector r⃗\vec{r}r.
- In matrix terms, if you think of the standard basis vectors as forming the columns of the identity matrix III, the operation: I[xyz]=xe⃗1+ye⃗2+ze⃗3,I \begin{bmatrix} x \\ y \\ z \end{bmatrix} = x \vec{e}_1 + y \vec{e}_2 + z \vec{e}_3,I​xyz​​=xe1​+ye2​+ze3​, shows that building the vector from its coordinates is itself a linear transformation.

### 4. **Understanding Your Question:**

- **Yes,** the coordinates (x,y,z)(x, y, z)(x,y,z) **are fundamentally the scalings** of the unit basis vectors:
    
    x=x⋅e⃗1,y=y⋅e⃗2,z=z⋅e⃗3.x = x \cdot \vec{e}_1, \quad y = y \cdot \vec{e}_2, \quad z = z \cdot \vec{e}_3.x=x⋅e1​,y=y⋅e2​,z=z⋅e3​.
- The position vector r⃗\vec{r}r in space is **constructed** by scaling the basis vectors by these coordinates and then adding them up.
    

### 5. **Scaling Process as a Linear Transformation:**

- You are correct in suggesting that this scaling process can be viewed as a linear transformation. If we have a matrix that represents a basis (in this case, the identity matrix for the standard basis vectors), the operation of multiplying the coordinates by this matrix is a linear transformation that maps the coordinates to a position vector.

### **Summary:**

So, **yes**, a point represented by the coordinates (x,y,z)(x, y, z)(x,y,z) **is fundamentally** the combination of the unit basis vectors scaled by the values x,y,zx, y, zx,y,z. Each coordinate x,y,zx, y, zx,y,z acts as a scalar that scales the corresponding unit basis vector:

x=x⋅e⃗1,y=y⋅e⃗2,z=z⋅e⃗3.x = x \cdot \vec{e}_1, \quad y = y \cdot \vec{e}_2, \quad z = z \cdot \vec{e}_3.x=x⋅e1​,y=y⋅e2​,z=z⋅e3​.

This representation is intrinsic to how linear algebra defines points and vectors in space. The scaling process is linear, hence aligning with the concept of linear transformations.


