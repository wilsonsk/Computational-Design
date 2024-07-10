# Fields
## [[Abstract Mathematical Spaces#Fields|Fields]] (of Field Theory, Algebra) vs. Fields (as Functions)
### Fields (of Field Theory)
A [[Abstract Mathematical Spaces#Structured Set (i.e. Space)|Structured Set]] with addition and multiplication satisfying certain properties.

In algebra, a **field** is a set equipped with two operations, usually called addition and multiplication, that satisfy certain axioms.
	These are abstract algebraic structures that provide a framework for many areas of mathematics, including number theory, algebraic geometry, and cryptography.
		This definition comes from field theory, a branch of abstract algebra.
##### Definition
A field $F$ is a set with two operations (addition and multiplication) such that:
1. **Closure**: For all $\LARGE a, b \in F$, both $\LARGE a+b \text{ and } \cdot b$ are in $\LARGE F$.
2. **Associativity**: Both addition and multiplication are associative.
3. **Commutativity**: Both addition and multiplication are commutative.
4. **Identity Elements**: There exist elements $\LARGE 0 \in F$ and $\LARGE 1 \in F$ such that for all $\LARGE a \in F$, $\LARGE a + 0 = a$ and $\LARGE a \cdot 1 = a$.
5. **Additive Inverses**: For every $\LARGE a \in F$, there exists an element $\LARGE -a \in F$ such that $\LARGE a + (-a) = 0$.
6. **Multiplicative Inverses**: For every $\LARGE a \in F$ (except $0$), there exists an element $a^{-1} \in F$ such that $\LARGE a \cdot a^{-1} = 1$.
7. **Distributivity**: Multiplication is distributive over addition, i.e., $\LARGE a \cdot (b + c) = a \cdot b + a \cdot c$ for all $\LARGE a, b, c \in F$.
#### Fields as Functions in Analysis and Physics
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
### Commonalities
Despite the differences in specific definitions, the term "field" in all these contexts shares some common features:
1. **Distribution Over a Space**:
    - Fields describe values or properties distributed over a space (be it physical space, a set of points, or an abstract space).
    - In a mathematical field, the elements are distributed over the set with the operations defined on them.
    - In scalar and vector fields, the values (scalars or vectors) are associated with points in a physical or abstract space.
2. **Functional Association**:
    - A field involves an association or mapping between elements.
    - In mathematics, this involves operations on elements within the field.
    - In physics and biology, fields map physical quantities (scalars, vectors, or developmental potentials) to points in space.
3. **Concept of Influence or Interaction**:
    - Fields often represent how values or quantities influence each other across a space.
    - In a mathematical field, elements interact through operations.
    - In scalar and vector fields, quantities like temperature, pressure, or force influence each point in the space.
    - In morphogenetic fields, the potential for development is influenced by the spatial distribution of cells.

### Formal Definitions

1. **Relation**:
    
    - A relation $R$ between two sets $A$ and $B$ is a subset of the Cartesian product $A \times B$.
    - Example: $R = {(a, b) \in A \times B \mid \text{some condition holds} }$.
2. **Function (Mapping)**:
    
    - A function $f$ from a set $A$ to a set $B$ is a relation such that every element of $A$ is related to exactly one element of $B$.
    - Notation: $f: A \rightarrow B$.
3. **Operation**:
    
    - An operation is a function that takes elements from one or more sets and maps them to another set.
    - Binary operation example: $+: \mathbb{R} \times \mathbb{R} \rightarrow \mathbb{R}$ where $+(a, b) = a + b$.

Relations often dictate the mapping between elements, and these mappings can indeed be represented by functions or operations. To clarify this further, let’s delve into the concepts of relations, mappings, functions, and operations:

### Relations

**Definition**:

- A relation between two sets is a collection of ordered pairs containing one element from each set.
- It describes how elements from one set are related to elements of another set (or the same set).

**Example**:

- The "less than" relation on the set of real numbers is a collection of pairs $(a, b)$ such that $a < b$.

### Mappings and Functions

**Definition**:

- A mapping (or function) is a special type of relation where each element of the first set (domain) is related to exactly one element of the second set (codomain).
- Functions are often described as rules that assign each element of a domain to a unique element in the codomain.

**Example**:

- The function $f(x) = x^2$ maps each real number $x$ to its square.

### Operations as Functions

**Operations as Special Functions**:

- Operations can be viewed as functions that map elements from their domain(s) to their codomain(s).
- For example, addition in arithmetic can be seen as a function that maps pairs of numbers to their sum: $f(a, b) = a + b$.

### How Relations Dictate Mappings and Operations

1. **Relations Dictating Mappings**:
    
    - A relation can define how elements of one set correspond to elements of another set.
    - For example, the relation "is the square of" defines a mapping between the set of real numbers and itself: $y = x^2$.
2. **Functions and Operations Representing Relations**:
    
    - Functions are specific kinds of relations where each input is related to one output.
    - Operations (like addition, multiplication) are functions that perform specific actions on inputs.
    - For example, the relation $y = f(x)$, where $f$ is a function, describes how each $x$ maps to $y$.

### Examples
## Field in Linear Algebra
In Linear Algebra, a field does **not** refer to a region of space.
A **field** $F$ is a set equipped with two operations, usually called addition and multiplication, satisfying the following properties:

1. **Associativity of Addition and Multiplication**:
    - (a+b)+c=a+(b+c)(a + b) + c = a + (b + c)(a+b)+c=a+(b+c)
    - (a⋅b)⋅c=a⋅(b⋅c)(a \cdot b) \cdot c = a \cdot (b \cdot c)(a⋅b)⋅c=a⋅(b⋅c)
2. **Commutativity of Addition and Multiplication**:
    - a+b=b+aa + b = b + aa+b=b+a
    - a⋅b=b⋅aa \cdot b = b \cdot aa⋅b=b⋅a
3. **Additive and Multiplicative Identity**:
    - There exists an element 0∈F0 \in F0∈F such that a+0=aa + 0 = aa+0=a for all a∈Fa \in Fa∈F.
    - There exists an element 1∈F1 \in F1∈F such that a⋅1=aa \cdot 1 = aa⋅1=a for all a∈Fa \in Fa∈F and 1≠01 \neq 01=0.
4. **Additive Inverses**:
    - For each a∈Fa \in Fa∈F, there exists an element −a∈F-a \in F−a∈F such that a+(−a)=0a + (-a) = 0a+(−a)=0.
5. **Multiplicative Inverses**:
    - For each a∈Fa \in Fa∈F, a≠0a \neq 0a=0, there exists an element a−1∈Fa^{-1} \in Fa−1∈F such that a⋅a−1=1a \cdot a^{-1} = 1a⋅a−1=1.
6. **Distributivity of Multiplication over Addition**:
    - a⋅(b+c)=(a⋅b)+(a⋅c)a \cdot (b + c) = (a \cdot b) + (a \cdot c)a⋅(b+c)=(a⋅b)+(a⋅c)