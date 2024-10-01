# Points as Vectors
A concept called Cartesian Vectors.
## Vectors
$$\LARGE \vec{v} = \mathbf{v} = (v_1, v_2, v_3) = \begin{bmatrix} v_1 \\ v_2 \\v_3 \end{bmatrix} = \begin{bmatrix} \Delta{v}_1 \\ \Delta v_2 \\ \Delta v_3 \end{bmatrix} = (v_1)\hat{i} + (v_2) \hat{j} + (v_3) \hat{k}$$
Abstract Mathematical Objects that contain two properties.
1. Direction
2. Magnitude
## Vector Expression
The **Cartesian Form (i.e. scalar basis form)**, **tuple form**, and **bracket form** are all different ways of expressing the **same vector**. 
	They emphasize different aspects: the basis vectors, the coordinates, or the column structure used in linear algebra.
		The **diagonal matrix form** is a way of encoding the components of a vector as part of a transformation (specifically scaling). 
			While not strictly a vector in the traditional sense, it serves as a representation that dictates how to scale each axis.
##### A Vector as the Measure of Displacement
$$\LARGE \Delta{x}, \Delta{y}, \Delta{z}$$
Where what is being **displaced** are the "**points**" defined by the **component scalar functions**.
	More specifically, the scalars produced by the component scalar functions.

