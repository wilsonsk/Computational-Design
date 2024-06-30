# Linear Map
## A Linear Map (i.e. a [[Linear Transformations|Linear Transformation]])
Is a [[Functions|function]] between two vector spaces that preserves the operations of vector addition and scalar multiplication.

If $V$ and $W$ are vector spaces over the same field $F$, a function 
$$T: V \rightarrow W$$ Is called a linear map if for all vectors $$\mathbf{u}, \mathbf{v} \in V$$ And all scalars $c \in F$, the following two conditions hold:

- **Additivity**: $$\LARGE T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})$$
- **Homogeneity (Scalar Multiplication)**: $$\LARGE T(c \mathbf{u}) = c T(\mathbf{u})$$
### Vector Space
A **vector space** (also known as a linear space) is a fundamental structure in linear algebra and many other areas of mathematics. 
	It consists of a set of vectors, along with two operations: vector addition and scalar multiplication.
	
 A vector space is a set of elements, called vectors, that can be added together and multiplied by scalars, satisfying certain properties.
	
A vector space $V$ over a field $F$ (commonly the field of real numbers $\mathbb{R}$ or complex numbers $\mathbb{C}$) is a set equipped with two operations:
- **Vector Addition**: An operation that takes any two vectors $\mathbf{u}$ and $\mathbf{v}$ in $V$ and produces another vector $\mathbf{w} \in V$.
- **Scalar Multiplication**: An operation that takes a scalar $c \in F$ and a vector $\mathbf{u} \in V$ and produces another vector $\mathbf{v} \in V$.
##### I.e. Linear Space
The term "linear space" emphasizes these fundamental properties of linearity.
- **Linearity**: Reflects the property that the space is closed under linear combinations of vectors. For any vectors u,v\mathbf{u}, \mathbf{v}u,v and scalars a,ba, ba,b, the combination au+bva \mathbf{u} + b \mathbf{v}au+bv remains within the space.
- **Space**: Indicates that we are dealing with a set of vectors that form a mathematical structure adhering to these rules.

- - -
### Vector Addition
**Vector addition** is the operation of adding two vectors together to form a new vector. 
	This operation is defined component-wise.
#### Definition
Given two vectors $\mathbf{u}$ and $\mathbf{v}$ in a vector space $V$, where:
$$\LARGE \mathbf{u} = \begin{pmatrix} u_1 \\ u_2 \\ \vdots \\ u_n \end{pmatrix}$$
$$\LARGE \mathbf{v} = \begin{pmatrix} v_1 \\ v_2 \\ \vdots \\ v_n \end{pmatrix}$$
$$\LARGE \text{The sum } \mathbf{w} = \mathbf{u} + \mathbf{v} \text{ is given by: } \mathbf{w} = \begin{pmatrix} u_1 + v_1 \\ u_2 + v_2 \\ \vdots \\ u_n + v_n \end{pmatrix}.$$
#### Properties
- **Commutativity**: u+v=v+u\mathbf{u} + \mathbf{v} = \mathbf{v} + \mathbf{u}u+v=v+u
- **Associativity**: u+(v+w)=(u+v)+w\mathbf{u} + (\mathbf{v} + \mathbf{w}) = (\mathbf{u} + \mathbf{v}) + \mathbf{w}u+(v+w)=(u+v)+w
- **Identity Element**: There exists a zero vector 0\mathbf{0}0 such that u+0=u\mathbf{u} + \mathbf{0} = \mathbf{u}u+0=u
- **Inverse Element**: For each u\mathbf{u}u, there exists a vector −u-\mathbf{u}−u such that u+(−u)=0\mathbf{u} + (-\mathbf{u}) = \mathbf{0}u+(−u)=0


- - - 
### Scalar Multiplication
**Scalar multiplication** is the operation of multiplying a vector by a scalar (a number from the field over which the vector space is defined), which scales the vector.
#### Definition
Given a vector $u$ in a vector space $V$ and a scalar $c$ from a field $F$, the product $\mathbf{u}c$ is a new vector $\vec{v}$ defined by multiplying each component of $\mathbf{u}$ by $c$:
$$\LARGE \mathbf{u} = \begin{pmatrix} u_1 \\ u_2 \\ \vdots \\ u_n \end{pmatrix}$$

