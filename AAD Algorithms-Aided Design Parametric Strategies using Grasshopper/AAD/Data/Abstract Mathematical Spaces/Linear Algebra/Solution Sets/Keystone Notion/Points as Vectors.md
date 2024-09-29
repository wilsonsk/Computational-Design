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
The output is a three new vectors formed by this linear combination of the basis vectors.
###### The $\textcolor{green}{\text{Mapping}}$ of the Linear Transformation, $\LARGE \textcolor{green}{T : (\vec{e_1}, \vec{e_2}, \vec{e_3}) \to T_A(\vec{e_1}, T_A\vec{e_2}, T_A\vec{e_3})}$
The linear transformation $T$ takes the three input basis vectors $(\vec{e_1},\vec{e_2},\vec{e_3})$ and construct three new vectors as linear combinations of the standard basis vectors.
	The components of the Transformation are Linear Combinations.
###### The $\textcolor{teal}{\text{Mapping Operator}}$, $\LARGE T_A$
The matrix $A$ **encodes the rules** of the transformation. 
	It dictates how every input vector $\vec{v}$ is changed when the linear transformation $TA$​ is applied.
		 The entries of the matrix determine the nature of the transformation, such as scaling, rotating, reflecting, shearing, or mixing the components of the input vector.
### Each $\LARGE T_A(\vec{e_1}), T_A(\vec{e_2}), T_A(\vec{e_3})$ is Itself a Linear Transformation (of a Basis Vector)
$$\LARGE T: \textcolor{violet}{\mathbb{R}^n} \to \textcolor{yellow}{\mathbb{R}^m}, \quad \textcolor{teal}{T} : \textcolor{violet}{(\vec{e_1}, \vec{e_2}, \vec{e_3})} \to \textcolor{yellow}{T_A(\vec{e_1}) + T_A(\vec{e_2}) + T_A(\vec{e_3})}$$
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
###### Remember A Vector is a Linear Combination of Basis Vectors (i.e. Scaled Standard Unit Vectors)
$$\LARGE \vec{v} = (x,y,z)$$
$$\LARGE \vec{v} = \mathbf{v} = T_A(x,y,z) = (x)\vec{e_1} + (y) \vec{e_2} + (z) \vec{e_3}$$
###### Remember that the Image of the Transformation is then Determined by the Transformation of the Basis Vectors, $(\vec{e_1}, \vec{e_2}, \vec{e_3})$.
$$\large \textcolor{green}{T(}\textcolor{violet}{\vec{v}}\textcolor{green}{)} = \textcolor{green}{T_A(}\textcolor{red}{x}(\vec{e_1}) + \textcolor{red}{y}(\vec{e_2}) + \textcolor{red}{z}(\vec{e_3}) \textcolor{green}{)} = \textcolor{red}{x}\textcolor{green}{T_A(\vec{e_1})} + \textcolor{red}{y}\textcolor{green}{T_A(\vec{e_2})} + \textcolor{red}{z}\textcolor{green}{T_A(\vec{e_3})} = \textcolor{yellow}{x \hat{i} + y \hat{j} + z \hat{k}}$$
Where $\LARGE \hat{i}, \hat{j}, \hat{k}$ have been transformed by $T_A$.
	After the image is produced, the vector containing the components $x,y,z$ (as scalars) is Linearly Transformed by the output image of the transformed basis vectors, $T_A$. 
		I.e. The Linear Transformation of a vector (some non-basis vector) is the Linear Combination of the transformed basis vectors with the components of the vector now being transformed.
###### The $\textcolor{violet}{\text{Input}}$ to the Linear Transformation, $\LARGE \vec{v}$
**The Input** to the transformation $T$ is a **vector** $\vec{v} = (x, y, z)$ in $\mathbb{R}^3$.
	This vector can be thought of as having three components, which are the coordinates $x,y,z$ with respect to the standard basis vectors $\hat{i}, \hat{j}, \hat{k}$.
		I.e. This input vector has a shorthand represented by the a corresponding "point" $(x,y,z)$ that is associated with that input Position Vector.
###### The $\textcolor{yellow}{\text{Output}}$ (i.e. Image) of the Linear Transformation, $\LARGE T_A(\vec{v})$
The result is a new vector formed by this linear combination of the basis vectors.
	This new vector is either within the same space or a different space, depending on defined codomain. 
###### The $\textcolor{green}{\text{Mapping of the Linear Transformation}}$, $\LARGE T : (\vec{v}) \to T_A(\vec{v})$
The linear transformation $T$ takes the input coordinates $(x, y, z)$ and constructs a vector as a linear combination of the standard basis vectors.
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
### The Image Matrix $T_A(\vec{e_i})$ (of Transformed Basis Vectors) is a New Matrix $A$
Which is what transforms the Vectors in this Space.
##### Matrix, $A$ of $T_A$
The matrix $A$ **encodes the rules** of the transformation. 
	It dictates how every input vector $\LARGE \vec{v}$ is changed when the linear transformation $T_A$$​ is applied.
		 The entries of the matrix determine the nature of the transformation, such as scaling, rotating, reflecting, shearing, or mixing the components of the input vector.