![[Pasted image 20240927062156.png|500]]
#### A Vector as a Tuples of Scalars (i.e. Coordinates)
$$\LARGE (v_1, v_2), \quad (v_1, v_2, v_3), \quad (v_1, v_2, \dots, v_n)$$
Where $\LARGE v_1, v_2, v_n$ are **[[#Component Scalar Functions of Vectors|component scalar functions]]**.
	Where **component scalar functions** are the coordinates that describe a "point".
### Tuple Form (Coordinate or Point Form)
Here, a vector is represented by an **ordered list of numbers** (its components), without explicitly mentioning the basis vectors:
$$\LARGE \vec{v} = (x, y, z)$$
- **Tuple:** The tuple simply lists the coordinates in an ordered form.
- **Implied Basis:** The form implies that the vector is with respect to a standard basis (typically $\LARGE \hat{i}, \hat{j}, \hat{k}$ in Cartesian coordinates).
- **Example:** The vector $(3,2,−1)$ implies a vector whose $x$-component is 3, $y$-component is 2, and $z$-component is -1.
### Bracket Form (Column or Row Vector)
Vectors can also be written in **matrix bracket notation**, commonly used in linear algebra:
$$\LARGE \vec{v} = \begin{bmatrix} x \\ y \\ z \end{bmatrix} \quad \text{or} \quad \vec{v} = \begin{bmatrix} x & y & z \end{bmatrix}$$

- **Column Vector:** $\begin{bmatrix} x \\ y \\ z \end{bmatrix}​$​​ is the standard way to represent vectors in linear transformations, especially when working with matrix multiplication.
- **Row Vector:** $\begin{bmatrix} x & y & z \end{bmatrix}$ is used in certain contexts, especially in matrix row operations or when dealing with dot products.
- **Example:** The vector $\begin{bmatrix} 3 \\ 2 \\ -1 \end{bmatrix}$​​ is equivalent to the tuple form $(3,2,−1)$ and the scalar basis form $\hat{i} + 2\hat{j} - \hat{k}$.
### A Vector is a Linear Combination of Basis Vectors of the Entire Vector Space
That is **any vector** can be **"reached"** by some **Linear Combination** of the **Standard Unit Vectors of a given Vector Space**.
$$\LARGE \vec{v} = \mathbf{v} = (v_1,v_2,v_3) = (x,y,z)$$
$$\LARGE T_A(v_1,v_2,v_3) = (v_1)\hat{i} + (v_2) \hat{j} + (v_3) \hat{k} = (x)\hat{i} + (y) \hat{j} + (z) \hat{k}$$
Where $T_A(v_1,v_2,v_3)$ is a Linear Transformation (i.e. a Vector-Valued Function) **applied to** the vector $\vec{v}$ in this Vector Space.
	Which are produced by taking the [[Data/Abstract Mathematical Spaces/Linear Algebra/Linearity/Dot Product|Dot Product]] of each component of vector $\vec{v}$ with the corresponding basis vector.
#### Cartesian Vector Form (i.e. Scalar Basis Form)
A Cartesian vector is a vector that is expressed in terms of Linear Combinations of its components along the Cartesian coordinate axes (i.e. Basis Vectors) defining the Vector Space.
	In three-dimensional space, these components are along the $x$-axis, $y$-axis, and $z$-axis, represented by the unit vectors $\LARGE \vec{i} = (1, 0, 0), \space \vec{j} = (0, 1, 0), \space \vec{k} = (0, 0, 1)$.
		Cartesian vectors can represent various quantities, such as displacement, force, velocity, or acceleration, not just the position of a point.
##### Cartesian Vector Representation
A  $\LARGE \vec{r}$ in 3D space is often written as:
$$\LARGE \vec{r} = x \vec{i} + y \vec{j} + z \vec{k}$$
where:
- **Components:** $x$, $y$, and $z$ are the **scalar components** of the vector, representing how much the vector extends in the direction of each of the Cartesian axes.
- **Basis Vectors:** i^,j^,k^\hat{i}, \hat{j}, \hat{k}i^,j^​,k^ are the unit vectors in the direction of the coordinate axes.
- The vector $\vec{r}$ originates from the origin and points to the location defined by the coordinates $(x, y, z)$.
### Position Vectors, $\vec{r}$, are Cartesian Vectors
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
### *But* the Linear Transformation of the Basis Vectors (thus the Entire Vector Space), Affects Every Linear Combination Applied to a Vector in the Space
###### Therefore, a Vector is a Linear Combination of the Image of the Basis Vectors.
I.e. A Vector scales the Image of the (i.e. Linear Transformation) of the Basis Vectors.
$$\large \textcolor{green}{T(}\textcolor{violet}{\vec{v}}\textcolor{green}{)} = \textcolor{green}{T_A(}\textcolor{red}{x}(\vec{e_1}) + \textcolor{red}{y}(\vec{e_2}) + \textcolor{red}{z}(\vec{e_3}) \textcolor{green}{)} = \textcolor{red}{x}\textcolor{green}{T_A(\vec{e_1})} + \textcolor{red}{y}\textcolor{green}{T_A(\vec{e_2})} + \textcolor{red}{z}\textcolor{green}{T_A(\vec{e_3})} = \textcolor{yellow}{x \hat{i} + y \hat{j} + z \hat{k}}$$
$$\LARGE \vec{v} = \mathbf{v} = (v_1, v_2, v_3) = \begin{bmatrix} v_1 \\ v_2 \\v_3 \end{bmatrix}$$
$$\LARGE (v_1) \hat{i} = v_1\begin{bmatrix} \hat{i}_1 \\\hat{i}_2 \\ \hat{i}_3\end{bmatrix}, \quad (v_2) \hat{j} = v_2\begin{bmatrix} \hat{j}_1 \\\hat{j}_2 \\ \hat{j}_3\end{bmatrix}, \quad (v_3) \hat{k} = v_3\begin{bmatrix} \hat{k}_1 \\\hat{k}_2 \\ \hat{k}_3\end{bmatrix}$$
$$\LARGE = (v_1) \hat{i} = v_1\begin{bmatrix} \hat{i}_1 \\\hat{i}_2 \\ \hat{i}_3\end{bmatrix}, \quad (v_2) \hat{j} = v_2\begin{bmatrix} \hat{j}_1 \\\hat{j}_2 \\ \hat{j}_3\end{bmatrix}, \quad (v_3) \hat{k} = v_3\begin{bmatrix} \hat{k}_1 \\\hat{k}_2 \\ \hat{k}_3\end{bmatrix}$$
$$\LARGE \vec{v}= (v_1,v_2,v_3) = (x,y,z) = (x(\vec{e_1}) + y(\vec{e_2}) + z(\vec{e_3}))$$
#### The Position Vector is an Image of a Linear Transformation Imposed By the Basis Vector 
When you represent a point $(x,y,z)$ in a vector space, you are scaling the basis vectors $\vec{i}, \vec{j}, \vec{k}$ by the coordinates $x,y$, and $z$.
	This process can be seen as a **linear transformation** where the coordinates $(x, y, z)$ serve as the "inputs" that scale the transformed basis vectors.

At their core, coordinates $(x,y,z)$ represent a **linear combination** of the basis vectors in a given coordinate system.
	In standard 3D Cartesian space, any point $(x,y,z)$ can be written as:
$$\LARGE \vec{r} = x \vec{i} + y \vec{j} + z \vec{k}$$
The coordinates $(x, y, z)$ are **not just static values**; they represent the **weights** in the linear combination of whatever the basis vectors are after the transformation $\LARGE T_A$​.
	In other words, the coordinates themselves remain the same numbers, but their interpretation is deeply connected to the basis vectors they're scaling. 
		Thus, the "coordinates" depend on the basis of the space, which may be transformed by $T_A$​.

**Coordinate points** can be viewed fundamentally as 
$$\LARGE T_A(x \vec{e}_1) = x T_A(\vec{e}_1), \quad T_A(y\vec{e}_2) = y T_A(\vec{e}_2),\quad T_A(z \vec{e}_3) = z T_A(\vec{e}_3)$$
$$\LARGE T(x \vec{e}_1 + y \vec{e}_2) = x T(\vec{e}_1) + y T(\vec{e}_2)$$
$$\LARGE \quad \text{Where $x, y, z$ are a scalars}$$
This expression ties the coordinates directly to the transformed basis vectors, embodying how points and vectors "live" in the transformed space.
## Standard Unit Vectors (Basis Vectors)
Are the most fundamental Vectors, containing component scalar functions that always produce the same constant scalars depending on the Basis Vector.
	The **define** the **Vector Space** they exist within.
##### The Basis Vector, $\LARGE \hat{i}$ aka $\LARGE \vec{e_1}$ (the $x$-Direction)
$$\large \mathbf{e}_1 = \vec{e}_1 = \mathbf{i} = \hat{i} = (\hat{i}_1, \hat{i}_2, \hat{i}_3) = \begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \\ \hat{i}_3 \end{bmatrix} = \begin{bmatrix} \Delta\hat{i}_1 \\ \Delta\hat{i}_2 \\ \Delta\hat{i}_3 \end{bmatrix}$$
$$\LARGE \hat{i} =  (\hat{i}_1 = 1, \space 
\hat{i}_2 = 0, \space \hat{i}_3 = 0) = \begin{bmatrix} 1 \\ 0 \\0 \end{bmatrix} = (1, 0, 0)$$
##### The Basis Vector, $\LARGE \hat{j}$ aka $\LARGE \vec{e_2}$ (the $y$-Direction)
$$\large \mathbf{e}_2 = \vec{e}_2 = \mathbf{j} = \hat{j} = (\hat{j}_1, \hat{j}_2, \hat{j}_3) = \begin{bmatrix} \hat{j}_1 \\ \hat{j}_2 \\\hat{j}_3 \end{bmatrix}  = \begin{bmatrix} \Delta\hat{j}_1 \\ \Delta\hat{j}_2 \\ \Delta\hat{j}_3 \end{bmatrix}$$
$$\LARGE \hat{j} = (\hat{j}_1 = 0, \space \hat{j}_2 = 1, \space  \hat{j}_3=0) = \begin{bmatrix} 0 \\ 1 \\0 \end{bmatrix} = (0,1,0)$$
##### The Basis Vector, $\LARGE \hat{k}$ aka $\LARGE \vec{e_3}$ (the $z$-Direction)
$$\large \mathbf{e}_3 = \vec{e}_3 = \mathbf{k} =  \hat{k} = (\hat{k}_1, \hat{k}_2, \hat{k}_3) = \begin{bmatrix} \hat{k}_1 \\ \hat{k}_2 \\\hat{k}_3 \end{bmatrix} = \begin{bmatrix} \Delta\hat{k}_1 \\ \Delta\hat{k}_2 \\ \Delta\hat{k}_3 \end{bmatrix}$$
$$\LARGE \hat{k} = (\hat{k}_1= 0,\space \hat{k}_2=0,\space \hat{k}_1=1)= \begin{bmatrix} 0 \\ 0 \\1 \end{bmatrix} = (0, 0, 1)$$
## $\text{\textcolor{green}{Linear Transformation} \textcolor{violet}{Applied to the Basis Vectors}}$ (Low Level)
The purpose of transforming the **basis vectors** specifically is to set the "rules" or "instructions" for how the entire space changes.
	Since every vector in the vector space can be expressed as a linear combination of the basis vectors, transforming these basis vectors defines how any vector in the space will be altered by the transformation.
$$\LARGE T: \textcolor{violet}{\mathbb{R}^n} \to \textcolor{yellow}{\mathbb{R}^m}, \quad \textcolor{teal}{T} : \textcolor{violet}{(\vec{e_1}, \vec{e_2}, \vec{e_3})} \to \textcolor{yellow}{T_A(\vec{e_1}) + T_A(\vec{e_2}) + T_A(\vec{e_3})}$$
$$\LARGE \textcolor{violet}{Domain_{\space T} \subset \mathbb{R}^n},\quad  \textcolor{yellow}{Codomain_{\space T} =\set{\mathbb{R}^m}}, \quad Range_{\space T} \subset \mathbb{R}^m$$
- **$\textcolor{green}{T}$:** Refers to a linear transformation in a general sense.
- **$\textcolor{teal}{T_A}$​:** The Transformation Operator.
	- Explicitly denotes the linear transformation associated with the matrix $A$. 
	- It’s a way to connect the transformation to its matrix representation.
###### The $\textcolor{violet}{\text{Input}}$ to the Linear Transformation, $\LARGE \vec{e_i}$
The input to the transformation $T$ is are **three Standard Unit Vectors** $\LARGE \textcolor{violet}{\vec{e_1}, \vec{e_2}, \vec{e_3}}$ in $\mathbb{R}^3$.
###### The $\textcolor{yellow}{\text{Output}}$ (i.e. Images) of the Linear Transformations, $\LARGE \textcolor{yellow}{T_A(\vec{e_1}), T_A(\vec{e_2}), T_A(\vec{e_3})}$
The output are three new vector Images formed by this linear combination of the basis vectors.
###### The $\textcolor{green}{\text{Mapping}}$ of the Linear Transformation, $\LARGE \textcolor{green}{T : (\vec{e_1}, \vec{e_2}, \vec{e_3}) \to T_A(\vec{e_1}, T_A\vec{e_2}, T_A\vec{e_3})}$
The linear transformation $T$ takes the three input basis vectors $(\vec{e_1},\vec{e_2},\vec{e_3})$ and construct three new vectors as linear combinations of the standard basis vectors.
	The components of the Transformation are Linear Combinations.
###### The $\textcolor{teal}{\text{Mapping Operator}}$, $\LARGE T_A$
The matrix $A$ **encodes the rules** of the transformation. 
	It dictates how every input vector $\vec{v}$ is changed when the linear transformation $TA$​ is applied.
		 The entries of the matrix determine the nature of the transformation, such as scaling, rotating, reflecting, shearing, or mixing the components of the input vector.
### Each $\LARGE T_A(\vec{e_1}), T_A(\vec{e_2}), T_A(\vec{e_3})$ is Itself a Linear Transformation (of a Basis Vector)
$$\LARGE T: \textcolor{violet}{\mathbb{R}^n} \to \textcolor{yellow}{\mathbb{R}^m}, \quad \textcolor{teal}{T} : \textcolor{violet}{(\vec{e_1}, \vec{e_2}, \vec{e_3})} \to \textcolor{yellow}{T_A(\vec{e_1}) + T_A(\vec{e_2}) + T_A(\vec{e_3})}$$
$$\LARGE \textcolor{teal}{T}\textcolor{violet}{(\vec{e_1} + \vec{e_2} + \vec{e_3})} = \textcolor{yellow}{T_A(\vec{e_1}) + T_A(\vec{e_2}) + T_A(\vec{e_3})}$$
$$\LARGE T_{A}(\vec{e_1}) = A\vec{e_1}, \quad T_{A}(\vec{e_2}) = A\vec{e_2}, \quad T_{A}(\vec{e_3}) = A\vec{e_3}$$
$$\LARGE \textcolor{green}{A = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix}}, \quad \textcolor{violet}{\vec{e_1} = \begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \end{bmatrix} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}}, \quad \textcolor{violet}{\vec{e}_2 = \begin{bmatrix} \hat{j}_1 \\ \hat{j}_2 \end{bmatrix} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}}$$
$$\LARGE \textcolor{yellow}{T_A(\vec{e_1})} = \textcolor{green}{\begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix}} \textcolor{violet}{\begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \end{bmatrix}} = \textcolor{yellow}{\begin{bmatrix} (a_{11} \cdot \hat{i}_1) + (a_{12} \cdot \hat{i}_2) \\ (a_{21} \cdot \hat{i}_1) + (a_{22} \cdot \hat{i}_2) \end{bmatrix}}$$
$$\LARGE = \textcolor{yellow}{T_A(\vec{e_1}) }= \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix} \begin{bmatrix} 1 \\ 0 \end{bmatrix} = \begin{bmatrix} (a_{11} \cdot 1) + (a_{12} \cdot 0) \\ (a_{21} \cdot 1) + (a_{22} \cdot 0) \end{bmatrix} = \textcolor{yellow}{\begin{bmatrix} a_{11} \\ a_{21}\end{bmatrix}}$$
$$\LARGE \textcolor{yellow}{T_A(\vec{e_2})} = \textcolor{green}{\begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix}} \textcolor{violet}{\begin{bmatrix} \hat{j}_1 \\ \hat{j}_2 \end{bmatrix}} = \textcolor{yellow}{\begin{bmatrix} (a_{11} \cdot \hat{j}_1) + (a_{12} \cdot \hat{j}_2) \\ (a_{21} \cdot \hat{j}_1) + (a_{22} \cdot \hat{j}_2) \end{bmatrix}}$$
$$\LARGE = \textcolor{yellow}{T_A(\vec{e_2})} = \begin{bmatrix} a_{11} \quad a_{12} \\ a_{21} \quad a_{22} \end{bmatrix} \begin{bmatrix} 0 \\ 1 \end{bmatrix} = \begin{bmatrix} (a_{11} \cdot 0) + (a_{12} \cdot 1) \\ (a_{21} \cdot 0) + (a_{22} \cdot 1) \end{bmatrix} = \textcolor{yellow}{\begin{bmatrix} a_{12} \\ a_{22}\end{bmatrix}}$$
##### And Each **Row** (i.e. component) of the Linear Transformation of the Basis Vectors, is a Linear Combination (i.e. a Scalar Function)
Here is the expression converted to LaTeX form:
$$\LARGE T_A(\vec{e}_j) = \sum_{i=1}^{m} a_{ij} \hat{e}_i.$$

