# Fields
Despite the differences in specific definitions, the term "field" in all these contexts shares some common features:
#### Distribution Over a Space
Fields describe values or properties distributed over a space (be it physical space, a set of points, or an abstract space).
	In a mathematical field, the elements are distributed over the set with the operations defined on them.
		In scalar and vector fields, the values (scalars or vectors) are associated with points in a physical or abstract space.
#### Functional Association
A field involves an association or mapping between elements.
	In mathematics, this involves operations on elements within the field.
		In physics and biology, fields map physical quantities (scalars, vectors, or developmental potentials) to points in space.
#### Concept of Influence or Interaction
Fields often represent how values or quantities influence each other across a space.
	In a mathematical field, elements interact through operations.
		In scalar and vector fields, quantities like temperature, pressure, or force influence each point in the space.
			In morphogenetic fields, the potential for development is influenced by the spatial distribution of cells.

- - -
## [[Abstract Mathematical Spaces#Fields|Fields]] (of Field Theory, Algebra) vs. Fields (as Functions)

### Fields (of Field Theory)
A [[Abstract Mathematical Spaces#Structured Set (i.e. Space)|Structured Set]] with addition and multiplication satisfying certain properties.

In algebra, a **field** is a set equipped with two operations, usually called addition and multiplication, that satisfy certain axioms.
	These are abstract algebraic structures that provide a framework for many areas of mathematics, including number theory, algebraic geometry, and cryptography.
		This definition comes from field theory, a branch of abstract algebra.
#### Axioms of a Field
A field $F$ is a set with two operations (addition and multiplication) that satisfy the following axioms:
1. **Closure**: For all $\LARGE a, b \in F$, both $\LARGE a+b \text{ and } \cdot b$ are in $\LARGE F$.
2. **Associativity**: Both addition and multiplication are associative.
3. **Commutativity**: Both addition and multiplication are commutative.
4. **Identity Elements**: There exist elements $\LARGE 0 \in F$ and $\LARGE 1 \in F$ such that for all $\LARGE a \in F$, $\LARGE a + 0 = a$ and $\LARGE a \cdot 1 = a$.
5. **Additive Inverses**: For every $\LARGE a \in F$, there exists an element $\LARGE -a \in F$ such that $\LARGE a + (-a) = 0$.
6. **Multiplicative Inverses**: For every $\LARGE a \in F$ (except $0$), there exists an element $a^{-1} \in F$ such that $\LARGE a \cdot a^{-1} = 1$.
7. **Distributivity**: Multiplication

- - -
### Fields as [[Mapping|Mappings]] in Analysis and Physics
In the context of analysis, physics, and geometry, a **field** refers to a [[Mapping|function]] that assigns values (scalars, vectors, etc.) to points in a space. 
	- These are functions that provide a way to describe how quantities vary over space and time in physical contexts.
		- They are foundational in fields like fluid dynamics, electromagnetism, and general relativity.
			This is quite different from the algebraic definition.
##### Scalar Field
A scalar field is a function that assigns a scalar value to every point in a space.
**Example**: Temperature distribution in a room, where each point $(x, y, z)$ has a temperature value $T(x, y, z)$.
###### Mathematical Representation
**Scalar Field**: $\LARGE f: \mathbb{R}^n \to \mathbb{R}$
##### Vector Field
A vector field is a function that assigns a vector to every point in a space.
**Example**: Wind velocity in the atmosphere, where each point $(x, y, z)$ has a velocity vector $\mathbf{v}(x, y, z)$.
###### Mathematical Representation
**Vector Field**: $\LARGE \mathbf{F}: \mathbb{R}^n$
The term "field" (denoted as $F$) refers to a set along with two operations, addition and multiplication, that satisfy the field axioms. 
	A field is a mathematical structure used in linear algebra to define scalar values for vector spaces.
