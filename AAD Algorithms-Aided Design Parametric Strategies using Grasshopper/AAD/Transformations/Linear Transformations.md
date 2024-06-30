# Linear Transformations
A linear transformation can be thought of as a kind of [[Linear Motion|linear "motion"]] but it's more general and abstract than physical motion.
	This means they maintain the operations of vector addition and scalar multiplication, crucial for many theoretical and practical applications in mathematics, physics, computer science, and engineering.
		They are not restricted to just "motion" in the physical sense but encompass any operation that adheres to the principles of linearity.

Linear transformations encompass a wide range of operations that include, but are not limited to, motions like translations, rotations, and scaling.

### Linear Transformations and Linear Motion

1. **Translation**: Typically, translation is not considered a linear transformation because it doesn’t preserve the origin. However, in an extended framework called affine transformations, translations are included.
    
2. **Rotation**: Rotating a vector about the origin in two or three dimensions is a linear transformation. The rotation transformation preserves the lengths of vectors and angles between them.
    
3. **Scaling**: Scaling stretches or shrinks vectors by a constant factor and is a straightforward example of a linear transformation. It changes the magnitude of vectors but preserves their direction.
    
4. **Reflection**: Reflecting vectors across a line or plane is also a linear transformation. It changes the direction of vectors but keeps their magnitudes.
    
5. **Shearing**: Shearing is a transformation that shifts each point in a fixed direction, which can be visualized as slanting an object. It is linear because it maps lines to lines and preserves parallelism.
    

### Key Properties of Linear Transformations

- **Preservation of the Origin**: Linear transformations map the zero vector in the input space to the zero vector in the output space.
- **Linearity**: They preserve vector addition and scalar multiplication: T(u+v)=T(u)+T(v)T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})T(u+v)=T(u)+T(v) T(cu)=cT(u)T(c \mathbf{u}) = c T(\mathbf{u})T(cu)=cT(u)

### Differences From [[Euclidean Transformations|Euclidean Transformations]]

1. **Distance Preservation**:
    
    - **Euclidean Transformations**: Preserve distances (are isometries).
    - **Linear Transformations**: Do not necessarily preserve distances. For example, scaling changes the distances between points.
2. **Inclusion of Translations**:
    
    - **Euclidean Transformations**: Include translations.
    - **Linear Transformations**: Do not include translations because they do not preserve the origin.

### Linear Transformations in Linear Algebra
Linear transformations in linear algebra are functions between two vector spaces that map vectors to vectors in a way that preserves vector addition and scalar multiplication.
	They can be represented by matrices, making them fundamental tools for operations in vector spaces. 
		While Euclidean transformations are specific to preserving distances and angles, linear transformations include a broader range of operations, such as scaling and shearing, which do not necessarily preserve distances but do maintain linearity.

 if VVV and WWW are vector spaces over the same field FFF, a function T:V→WT: V \rightarrow WT:V→W is a linear transformation if for all vectors u,v∈V\mathbf{u}, \mathbf{v} \in Vu,v∈V and all scalars c∈Fc \in Fc∈F, the following two conditions hold:

1. **Additivity**: T(u+v)=T(u)+T(v)T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})T(u+v)=T(u)+T(v)
2. **Homogeneity (Scalar Multiplication)**: T(cu)=cT(u)T(c \mathbf{u}) = c T(\mathbf{u})T(cu)=cT(u)
### Key Properties of Linear Transformations

- **Preservation of the Origin**: Linear transformations map the zero vector in the input space to the zero vector in the output space.
- **Linearity**: They preserve linear combinations of vectors.