- $\LARGE T_A(\vec{e}_j)$: Represents the transformation of the $j$-th standard basis vector.
- $\LARGE \sum_{i=1}^{m} a_{ij} \hat{e}_i$: The result is a linear combination of the basis vectors in the codomain, where the coefficients $\LARGE a_{ij}$ come from the matrix  $A$.
### The Role of Matrix, $A$ of $T_A$
The matrix $A$ **encodes the rules** of the transformation. 
	It dictates how every Basis Vector is changed when the linear transformation $T_A$ is applied.
		 The entries of the matrix determine the nature of the transformation, such as scaling, rotating, reflecting, shearing, or mixing the components of the Basis Vector.
##### As a Transformative Map
The matrix $A$ is the concrete, numerical representation of the linear transformation $T_A$. 
	It defines the "rules" of how vectors in the input space are changed when they are mapped to the output space.

The matrix $A$ dictates **how** the input coordinates are transformed. 
	The form of the matrix $A$ does, in a way, represent the "structure" or "form" of the output vector.
		The matrix $A$ determines the linear combination of basis vectors that defines the output vector in the space.

Suppose $\LARGE A$ is an $\LARGE m \times n$ matrix:
$$\LARGE A = \begin{bmatrix} a_{11} & a_{12} & \dots & a_{1n} \\ a_{21} & a_{22} & \dots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \dots & a_{mn} \end{bmatrix}$$
When this matrix acts on the basis vector $\LARGE\hat{i} = \begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \\ \dots \\ \hat{i_n} \end{bmatrix}$,the result is:
$$\LARGE T_A(\hat{i}) = \begin{bmatrix} a_{11}\hat{i}_1 + a_{12}\hat{i}_2 + \dots + a_{1n}\hat{i}_n \\ a_{21}\hat{i}_1 + a_{22}\hat{i}_2 + \dots + a_{2n}\hat{i}_n \\ \vdots \\ a_{m1}\hat{i}_1 + a_{m2}\hat{i}_2 + \dots + a_{mn}\hat{i}_n \end{bmatrix}$$
##### As a Collection of Basis Transformations
The columns of $A$ show how the transformation affects the standard basis vectors of the input space, effectively describing how the entire space is transformed.
##### Basis Vector Mapping
The columns of the matrix $A$ represent how the transformation $T_A$$​ affects the standard basis vectors. 
	In an $n$-dimensional space:
		- The first column of $A$ describes how the basis vector $\LARGE \hat{i}_1 = (1, 0, \dots, 0)$ is transformed.
		- The second column describes the transformation of $\LARGE\hat{i}_2 = (0, 1, \dots, 0)$.
		- And so on for all $n$ columns.