$$\LARGE c\mathbf{u} = \begin{pmatrix} cu_1 \\ cu_2 \\ \vdots \\ cu_n \end{pmatrix}$$
#### Properties
- **Distributivity Over Vector Addition**: c(u+v)=cu+cvc(\mathbf{u} + \mathbf{v}) = c \mathbf{u} + c \mathbf{v}c(u+v)=cu+cv
- **Distributivity Over Scalar Addition**: (a+b)u=au+bu(a + b) \mathbf{u} = a \mathbf{u} + b \mathbf{u}(a+b)u=au+bu
- **Associativity**: a(bu)=(ab)ua(b \mathbf{u}) = (ab) \mathbf{u}a(bu)=(ab)u
- **Identity Element**: 1u=u1 \mathbf{u} = \mathbf{u}1u=u

- - - 
### Linearity in Vector Spaces
The term "linear" refers to properties and operations that preserve straight-line relationships and [[Proportion|proportionality]]. 
	In a vector space (or linear space), the operations of vector addition and scalar multiplication adhere to linearity principles. 
		- **Vector Addition**: The addition of two vectors is linear because it follows the rule of adding corresponding components. 
			- This operation preserves the "straight-line" nature of combining vectors.
		- **Scalar Multiplication**: Multiplying a vector by a scalar scales the vector linearly. 
			- This means that if you multiply a vector by a scalar, the direction remains the same (if the scalar is positive) or reverses (if the scalar is negative), and the length of the vector is scaled by the absolute value of the scalar.

- - - 

## What are the Purposes of Linear Maps
### Simplifying Complex Geometries
##### Local Linearization:
###### Tangential Spaces
Differential geometry often involves studying curves and surfaces by looking at their tangent spaces.
	Tangent spaces provide a linear approximation of the geometry at a point, making complex nonlinear shapes easier to analyze and work with locally.
###### Simplified Calculations
By transforming complex surfaces into their tangent planes at specific points, architects can perform simplified calculations for structural analysis and design.
### Understanding Curvature and Shape
#### Curvature Analysis
###### [[Gaussian Curvature|Gaussian Curvature]]
Transformations can help compute and visualize curvature properties of surfaces, such as Gaussian curvature, which is crucial for understanding the local shape of the surface.
###### [[Mean Curvature|Mean Curvature]]
Similarly, transformations allow the calculation of mean curvature, important for assessing the surface smoothness and behavior under physical forces.
### [[Form-Finding Strategies Using Kangaroo|Structural Optimization]]
#### Form-Finding
###### [[Digital Form-Finding#Minimal Surfaces|Minimal Surfaces]]
Transformations to find minimal surfaces (surfaces that locally minimize area) are essential in architectural design for creating efficient and aesthetically pleasing structures.
###### Optimization Algorithms
Transformations facilitate the application of optimization algorithms that help in designing structures that are both strong and material-efficient.
### Parametric Design and Surface Manipulation
#### Parametric Modeling
###### [[Surfaces|Surface Representations]]
Transformations between different parameter spaces (e.g., from Cartesian to polar coordinates) enable more flexible and intuitive surface representations and manipulations.
###### Control Points and [[Nurbs Curves|NURBS]]
Using transformations, architects can control complex shapes via simpler underlying geometries, such as Non-Uniform Rational B-Splines (NURBS), enhancing the precision and flexibility of the design process.
### Visualization and Simulation
#### Simulation of Physical Properties
###### Stress and Strain Analysis
Transformations help simulate physical properties, such as stress and strain on architectural surfaces, providing critical insights into how materials will behave under various loads.
###### Thermal and Environmental Analysis
Understanding how surfaces interact with environmental factors (e.g., heat distribution, airflow) can be simplified through appropriate transformations, aiding in sustainable design.