###### Linear Combination of Basis Vectors
When $T_A$​ acts on a general vector $\vec{v} = \begin{bmatrix} v_1 \\ v_2 \\ v_3 \end{bmatrix}$, the output vector is:
$$\LARGE T_A(\vec{v}) = A \vec{v} = v_1 \begin{bmatrix} a_{11} \\ a_{21} \\ a_{31} \end{bmatrix} + v_2 \begin{bmatrix} a_{12} \\ a_{22} \\ a_{32} \end{bmatrix} + v_3 \begin{bmatrix} a_{13} \\ a_{23} \\ a_{33} \end{bmatrix}$$

This shows that the transformation scales and combines the columns of $A$ according to the components $\LARGE v_1, v_2, v_3$​ of the input vector.
###### Matrix $A$ as a Set of Instructions
The matrix $A$ tells you **how** to construct the output vector $T_A(\vec{v})$ from the input vector $\vec{v}$.
	When you multiply $A$ by $\vec{v}$, you are effectively taking a weighted sum of the columns of $A$ using the components of $\vec{v}$ as weights:
 $$\LARGE T_A(\vec{v}) = A \vec{v} = v_1 \begin{bmatrix} a_{11} \\ a_{21} \\ \dots \\ a_{m1} \end{bmatrix} + v_2 \begin{bmatrix} a_{12} \\ a_{22} \\ \dots \\ a_{m2} \end{bmatrix} + \dots + v_n \begin{bmatrix} a_{1n} \\ a_{2n} \\ \dots \\ a_{mn} \end{bmatrix}$$
This shows how each coordinate of $\vec{v}$ contributes to the resulting output vector according to the columns of $A$.
###### Geometric Interpretation
If $A$ is a **diagonal matrix** like $\LARGE \begin{bmatrix} a & 0 & 0 \\ 0 & b & 0 \\ 0 & 0 & c \end{bmatrix}​$, it represents **scaling** along each of the axes by the factors $a,b$, and $c$.
If $A$ contains off-diagonal terms, it can represent more complex
##### The Image of a Linear Transformation of a Basis Vector ***is*** a Matrix, $T_A$
The matrix $A$ containing $(x, y, z)$ defines a **linear transformation** because the resulting vector $T_A(\vec{v})$is a linear combination of the coordinates $x,y,z$ and the input vector's components.
	This setup aligns with the idea of a **vector-valued function**, where the output is a vector, and the function maps input vectors to other vectors through linear combinations involving $x,y,z$.

The matrix $A$ dictates **how** the input coordinates are transformed. 
	The form of the matrix $A$ does, in a way, represent the "structure" or "form" of the output vector.
		The matrix $A$ determines the linear combination of basis vectors that defines the output vector in the space.

Suppose $\LARGE A$ is an $\LARGE m \times n$ matrix:
$$\LARGE A = \begin{bmatrix} a_{11} & a_{12} & \dots & a_{1n} \\ a_{21} & a_{22} & \dots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \dots & a_{mn} \end{bmatrix}$$

When this matrix acts on the vector $\LARGE\vec{v} = \begin{bmatrix} v_1 \\ v_2 \\ \dots \\ v_n \end{bmatrix}$,the result is:
$$\LARGE T_A(\vec{v}) = A \vec{v} = \begin{bmatrix} a_{11}v_1 + a_{12}v_2 + \dots + a_{1n}v_n \\ a_{21}v_1 + a_{22}v_2 + \dots + a_{2n}v_n \\ \vdots \\ a_{m1}v_1 + a_{m2}v_2 + \dots + a_{mn}v_n \end{bmatrix}$$
### Components of the Whole $T_A(\vec{v})$
$$\LARGE T : (\vec{v}) \to T_A(\vec{v})$$
Each $\LARGE T_i(\vec{v})$ (i.e. each "row" of $T_A(\vec{v})$) is a **scalar component function** defined by the linear combination of the input vector $\vec{v}$, scaled by the elements of the matrix $A$.:
$$\LARGE T_i(\vec{v}) = a_{i1}v_1 \cdot \vec{e_1} + a_{i2}v_2 \cdot \vec{e_2}+ \dots + a_{in}v_n \cdot \vec{e_n}$$
$$\LARGE T_A(\vec{v}) = A \vec{v} = \begin{bmatrix} a_{11}v_1 + a_{12}v_2 + \dots + a_{1n}v_n \\ a_{21}v_1 + a_{22}v_2 + \dots + a_{2n}v_n \\ \vdots \\ a_{m1}v_1 + a_{m2}v_2 + \dots + a_{mn}v_n \end{bmatrix}$$
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
### The Component Scalar Functions of the Linear Transformation Applied to a Vector

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