For example, if $a$ is a $3 \times 3$ matrix:
$$\LARGE A = \begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{bmatrix}$$

the columns $\LARGE\begin{bmatrix} a_{11} \\ a_{21} \\ a_{31} \end{bmatrix}, \begin{bmatrix} a_{12} \\ a_{22} \\ a_{32} \end{bmatrix}, \begin{bmatrix} a_{13} \\ a_{23} \\ a_{33} \end{bmatrix}​$​​​ represent the images of the standard basis vectors $\hat{i}, \hat{j}$, and $\hat{k}$ under the transformation.
##### The Image of a Linear Transformation of a Basis Vector ***are*** a Vectors, $T_A$
**Each Basis Vector** essentially **associates** with a **specific column** of the **Matrix $A$**.
	Thus the columns of Matrix $A$ are responsible for transforming a corresponding Basis Vector. 
		**Each Row** is a **Linear Combination** (i.e. a Scalar Function).
$$\LARGE \vec{e_1} = \hat{i} = \textcolor{violet}{\begin{bmatrix} 1 \\ 0 \\0 \end{bmatrix}}$$
$$\large \textcolor{yellow}{T_A(\hat{i})} = \textcolor{green}{\begin{bmatrix} a_{11} \quad a_{12} \quad a_{13} \\ a_{21} \quad a_{22} \quad a_{23} \\ a_{31} \quad a_{32} \quad a_{33}\end{bmatrix}} \textcolor{violet}{\begin{bmatrix} \hat{i}_1 \\ \hat{i}_2 \\ \hat{i}_3 \end{bmatrix}} = \textcolor{yellow}{\begin{bmatrix} (\hat{i}_1 \cdot a_{11}) + (\hat{i}_2 \cdot a_{12}) + (\hat{i}_3 \cdot a_{13}) \\ (\hat{i}_1 \cdot a_{21}) + (\hat{i}_2 \cdot a_{22}) + (\hat{i}_3 \cdot a_{23}) \\ (\hat{i}_1 \cdot a_{31}) + (\hat{i}_2 \cdot a_{32}) + (\hat{i}_3 \cdot a_{33})  \end{bmatrix} } =\textcolor{yellow}{\begin{bmatrix}  \hat{i}_1 \cdot a_{11} \\  \hat{i}_1 \cdot a_{21} \\  \hat{i}_1 \cdot a_{31} \end{bmatrix}}$$
$$\LARGE \vec{e_2} = \hat{j} = \textcolor{violet}{\begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix}}$$
$$\large \textcolor{yellow}{T_A(\hat{j})} = \textcolor{green}{\begin{bmatrix} a_{11} \quad a_{12} \quad a_{13} \\ a_{21} \quad a_{22} \quad a_{23} \\ a_{31} \quad a_{32} \quad a_{33}\end{bmatrix}} \textcolor{violet}{\begin{bmatrix} \hat{j}_1 \\ \hat{j}_2 \\ \hat{j}_3 \end{bmatrix}} = \textcolor{yellow}{\begin{bmatrix} (\hat{j}_1 \cdot a_{11}) + (\hat{j}_2 \cdot a_{12}) + (\hat{j}_3 \cdot a_{13}) \\ (\hat{j}_1 \cdot a_{21}) + (\hat{j}_2 \cdot a_{22}) + (\hat{j}_3 \cdot a_{23}) \\ (\hat{j}_1 \cdot a_{31}) + (\hat{j}_2 \cdot a_{32}) + (\hat{j}_3 \cdot a_{33})  \end{bmatrix} } = \textcolor{yellow}{\begin{bmatrix} (\hat{j}_2 \cdot a_{12}) \\ (\hat{j}_2 \cdot a_{22}) \\ (\hat{j}_2 \cdot a_{32}) \end{bmatrix}}$$
$$\LARGE \vec{e_3} = \hat{k} =\textcolor{violet} {\begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}}$$
$$\large \textcolor{yellow}{T_A(\hat{k})} = \textcolor{green}{\begin{bmatrix} a_{11} \quad a_{12} \quad a_{13} \\ a_{21} \quad a_{22} \quad a_{23} \\ a_{31} \quad a_{32} \quad a_{33}\end{bmatrix}} \textcolor{violet}{\begin{bmatrix} \hat{k}_1 \\ \hat{k}_2 \\ \hat{k}_3 \end{bmatrix}} = \textcolor{yellow}{\begin{bmatrix} (\hat{k}_1 \cdot a_{11}) + (\hat{k}_2 \cdot a_{12}) + (\hat{k}_3 \cdot a_{13}) \\ (\hat{k}_1 \cdot a_{21}) + (\hat{k}_2 \cdot a_{22}) + (\hat{k}_3 \cdot a_{23}) \\ (\hat{k}_1 \cdot a_{31}) + (\hat{k}_2 \cdot a_{32}) + (\hat{k}_3 \cdot a_{33})  \end{bmatrix} } =\textcolor{yellow}{\begin{bmatrix} (\hat{k}_3 \cdot a_{13}) \\ (\hat{k}_3 \cdot a_{23}) \\ (\hat{k}_3 \cdot a_{33}) \end{bmatrix}}$$
These result in a new output image vectors.
	These new Matrices $A$ of the Transformed Basis Vectors, can be used to subsequently transform any Vectors in this new space. 
## $\text{\textcolor{green}{Linear Transformation} \textcolor{violet}{Applied to a Vector, }} \textcolor{violet}{\vec{v}}$ (High Level)
The Idea is that, if a Vector Space is itself transformed that is its Basis Vectors are linearly Transformed, then the vectors within that original non transformed space, will then be transformed according to the linear transformation of the space they exist within. 
###### Remember A Vector is a Linear Combination of Basis Vectors (i.e. Scaled Standard Unit Vectors)
$$\LARGE \textcolor{violet}{\vec{v} = (x,y,z)}$$
$$\LARGE \textcolor{violet}{\vec{v} = \mathbf{v}} = \textcolor{teal}{T_A(}\textcolor{violet}{x,y,z}\textcolor{teal}{)} = \textcolor{teal}{T}\textcolor{violet}{\begin{bmatrix} x \\ y\\ z \end{bmatrix}}$$
$$\LARGE = \textcolor{teal}{T}(\textcolor{violet}{x}(\textcolor{green}{\vec{e_1}}) + \textcolor{violet}{y}(\textcolor{green}{\vec{e_2}}) +\textcolor{violet}{z}(\textcolor{green}{\vec{e_3}}))$$
###### Remember that the Image of the Transformation is then Determined by the Image of the Basis Vectors, $(\vec{e_1}, \vec{e_2}, \vec{e_3})$.
Where $\LARGE \hat{i}, \hat{j}, \hat{k}$ have been transformed by $T_A$.
	After the image is produced, the vector containing the components $x,y,z$ (as scalars) is Linearly Transformed by the output image of the transformed basis vectors, $T_A$. 
		I.e. The Linear Transformation of a vector (some non-basis vector) is the Linear Combination of the transformed basis vectors with the components of the vector now being transformed.
$$\LARGE \textcolor{green}{T(}\textcolor{violet}{\vec{v}}\textcolor{green}{)} = \textcolor{green}{T_A(}\textcolor{violet}{x}(\textcolor{green}{\vec{e_1}}) + \textcolor{violet}{y}(\textcolor{green}{\vec{e_2}}) + \textcolor{violet}{z}(\textcolor{green}{\vec{e_3}}) \textcolor{green}{)} = \textcolor{violet}{x}\textcolor{green}{T_A(\vec{e_1})} + \textcolor{violet}{y}\textcolor{green}{T_A(\vec{e_2})} + \textcolor{violet}{z}\textcolor{green}{T_A(\vec{e_3})}$$
$$\LARGE = \textcolor{violet}{x} \textcolor{green}{\begin{bmatrix}  \hat{i}_1 \cdot a_{11} \\  \hat{i}_1 \cdot a_{21} \\  \hat{i}_1 \cdot a_{31} \end{bmatrix}} + \textcolor{violet}{y} \textcolor{green}{\begin{bmatrix} (\hat{j}_2 \cdot a_{12}) \\ (\hat{j}_2 \cdot a_{22}) \\ (\hat{j}_2 \cdot a_{32}) \end{bmatrix}} + \textcolor{violet}{z} \textcolor{green}{\begin{bmatrix} (\hat{k}_3 \cdot a_{13}) \\ (\hat{k}_3 \cdot a_{23}) \\ (\hat{k}_3 \cdot a_{33}) \end{bmatrix}}$$
$$\LARGE = \textcolor{yellow}{x \hat{i} + y \hat{j} + z \hat{k}}$$
###### The $\textcolor{violet}{\text{Input}}$ to the Linear Transformation, $\LARGE \vec{v}$
**The Input** to the transformation $T$ is a **vector** $\vec{v} = (x, y, z)$ in $\mathbb{R}^3$.
	This vector can be thought of as having three components, which are the coordinates $x,y,z$ with respect to the standard basis vectors $\hat{i}, \hat{j}, \hat{k}$.
		I.e. This input vector has a shorthand represented by the a corresponding "point" $(x,y,z)$ that is associated with that input Position Vector.
###### The $\textcolor{yellow}{\text{Output}}$ (i.e. Image) of the Linear Transformation, $\LARGE T_A(\vec{v})$
The result is a new vector formed by this linear combination of the basis vectors.
	This new vector is either within the same space or a different space, depending on defined codomain. 
###### The $\textcolor{green}{\text{Mapping of the Linear Transformation}}$, $\LARGE T : (\vec{v}) \to T_A(\vec{v})$
The linear transformation $T$ takes the input coordinates $(x, y, z)$ and constructs a vector as a linear combination of the standard basis vectors.
	The Linear Transformations maps the three previously Vector Images of the Basis Vectors, expressed as $\LARGE T(\vec{e_1}), T(\vec{e_2}), T(\vec{e_3})$. 
		Where each is a linear combination of the Basis Vectors and the corresponding columns of the original Matrix $A$.
			This results in a new vector in the vector space.
				**Scaling:** Each component $x,y,z$ of the input vector scales its corresponding basis vector.
				**Direction:** The resulting vector $\hat{i} + y \hat{j} + z \hat{k}$ points in the direction defined by the combination of scaled basis vectors.
###### The $\textcolor{teal}{\text{Mapping Operator}}$, $\LARGE T_A(\vec{e_i})$
The **Vectors** $T_A(\vec{e_i})$ **encodes the rules** of the transformation as defined by the Basis Vectors. 
	It dictates how every input vector $\vec{v}$ is changed when the linear transformation $TA$​ is applied.
		 The entries of the matrix determine the nature of the transformation, such as scaling, rotating, reflecting, shearing, or mixing the components of the input vector.
### Linear Transformations Applied to Vectors are Defined by Linear Combinations of Basis Vectors
###### Therefore, the Linear Transformations Applied to Vectors, **depend on** the Images of the Transformed Basis Vectors
Linear Transformations of the Basis Vectors occur **prior** to any additional higher level Linear Transformations of a vector by these output images.

Each entry in the output vector can be broken down into a linear combination of the basis vectors in the output space:
$$\LARGE T_A(\vec{v}) = \sum_{j=1}^{n} v_j \left( \sum_{i=1}^{m} a_{ij} \hat{e}_i \right)$$
$$\LARGE =T_A(\vec{v}) = \sum_{i=1}^{m} \left( \sum_{j=1}^{n} a_{ij} v_j \right) \hat{e}_i$$
Here:
- **$\LARGE a_{ij}v_j$:** Represents the scaling of the $j$-th input component by the matrix ($T_A$) element $a_{ij}$​.
- **$\LARGE \hat{e}_i$​:** Represents the standard basis vector in the output space ($\LARGE \mathbb{R}^m$).
### The Three Vector Images $T_A(\vec{e_1}), T_A(\vec{e_2}), T_A(\vec{e_3})$ (of Transformed Basis Vectors)
Which is what transforms the Vectors in this Space.
###### Linear Combination of the Images of the Basis Vectors
When $T_A$​ acts on a general vector $\vec{v} = \begin{bmatrix} v_1 \\ v_2 \\ v_3 \end{bmatrix}$, the output vector is:
$$\LARGE \textcolor{violet}{T_A(\vec{v})} = \textcolor{violet}{v_1} \textcolor{green}{\begin{bmatrix}  \hat{i}_1 \cdot a_{11} \\  \hat{i}_1 \cdot a_{21} \\  \hat{i}_1 \cdot a_{31} \end{bmatrix}} + \textcolor{violet}{v_2} \textcolor{green}{\begin{bmatrix} (\hat{j}_2 \cdot a_{12}) \\ (\hat{j}_2 \cdot a_{22}) \\ (\hat{j}_2 \cdot a_{32}) \end{bmatrix}} + \textcolor{violet}{v_3} \textcolor{green}{\begin{bmatrix} (\hat{k}_3 \cdot a_{13}) \\ (\hat{k}_3 \cdot a_{23}) \\ (\hat{k}_3 \cdot a_{33}) \end{bmatrix}}$$

This shows that the transformation scales and combines the columns of $A$ according to the components $\LARGE v_1, v_2, v_3$​ of the input vector.
###### The Vector Image $T_A(\vec{e_i})$ as a Set of Instructions
The Vector Image $T_A(\vec{e_i})$ tells you **how** to construct the output vector $T_A(\vec{v})$ from the input vector $T_A\vec{e_i}$.
	When you multiply $T_A(\vec{e_i})$ by $\vec{v}$, you are effectively taking a weighted sum of the columns of $A$ using the components of $\vec{v}$ as weights:
		This shows how each coordinate of $\vec{v}$ contributes to the resulting output vector according to the columns of $A$.
### Components of the Whole $T_A(\vec{v})$
$$\LARGE T : (\vec{v}) \to T_A(\vec{v})$$
Each $\LARGE T_i(\vec{v})$ (i.e. each "row" of $T_A(\vec{v})$) is a **scalar component function** defined by the linear combination of the input vector $\vec{v}$, scaled by the elements of the matrix $A$.:
$$\LARGE T_i(\vec{v}) = a_{i1}v_1 \cdot \vec{e_1} + a_{i2}v_2 \cdot \vec{e_2}+ \dots + a_{in}v_n \cdot \vec{e_n}$$
$$\LARGE \textcolor{violet}{T_A(\vec{v})} = \textcolor{violet}{v_1} \textcolor{green}{\begin{bmatrix}  \hat{i}_1 \cdot a_{11} \\  \hat{i}_1 \cdot a_{21} \\  \hat{i}_1 \cdot a_{31} \end{bmatrix}} + \textcolor{violet}{v_2} \textcolor{green}{\begin{bmatrix} (\hat{j}_2 \cdot a_{12}) \\ (\hat{j}_2 \cdot a_{22}) \\ (\hat{j}_2 \cdot a_{32}) \end{bmatrix}} + \textcolor{violet}{v_3} \textcolor{green}{\begin{bmatrix} (\hat{k}_3 \cdot a_{13}) \\ (\hat{k}_3 \cdot a_{23}) \\ (\hat{k}_3 \cdot a_{33}) \end{bmatrix}}$$
$$\LARGE T_A(\textcolor{violet}{\vec{v}}) = \begin{bmatrix} (\textcolor{violet}{v_1}\cdot \textcolor{green}{\hat{i}_1a_{11}}) + (\textcolor{violet}{v_2}\cdot \textcolor{green}{\hat{i}_2a_{12}}) + \dots + (\textcolor{violet}{v_n} \cdot \textcolor{green}{\hat{i}_na_{1n}}) \\ (\textcolor{violet}{v_1} \cdot \textcolor{green}{\hat{i}_1 a_{21}}) + (\textcolor{violet}{v_2} \cdot \textcolor{green}{\hat{i}_2a_{22}}) + \dots + (\textcolor{violet}{v_n} \cdot \textcolor{green}{\hat{i}_na_{2n}}) \\ \vdots \\ (\textcolor{violet}{v_1} \cdot \textcolor{green}{\hat{i}_1a_{m1}}) + (\textcolor{violet}{v_2} \cdot \textcolor{green}{\hat{i}_2a_{m2}}) + \dots + (\textcolor{violet}{v_n} \cdot \textcolor{green}{\hat{i}_n a_{mn}}) \end{bmatrix}$$
- Each **row entry** in the resulting vector $\LARGE T_A(\vec{v})$ is a **linear combination** of the coordinates $v_1, v_2, \dots, v_n$​ of the input vector $\vec{v}$, scaled by the elements of the matrix $A$.

The **$\LARGE \textcolor{violet}{\text{Scalar-Valued Functions}}$** in this context are the individual linear combinations for each row in the resulting vector.

$$\LARGE T_{A}(\vec{v}) = \begin{bmatrix} T_1(\vec{v}) \\ T_2(\vec{v}) \\ T_3(\vec{v}) \end{bmatrix}$$
###### The first component (or "scalar function") is: 
$$\LARGE \textcolor{violet}{T_1(\vec{v}) = a_{11}v_1 + a_{12}v_2 + \dots + a_{1n}v_n}$$
###### The second component is:
$$\LARGE \textcolor{violet}{T_2(\vec{v}) = a_{21}v_1 + a_{22}v_2 + \dots + a_{2n}v_n}$$
###### Generally, the $i$-th component of the vector $T_A(\vec{v})$ is:
$$\LARGE \textcolor{violet}{T_i(\vec{v}) = a_{i1}v_1 + a_{i2}v_2 + \dots + a_{in}v_n}$$

In this form, $T_A$​ produces an **output vector** whose components are scalar functions of the input coordinates.
	These scalar functions depend on both the matrix $A$ (through its entries $\LARGE a_{ij}$​) and the input vector $\LARGE \vec{v}$.
#### Linearity Properties of Linear Transformations
##### The Output Value of a Transformation (i.e. the image) of a Sum of Values is Equal to the Sum of the Output Values
$$\LARGE T(\vec{x} + \vec{y} + \vec{z}) = T(\vec{x}) + T(\vec{y}) + T(\vec{z})$$
##### The Output Value of a Transformation (i.e. the image) of a Scaling of a Value is Equal to the Scaling of the Output Value of a Transformation 
$$\LARGE T(\alpha\vec{x}) = \alpha T(\vec{x}), \quad \text{Where $\alpha$ is a scalar}$$
##### The [[Linear Combinations|Linear Combinations]] of Vectors is Equal to the Linear Combination of the Images of the Vectors
$$\LARGE T(\alpha \vec{x} + \beta \vec{y}) = \alpha T(\vec{x}) + \beta T(\vec{y}), \quad \text{Where $\alpha$ and $\beta$ are are scalars}$$
## The Derivation of the Standard Form Line Equation 
A line $ax+by =c$ as a set of position vectors that have a perpendicular distance from origin along the normal vector that is given by c over the magnitude of the normal vector.


The equation of a line in 2D space is a **formal constraint** that describes a **set of values**, and **geometrically** defines those set of points to lie on a line 2D space.
$$\LARGE ax + by = c$$
Where $a,b$, and $c$ are constants, and $(x,y)$ are coordinates in the 2D plane.
	$c$ is a constant that determines the line's position relative to the origin.
		This equation defines a relationship between $x$ and $y$ that all points on the line satisfy. 
			Geometrically, $(a,b)$ represents a vector perpendicular (normal) to the line, and $c$ determines the line's distance from the origin.

The line itself is all the points $(x,y)$ that satisfy the equation $ax+by=c$.
	The line equation imposes a **linear constraint** on the coordinates $(x,y)$ of points. 
		In vector terms, this constraint defines a **subspace** of the 2D space — specifically, a 1-dimensional line.
### Origin in Vector Spaces
The standard form of the line equation can be understood as derived from the **[[Data/Abstract Mathematical Spaces/Linear Algebra/Linearity/Dot Product|dot product]]** of vectors. 
	This implies that the line equation is rooted in the geometry of vector spaces:
	    The line equation can be seen as expressing the fact that all points on the line have a **constant projection** onto the normal vector $[a,b]$.
		    This highlights that the line equation is inherently about the relationship between vectors and their directions, i.e., the constraints imposed on a vector's coordinates to lie on a line.

The line equation imposes a **linear constraint** on the coordinates of points.
	In vector terms, this constraint defines a **subspace** of the 2D space — specifically, a 1-dimensional line.

The coefficients $a$ and $b$ act as **weights** that combine the standard basis vectors $\hat{i} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}$ and $\hat{j} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}$.
	This combination defines the line's normal vector $\vec{n}$, which is central to understanding the line's orientation.
### Geometric Implications of the Components
###### $\LARGE a$ and $\LARGE b$
They define the direction orthogonal (perpendicular) to the line. 
	The ratio $\LARGE \frac{a}{b}$​ gives the slope of the line when $b \neq 0$.
		 Geometrically, these coefficients indicate how the line changes as you move along the $x$ or $y$ directions.
###### $\LARGE c$
This shifts the line in the direction of the normal vector.
	If you change $c$ while keeping $a$ and $b$ constant, you’re moving the line along the direction perpendicular to its orientation.
### Line as a Set of Vectors
Consider **every point** $(x,y)$ on the line as being represented by a **[[#Position Vectors, $ vec{r}$, are Cartesian Vectors|position vector]]**:
$$\LARGE \vec{r} = x \hat{i} + y \hat{j}$$
The line equation $ax+by=c$ tells us that for all position vectors $\vec{r}$ on the line, the dot product with the normal vector $\vec{n} = a \hat{i} + b \hat{j}$ is constant:
$$\LARGE \vec{n} \cdot \vec{r} = c$$
- This means that the projection of any point $\vec{r}$ onto the normal vector $\vec{n}$ is fixed, implying that all such points lie on a line orthogonal to $\vec{n}$.
### Linking to Linear Transformations
You can think of the line equation as the result of a **linear transformation** applied to the vector
$$\LARGE \vec{r} = \begin{bmatrix} x \\ y \end{bmatrix}$$
$$\LARGE T(\vec{r}) = \begin{bmatrix} a & b \end{bmatrix} \cdot \vec{r}$$
This transformation "projects" $\vec{r}$ onto the direction of $\vec{n}$.
	The line itself is the set of all vectors $\vec{r}$ that, under this transformation, yield the constant value $c$. 
		This perspective shows that the line equation is tied to the concept of **projection** in vector spaces.
### A Linear Map from Vectors to Scalars (i.e. A Scalar Function)
The dot product with a fixed vector $[ab]$ can be interpreted as a linear map from vectors in $\mathbb{R}^2$ to scalars in $\mathbb{R}$:
$$\LARGE T(\vec{r}) = \begin{bmatrix} a & b \end{bmatrix} \cdot \vec{r}$$
Where $\vec{v} = [x \, y]$.
	This operation maps the vector $\vec{v}$ to a scalar, and it is **linear** because it satisfies the properties of linearity (additivity and scalar multiplication).

If you think of this dot product as a **linear map**, it can be interpreted as **extracting a certain "projection" or "component"** of the vector $[xy]$ in the direction of the fixed vector $[a \, b]$.
	In this sense, the dot product acts like a **transformation** that compresses the information of the vector $[xy]$ into a single scalar, $c$.
### Dot Product Representation:
expressing the standard form of a line ax+by=cax + by = cax+by=c as a dot product is indeed a formal and valid way to represent the line in linear algebra. Here's how this works and why it's a formal representation:
- The standard form of a line in 2D is given by:
    
    ax+by=c,ax + by = c,ax+by=c,
    
    where aaa and bbb are constants that define the slope and orientation of the line, and 
    
- This can be rewritten using the **dot product** of two vectors:
    
    [ab]⋅[xy]=c,\begin{bmatrix} a & b \end{bmatrix} \cdot \begin{bmatrix} x \\ y \end{bmatrix} = c,[a​b​]⋅[xy​]=c,
    
    where [ab]\begin{bmatrix} a & b \end{bmatrix}[a​b​] is a vector normal to the line, and [xy]\begin{bmatrix} x \\ y \end{bmatrix}[xy​] is a point on the line.
    

### 2. **Why This Is a Formal Representation:**

- **Dot Product:** The dot product of two vectors n⃗=[ab]\vec{n} = \begin{bmatrix} a & b \end{bmatrix}n=[a​b​] and v⃗=[xy]\vec{v} = \begin{bmatrix} x & y \end{bmatrix}v=[x​y​] is defined as:
    
    n⃗⋅v⃗=a⋅x+b⋅y.\vec{n} \cdot \vec{v} = a \cdot x + b \cdot y.n⋅v=a⋅x+b⋅y.
    
    This operation results in a scalar quantity. In this case, the dot product equals the constant ccc, which represents a specific geometric condition that the point (x,y)(x, y)(x,y) must satisfy to lie on the line.
    
- **Normal Vector:** The vector [ab]\begin{bmatrix} a & b \end{bmatrix}[a​b​] is **normal** (perpendicular) to the line. This means it defines the orientation of the line. The equation n⃗⋅v⃗=c\vec{n} \cdot \vec{v} = cn⋅v=c indicates that for any point (x,y)(x, y)(x,y) on the line, the projection of the point onto the normal vector remains constant, which geometrically defines a line.
    
- **Geometric Constraint:** The expression n⃗⋅v⃗=c\vec{n} \cdot \vec{v} = cn⋅v=c is a **linear constraint** in the plane. In linear algebra, this is formally understood as the set of points (x,y)(x, y)(x,y) that satisfy this constraint, which forms a line.
    

### 3. **Advantages of the Dot Product Representation:**

- **Compactness:** Using the dot product provides a compact and vector-based way to express the line equation.
- **Extension to Higher Dimensions:** This method of using a normal vector to define a linear constraint can be extended to higher dimensions. For example, in 3D, the equation ax+by+cz=dax + by + cz = dax+by+cz=d can be written as the dot product n⃗⋅v⃗=d\vec{n} \cdot \vec{v} = dn⋅v=d, where n⃗=[a,b,c]\vec{n} = [a, b, c]n=[a,b,c] is a normal vector to the plane.
- **Relation to Linear Algebra:** This representation connects directly to linear algebra concepts such as vector projection, orthogonality, and linear constraints.

### 4. **Formal Interpretation:**

- In the dot product form, [ab]⋅[xy]=c\begin{bmatrix} a & b \end{bmatrix} \cdot \begin{bmatrix} x \\ y \end{bmatrix} = c[a​b​]⋅[xy​]=c, we are specifying that the vector [xy]\begin{bmatrix} x & y \end{bmatrix}[x​y​] lies on a line whose normal vector is [ab]\begin{bmatrix} a & b \end{bmatrix}[a​b​]. The constant ccc controls the line's offset from the origin.
- In linear algebra, this is a **hyperplane equation** in 2D space (a line), which formally divides the space into regions based on the sign of the dot product.

### **Conclusion:**

Yes, expressing the standard form of a line ax+by=cax + by = cax+by=c as a dot product [ab]⋅[xy]=c\begin{bmatrix} a & b \end{bmatrix} \cdot \begin{bmatrix} x \\ y \end{bmatrix} = c[a​b​]⋅[xy​]=c is a formal and mathematically rigorous way to represent the line in linear algebra. It leverages the concept of the dot product to succinctly describe the geometric relationship that defines all points on the line.

## Relation to Linear Transformations
The relationship between the line's dot product form and a linear transformation of a position vector comes down to how linear transformations affect vectors in space and how the conditions of the line's equation are preserved or modified under such transformations. Let’s break this down in the context of linear algebra.

### 1. **Recap: Line Representation and Linear Transformations**

- **Line Equation as Dot Product:** The line equation in 2D can be written using the dot product:
    
    [ab]⋅[xy]=c,\begin{bmatrix} a & b \end{bmatrix} \cdot \begin{bmatrix} x \\ y \end{bmatrix} = c,[a​b​]⋅[xy​]=c,
    
    where [ab]\begin{bmatrix} a & b \end{bmatrix}[a​b​] is the normal vector to the line and [xy]\begin{bmatrix} x \\ y \end{bmatrix}[xy​] is a position vector representing a point on the line.
    
- **Linear Transformation:** A linear transformation T:R2→R2T: \mathbb{R}^2 \to \mathbb{R}^2T:R2→R2 can be represented by a matrix AAA. For a position vector v⃗=[xy]\vec{v} = \begin{bmatrix} x \\ y \end{bmatrix}v=[xy​], the transformed vector v⃗′\vec{v}'v′ is given by:
    
    T(v⃗)=Av⃗.T(\vec{v}) = A \vec{v}.T(v)=Av.
    
    This transformation changes the coordinates of v⃗\vec{v}v, which geometrically corresponds to scaling, rotating, shearing, or otherwise transforming the space in which the vector resides.
    

### 2. **How Linear Transformations Affect the Line Equation**

When we apply a linear transformation TTT (represented by the matrix AAA) to a vector v⃗=[xy]\vec{v} = \begin{bmatrix} x \\ y \end{bmatrix}v=[xy​], we get a new vector:

v⃗′=Av⃗=[x′y′].\vec{v}' = A \vec{v} = \begin{bmatrix} x' \\ y' \end{bmatrix}.v′=Av=[x′y′​].

The line equation ax+by=cax + by = cax+by=c describes a set of vectors v⃗\vec{v}v that lie on a specific line. When we apply the transformation TTT to all the vectors in this line, the shape, orientation, and position of the line can change.

### 3. **Transforming the Normal Vector of the Line**

- The line ax+by=cax + by = cax+by=c has a normal vector n⃗=[ab]\vec{n} = \begin{bmatrix} a \\ b \end{bmatrix}n=[ab​]. The line equation can be rewritten as a dot product: n⃗⋅v⃗=c.\vec{n} \cdot \vec{v} = c.n⋅v=c.
- When a linear transformation TTT is applied, both the vector v⃗\vec{v}v and the normal vector n⃗\vec{n}n are affected. However, to maintain a similar line equation in the transformed space, we also need to transform the normal vector. The new line equation in the transformed space is generally of the form: n⃗′⋅v⃗′=c′,\vec{n}' \cdot \vec{v}' = c',n′⋅v′=c′, where n⃗′=A−Tn⃗\vec{n}' = A^{-T} \vec{n}n′=A−Tn (the inverse transpose of AAA applied to n⃗\vec{n}n) and v⃗′=Av⃗\vec{v}' = A \vec{v}v′=Av. This result comes from how linear transformations affect dot products and normals in linear algebra.

### 4. **Relation Between Line Equation and Linear Transformation**

The relationship can be summarized as follows:

- **Original Line:** The line ax+by=cax + by = cax+by=c constrains vectors v⃗\vec{v}v in the 2D space.
- **Applying a Linear Transformation:** If you apply a linear transformation TTT (represented by AAA) to every vector v⃗\vec{v}v on the line, the image of the line under this transformation is generally another line. However, the normal vector of this new line and the equation defining it will change according to the transformation.
- **New Line Equation:** The new line equation in the transformed space involves the transformed normal vector n⃗′=A−Tn⃗\vec{n}' = A^{-T} \vec{n}n′=A−Tn. This means the linear transformation affects both the points on the line and the orientation of the line itself.

### 5. **Geometric Interpretation**

- **Linear Transformation as Mapping:** The linear transformation AAA maps the original line to a new line in the transformed space. The form of the line changes because the transformation modifies the coordinates of every point.
- **Preserving Linear Structure:** Despite the changes, a linear transformation will map lines to lines (or points, if the line collapses). This means that linear transformations preserve the "linear" nature of geometric objects such as lines and planes, though they can change their orientation, position, and scale.

### **Summary**

- The **dot product representation** of a line n⃗⋅v⃗=c\vec{n} \cdot \vec{v} = cn⋅v=c is formal and serves as a way to describe a linear relationship between vectors.
- A **linear transformation** T(v⃗)=Av⃗T(\vec{v}) = A \vec{v}T(v)=Av changes the coordinates of a vector, thus transforming the line defined by the dot product equation.
- Under a linear transformation, the line's normal vector n⃗\vec{n}n transforms to a new normal vector n⃗′=A−Tn⃗\vec{n}' = A^{-T} \vec{n}n′=A−Tn. The transformed position vectors v⃗′=Av⃗\vec{v}' = A \vec{v}v′=Av define a new line in the transformed space.

In conclusion, the line equation ax+by=cax + by = cax+by=c expressed as a dot product is related to linear transformations in that linear transformations change both the normal vector and the position vectors of the line, resulting in a new line in the transformed space. This shows the interplay between geometric constraints (like lines) and linear transformations in vector spaces.