# Mapping ($n : m$)
## [[Abstract Mathematical Spaces#Structured Set (i.e. Space)|Sets]] as Precedence for Mapping
A set is a well-defined **collection of distinct objects**, considered as an entity in its own right (and thus an element of some superset).  
	The items which constitute a particular set are called the elements or members of the set.
		Sets are one of the fundamental building blocks in mathematics and are used to define domains, codomains, and the relationships between them.
## Cartesian Product as a Fundamental Concept of Mappings
The Cartesian product of two sets $A$ and $B$, denoted $A \times B$, is the set of all ordered pairs $(a, b)$ where $a \in A$ and $b \in B$b.
$$\LARGE A×B={(a,b)∣a∈A \text{ and } b∈B}$$

The Cartesian product creates a new set from existing sets, which includes all possible ordered pairs of elements from the two sets.
	This new set provides a structured way to describe relationships between elements of the two original sets.

The Cartesian product allows for a clear and structured representation of all possible pairs of elements from two sets. 
	This structured representation is essential for defining precise rules for how elements from one set are associated with elements from another set.

- - -
## A Relation as a Subset of the Cartesian Product ($1 : n$)
Subsets of the Cartesian product representing **associations** between sets.

Relations provides the basic framework for associating elements of one set with elements of another set without imposing additional constraints. 

A **relation** between two sets $a$ and $B$ is any subset of the Cartesian product $A \times B$.
	It describes how elements of $A$ are associated with elements of $B$.
	
If $R$ is a relation from set $A$ to set $B$, then $R$ is a subset of $A \times B$

$$\LARGE R \subseteq A \times B$$
A relation between two sets is a collection of ordered pairs, where each pair consists of one element from each set. 
	It describes how elements from one set are related to elements of another set (or the same set).
		The key characteristic of a relation is that it explicitly involves ordered pairs, showing the association between elements of the two sets.
			A relation allows an element in the domain to be associated with multiple elements in the codomain.
				It generalizes the concept of a function by allowing an element in the domain to be associated with multiple elements in the codomain.

**Relations** in mathematics describe connections or associations between elements of a set. 
	A relation is a subset of the Cartesian product of a set with itself, defining how elements are related to one another.
		 Relations do not necessarily produce new elements within the set; rather, they characterize how existing elements interact or compare with each other.
### How Relations Dictate Mappings and Operations
1. **Relations Dictating Mappings**:
    - A relation can define how elements of one set correspond to elements of another set.
    - For example, the relation "is the square of" defines a mapping between the set of real numbers and itself: $y = x^2$.
2. **Functions and Operations Representing Relations**:
    - Functions are specific kinds of relations where each input is related to one output.
    - Operations (like addition, multiplication) are functions that perform specific actions on inputs.
    - For example, the relation $y = f(x)$, where $f$ is a function, describes how each $x$ maps to $y$.

> [!note]
> ### Types of Relations
These define specific properties or characteristics of how elements within a single set relate to each other.
>##### Reflexive Relation
Every element is related to itself.
>	*Example*: "is equal to" (e.g., $(a, a)$ for all $a \in A$).
>##### Symmetric Relation
If $(a, b)$ is in the relation, then $(b, a)$ is also in the relation.
>	*Example*: "is married to" (if $a$ is married to $b$, then $b$ is married to $a$).
>##### Transitive Relation
If $(a, b)$ and $(b, c)$ are in the relation, then $(a, c)$ is also in the relation.
>	*Example*: "is an ancestor of" (if $a$ is an ancestor of $b$ and $b$ is an ancestor of $c$, then $a$ is an ancestor of $c$).
>##### Equivalence Relation
A relation that is reflexive, symmetric, and transitive.
>	*Example*: "is congruent to" in geometry.

>[!note]
>### Associations of Relations
These describe how elements from two different sets are paired or associated, often emphasizing the nature of the pairing across different sets.
>##### General Association
Here, element 1 in Set A is associated with element 'a' in Set B, element 2 is associated with both 'a' and 'b', and element 3 is associated with 'b'.
>	There are no restrictions on how the associations are made.
>- **Set A**: {1, 2, 3}
>- **Set B**: {a, b}
>- **Relation R**: {(1, a), (2, a), (2, b), (3, b)}
>##### Non-Functional Relation
A relation can include pairs where one element in the domain is related to multiple elements in the codomain.
>	*Example*: {(x, y), (x, z)} where x is related to both y and z.
>##### Symmetric Relation
If (a, b) is in the relation, then (b, a) is also in the relation.
>	*Example*: The relation "is a sibling of" in a set of people. If Alice is a sibling of Bob, then Bob is a sibling of Alice.

- - -
## A Mapping as a Subset of Relations
Mappings, in their broadest sense, are a subset of relations, as they are a specific type of association between elements of two sets.
	While relations encompass any possible association between elements of two sets, mappings are a more structured concept that can include functions, multivalued mappings, and other types of correspondences. 

A mapping is a broad concept that refers to **any rule or process that associates elements of one set with elements of another set**. 
	This can include a wide variety of correspondences, not necessarily adhering to strict rules of uniqueness (i.e. functions) or well-defined behavior.

>[!note]
>## Mapping Associations 
>Associations define how elements of one set (the domain) are related to elements of another set (the codomain). 
	>These associations can vary based on the number of elements in the domain that are related to elements in the codomain and vice versa.
>### One to One, ($\LARGE 1:1$), aka Injective Mapping
>Each element in the domain set $A$ is related (i.e. mapped) to exactly one unique element in the codomain set $B$, and each element in $B$ is related to exactly one unique element in $A$.
>$$\LARGE \text{Let } A = \{1, 2, 3\} \text{ and } B = \{a, b, c\}$$
>$$\LARGE \text{A one-to-one relation can be } R = \{(1, a), (2, b), (3, c)\}$$
>### One to Many, ($\LARGE 1:n$ ), aka Multivalued Mapping
>An element in the domain set $A$ can be related (i.e. mapped) to multiple elements in the codomain set $B$.
> $$\LARGE \text{Let} A = \{1, 2\} \text{ and } B = \{a, b, c\}$$
>$$\LARGE \text{A one-to-many relation can be } R = \{(1, a), (1, b), (1, c), (2, a)\}$$
>### Many to One, ($\LARGE n:1$), aka Surjective Mapping
>Multiple elements in the domain can be related (i.e. mapped) to the same single element in the codomain.
>$$\LARGE \text{If } A = \{1, 2\} \text{ and } B = \{a\}$$
>$$\LARGE \text{A many-to-one relation could be } R = \{(1, a), (2, a)\}.$$
>### Many to Many, ($\LARGE n:m$), aka General Relation
>Multiple elements in the domain set $A$ can be related (i.e. mapped) to multiple elements in the codomain set $B$.
>$$\LARGE \text{Let } A = \{1, 2, 3\} \text{ and } B = \{a, b\}$$
>$$\text{A many-to-many relation can be } R = \{(1, a), (1, b), (2, a), (2, b), (3, a), (3, b)\}$$
## A Mapping Defines the [[Abstract Mathematical Spaces#Structure|Structure]] of a [[Abstract Mathematical Spaces#Structured Set (i.e. Space)|Structured Set]]
By defining these interactions, which shapes the domain, codomain, and range within the context of the structured set.
	The domain, codomain, and range are the primary sets that are structured by the mappings (relations, functions, operations) within a structured set. 
		These mappings define the relationships and interactions between elements of these sets, thereby determining their structure.
### Domain as a Subset of the Underlying Set
The domain of a mapping (or function) is the **set of all possible input values** that the mapping can process.
	It is the set from which the first elements of the ordered pairs are taken.

The domain is structured by the mapping because the mapping defines which elements are included as valid inputs.
	The structure of the domain is shaped by the requirements and constraints imposed by the mapping.
### Codomain as a Subset of Domain
The codomain of a mapping (or function) is the **set of all potential output values** that the mapping can produce. 
	It is the set that contains all possible results of the mapping, whether or not all elements in the codomain are actually produced by elements of the domain.

The codomain is defined by the mapping as the set of possible results that the mapping can produce.
	The structure of the codomain is influenced by the nature of the mapping and the type of outputs it can generate.

Using the Cartesian product clarifies the definitions of mappings by providing a concrete way to describe the associations between elements. 
	It allows us to talk about mappings in terms of sets of ordered pairs, which is crucial for mathematical rigor and precision.

Relations and functions are defined as subsets of the Cartesian product. 
	Without the Cartesian product, it would be difficult to formally describe and work with these subsets.
### Range as a Subset of Codomain
The range (or image) of a mapping (or function) is the **set of all actual output values** that are produced by the mapping (i.e. by applying the function to every element in the domain). 
	The range is always a subset (or equal to) the codomain.

The range is directly determined by the mapping as it is the actual set of outputs obtained. 
	The structure of the range is a subset of the codomain, specifically those elements that are realized through the mapping.

- - -
## A Function as a Subset of Mappings ($1 : 1$, $m:1$)
Special type of relation with a **uniqueness constraint on the association**.

A function is a specific type of Mapping where each element in the domain is associated with exactly one element in the codomain.
	Functions are well-defined mappings with unique outputs for each input.

Formally, a function $f$ from set $A$ to set $B$ is defined such that every element $a$ in $A$ is associated with exactly one element $b$ in $B$. 
$$\LARGE f: A \to B$$
#### Properties of Functions
1. **Uniqueness**: Each element in the domain is associated with exactly one element in the codomain.
2. **Well-defined**: For every $a \in A$, there is a unique $b \in B$ such that $(a, b) \in f$
### Function Classification 
Functions can be classified based on different criteria. 
	Two primary ways to classify functions are by the **nature of their associations** and by the **nature of their outputs**.
#### Associations of Functions
> [!note]
> These describe how elements from two different sets are paired or associated, often emphasizing the nature of the pairing across different sets.
> 	This describes how elements in the domain map to elements in the codomain, focusing on the uniqueness and nature of the mapping.
> 
> **Uniqueness Requirement**:  Each element in the domain is associated with exactly one element in the codomain.
> 	This rule ensures that each input (element in the domain) maps to a single output (element in the codomain).
> 		Functions **can** be
> 			$\LARGE 1:1$ or $\LARGE m:1$.
> 				**Cannot** be $\LARGE 1:m$ or $\LARGE n:m$.
> 					These violate the uniqueness requirement, as elements in the domain would map to more than one element in the codomain.
> ##### Injective (One-to-One) Function
> A function $f: A \to B$ is injective if different elements in $A$ map to different elements in $B$. 
> 	Formally, if $f(a_1) = f(a_2)$ implies $a_1 = a_2$.
> 
> **Example**: If $A = \{1, 2, 3\}$ and $B = \{a, b, c, d\}$, an injective function could be $f = \{(1, a), (2, b), (3, c)\}$.
> ##### Surjective (Onto) Function
> A function $f: A \to B$ is surjective if every element in $B$ is the image of at least one element in $A$. 
> 	Formally, for every $b \in B$, there exists an $a \in A$ such that $f(a) = b$.
> 
> **Example**: If $A = \{1, 2, 3\}$ and $B = \{a, b\}$, a surjective function could be $f = \{(1, a), (2, b), (3, a)\}$.
> ##### Bijective (One-to-One and Onto) Function
> A function $f: A \to B$ is bijective if it is both injective and surjective.
> 	This means that every element in $A$ maps to a unique element in $B$, and every element in $B$ is the image of a unique element in $A$.
> 
> **Example**: If $A = \{1, 2, 3\}$ and $B = \{a, b, c\}$, a bijective function could be $f = \{(1, a), (2, b), (3, c)\}$.
> ##### Constant Function
> A function $f: A \to B$ is constant if all elements in $A$ are mapped to the same single element in $B$.
> 
> **Example**: If $A = \{1, 2, 3\}$ and $B = \{a\}$, a constant function could be $f = \{(1, a), (2, a), (3, a)\}$.
> ##### Identity Function
> A function $f: A \to A$ is the identity function if every element maps to itself. Formally, $f(a) = a$ for all $a \in A$.
> 
> **Example**: If $A = \{1, 2, 3\}$, the identity function is $f = \{(1, 1), (2, 2), (3, 3)\}$.
#### Output Types of Functions
##### *For Context Within Structured Sets, See: [[Abstract Mathematical Spaces#Preservation Through Inheritance and Extension of Function Output and Input Types|Preservation Through Inheritance and Extension of Function Output and Input Types]]*
##### Output Type Preserved (i.e. Determined) by Inheritance
###### Function Output Types Are Determined by the Fields or Spaces in Which the Functions Are Defined (i.e. The Lower Level Imparting Field or Space)
Functions can be characterized by their output types, and these types are inherently dependent on the field or space within which they exist. 
	This dependency shapes how functions are defined and how their outputs are structured. 
		Furthermore, function types exhibit a hierarchical nature, where more complex function types build upon simpler ones, inheriting their properties and extending their applicability to higher-dimensional spaces.

Function types based on output can be seen as hierarchical.
	Where scalar functions within the field of real numbers is inherited by any space that is a itself a subset of the real number field.
##### Input Type Preserved (i.e. Determined) by Extensions
###### Function Input Types Are Determined by the Fields or Spaces in Which the Functions Operate (i.e. The Higher Level Inheriting Spaces)
Extension is represented by the fact that this inherited function can now take as input some type of value from the inheriting domain, extending its applicability to more complex structures.
	The inherited function can now take as input some type of value from the inheriting domain, extending its applicability.

> [!note]
> This categorizes functions based on the nature of their output values.
> ##### [[Abstract Mathematical Spaces#Scalar Functions|Scalar Functions]]
> **Field Dependency:** Scalar functions exist within the context of fields, such as the real number field $\mathbb{R}$.
> **Output Type:** The output of scalar functions is defined by the field they belong to. For example, a scalar function $f: \mathbb{R} \to \mathbb{R}$ produces real number outputs.
> **Fundamental:** Scalar functions represent the most fundamental level, dealing with outputs in their respective fields.
> $$\LARGE f:\mathbb{R} \to \mathbb{R}$$
> A scalar function maps one or more scalar (i.e. a real number, complex number, etc.) elements from its domain to a single scalar (i.e. real numbers, complex number, etc.) output.
> $$\LARGE f(x) = x^2 + 3x + 5$$
> Here, \( f \) maps a real number \( x \) to another real number \( f(x) \).
>###### For 2 Variables
$$f(x,y)$$
>###### For 3 Variables
>$$f(x,y,z)$$
>###### For $n$ Variables
>$$f(x_1, x_2, \ldots, x_n)$$
> ##### [[Abstract Mathematical Spaces#Vector Function|Vector-Valued Functions]]
> A vector-valued function maps elements from its domain to vectors.
> $$\LARGE \mathbf{f}: D \to V$$
> Where $D$ is the domain and $V$ is a vector space.
> **Space Dependency:** These functions exist within vector spaces derived from fields. For example, vector spaces like $\mathbb{R}^2$, $\mathbb{R}^3$, or $\mathbb{R}^n$ are derived from the real number field.
> **Output Type:** The output is a vector in a specific vector space, which is itself defined by the underlying field.
> $$\LARGE \mathbf{f}(t) = \begin{pmatrix} t \\t^2 \\t^3\end{pmatrix}$$
> Here, $\mathbf{f}$ maps a scalar $t$ to a 3-dimensional vector.
> ##### Matrix-Valued Functions
> A matrix-valued function maps elements from its domain to matrices.
> $$\LARGE F(t) = \begin{pmatrix}t & t^2 \\\sin(t) & \cos(t)\end{pmatrix}$$
> Here, $F$ maps a scalar $t$ to a $2x2$ matrix.
> ##### Complex-Valued Functions
> A complex-valued function maps elements from its domain to complex numbers.
> $$\LARGE f(z) = z^2 + 1$$
> Here, \(f\) maps a complex number \(z\) to another complex number.
> ##### Boolean Functions
> A Boolean function maps elements from its domain to Boolean values (true or false, or equivalently, 1 or 0).
> $$\LARGE f(x, y) = x \land y$$
> Here, \(f\) maps pairs of Boolean values to a single Boolean value using the logical AND operation.
> ##### Set-Valued Functions
> A set-valued function (or multivalued function) maps elements from its domain to sets of values rather than single values.
> $$\LARGE F(x) = \{y \in \mathbb{R} \mid y^2 = x\}$$
> Here, $(F)$ maps a real number $x$ to the set of its square roots.
> ##### Operator-Valued Functions
> An operator-valued function maps elements from its domain to operators.
> $$\LARGE T(t)(x) = e^{tA}x$$
> Here, $(T(t))$ is a function that maps $(t)$ to the operator $(e^{tA})$, which acts on the vector $(x)$.
> ##### Tensor-Valued Functions
> A tensor-valued function maps elements from its domain to tensors.
> $$\LARGE T(x, y, z) = x \otimes y \otimes z$$
> Here, $(T)$ maps three vectors $(x, y, z)$ to their tensor product.
> ##### Piecewise Functions
> Piecewise functions map elements from their domain to different values depending on which subdomain the input falls into.
> $$\LARGE f(x) =\begin{cases} x^2 & \text{if } x < 0 \\x + 1 & \text{if } x \geq 0 \end{cases}$$
> Here, $(f)$ maps 4 to $(x^2)$ for negative values and to $(x + 1)$ for non-negative values.

- - -
## An Operation as a Subset of Functions
Functions that define how elements of a set interact within an algebraic structure.

**Operations** in mathematics are functions that combine elements of a set to produce another element of the same set. 
	Operations are a subset of functions characterized by their specific rules for combining or transforming elements.
		They are rules that define how to combine elements within the [[Abstract Mathematical Spaces#Structure|structure]]. 
			Operations are fundamental in defining algebraic structures such as groups, rings, and fields.
### Association Types of Operations
Operations are typically associated with specific types of functions based on how they combine or transform elements. 
1. **One-to-One (1:1) Association**
2. **Many-to-One (m:1) Association**
### Types of Operations
Operations can be categorized based on the number of operands and the nature of the operation.
> [!note]
> #### Unary Operations
> Operations that take a single input (i.e. operand) from a set and produce an output in the same or a related set.
> - **Examples**:
>     - **Negation**: $f(a) = -a$
>     - **Square Root**: $f(a) = \sqrt{a}$ (defined for non-negative real numbers)
> #### Binary Operations
> Operations that take two inputs (i.e. operands) from a set and produce an output in the same set.
> - **Examples**:
>     - **Addition**: $f(a, b) = a + b$
>     - **Multiplication**: $f(a, b) = a \cdot b$
>     - **Division**: $f(a, b) = a / b$ (with $b \neq 0$)
> #### Higher-Arity Operations
> Operations that take more than two inputs (i.e. operands).
> - **Examples**:
>     - **Sum**: $\Sigma(a_1, a_2, \ldots, a_n) = a_1 + a_2 + \ldots + a_n$
>     - **Product**: $\Pi(a_1, a_2, \ldots, a_n) = a_1 \cdot a_2 \cdot \ldots \cdot a_n$

- - - 
## A Transformation as a Subset of Functions ($1:1$, $m:1$)
A **transformation** is fundamentally a type of **function**.
	Where a function is a rule that assigns each element in one set (called the domain) to a single element in another set (called the codomain).
		A transformation is a function that maps a set to itself or another set, often preserving some structure.
			**"A function that maps a set to itself or another set"** means that a transformation can take elements from one set and map them either back to the same set or to a different set.
				In this sense, a transformation does what a function does (maps each element of a set to a single element of another set) but also preserves some structure of the set, which is the distinguishing feature.
					 This preservation of structure is what makes transformations particularly important in certain fields of mathematics and physics.
				**Example of Mapping within the same set**: 
					If you have a set of points on a plane, a transformation could rotate all the points around the origin. 
						Here, both the domain and codomain are the same set of points on the plane.
				**Example of Mapping to a different set**: 
					If you have a set of temperatures measured in Celsius, a transformation could convert these to temperatures in Fahrenheit. 
						Here, the domain is the set of temperatures in Celsius, and the codomain is the set of temperatures in Fahrenheit.
			**"Preserving some structure"** refers to the fact that many transformations maintain certain properties or structures of the set.
##### Function vs. Transformation
Both statements are describing the same core concept of a function.
	A function maps elements of the domain to elements of the codomain, ensuring each element in the domain is paired with exactly one element in the codomain."
###### "Maps each element of a set to a single element of another set"
**Focus on Elements**:
- This phrase emphasizes the rule that assigns each individual element of the domain to a single element in the codomain.
- It highlights the idea that each element in the domain is associated with exactly one element in the codomain.
- This is the fundamental definition of a function.
###### "Maps a set to itself or another set"
**Focus on the Set**:
- This phrase emphasizes the mapping of the entire set (domain) to another set (codomain).
- It indicates that the function can map the elements of a set either to itself (the same set) or to a different set.

A transformation is a type of function, often used to emphasize changes or operations applied to the elements of a set. 
	In linear algebra, transformations often refer to functions mapping vector spaces to vector spaces.
		Transformations are typically associated with geometric or algebraic contexts, where they might involve shifting, rotating, scaling, or otherwise altering the elements of a set or space.

A transformation is a general term for any operation that maps elements from one set to another. 
	This can include a wide variety of mathematical operations, not limited to functions in the traditional sense.
#### Associations of Transformations
Transformations inherit the properties of functions, meaning they can be
$\LARGE 1:1$.
	A linear transformation where each input vector is mapped to a unique output vector.
$\LARGE m:1$.
	A non-linear transformation where multiple input vectors are mapped to the same output vector.
##### Transformation Types
- **Linear Transformation**: $T(\mathbf{x}) = A\mathbf{x}$, where $A$ is a matrix.
- **Affine Transformation**: T$(\mathbf{x}) = \mathbf{x} + \mathbf{b}$, where $A$ is a matrix and $\mathbf{b}$ is a vector.
- **Non-linear Transformation**: $3T(x) = x^3$.
- **Projective Transformation**
	- A transformation that maps lines to lines but does not necessarily preserve parallelism. It includes perspective transformations.
- **Euclidean Transformation**
	- A transformation that preserves distances and angles. Also known as rigid transformations.
- **Similarity Transformation**
	- A transformation that preserves angles but not necessarily distances. It is a combination of a Euclidean transformation and uniform scaling.
- **Homeothety (Dilation)**
	- A transformation that scales objects by a constant factor, either enlarging or shrinking them.
		- T(x)=kx where kkk is a scalar.
- **Möbius Transformation**
	- A complex function that maps the extended complex plane onto itself, preserving the general form of rational functions.
- **Conformal Transformation**
	- A transformation that preserves angles but not necessarily lengths.
- **Fourier Transform**
	- A transformation that decomposes a function into its constituent frequencies.
- **Wavelet Transform**
	- A transformation that represents data or functions in terms of wavelets with different scales and positions.
- **Coordinate Transformation**
	- A change of coordinates that can be linear or non-linear, used to simplify equations or understand geometrical structures.

- - - 
## Scalar Functions as a Subset of Functions
###### *Remember*: Properties of Functions
1. **Uniqueness**: Each element in the domain is associated with exactly one element in the codomain.
2. **Well-defined**: For every $a \in A$, there is a unique $b \in B$ such that $(a, b) \in f$
$$\LARGE f:R^n \to R$$
A **Scalar Function** is a mathematical function that maps points from an $n$-dimensional domain to a single real number (a scalar).
	They are generally used to to describe a relationship between variables where the output is a single scalar value.
		A more general term used across various mathematical disciplines. 
			It emphasizes the mathematical relationship between the input and the output.
###### What Mapping From One Domain to a Scalar Value Means
Scalar functions can have domains composed of various objects, not just real numbers.
	These domains can be multi-dimensional spaces, sets of vectors, matrices, or other mathematical objects.
		Scalar functions can map elements from complex domains (like vectors, matrices, or higher-dimensional points) to scalar values to simplify analysis or represent a specific quantity.
### Scalar Functions are Defined by their Input Type and Output Type
Scalar functions are differentiated from other functions primarily by the type of their inputs and outputs.
#### Input of Scalar Functions
##### Domain
The input can be elements from various sets, often **points** in a vector space like $\mathbb{R}^n$.

**Domains Composed of Vectors or Points in the Algebraic or Spatial Sense**
Often, the domain of a scalar function can be a set of vectors or points in a multi-dimensional space (e.g., $\mathbb{R}^n$). 
	The term "point" and "vector" can often be used interchangeably in the context of vector spaces, as both represent an ordered tuple of numbers in a given space.
###### If the Domain is "Algebraic"
It is referred to as a Scalar Function.
###### If the Domain is "[[#Spatial Fields as a Subset of Functions|Spatial]]"
It is referred to as a Scalar Field.
##### Points of a Scalar Function
> [!note]
> Refers to elements of a set that serve as the domain of a function, without a spatial interpretation.
A "point" does not always need to have a spatial interpretation. 
>	A point can be an element of any set that serves as the domain of a function. 
> 
> **Abstract (Algebraic) Points in a Set** (For Scalar Functions)
> A point can be any element of a set that serves as the domain of a function.
> 	For a scalar function $: A \to \mathbb{R}$, where $A$ is a non-spatial set, points are elements of $A$.
> 		Example: Consider a set $S = \{a, b, c\}$.
> 			 A point in this set could be $a$, $b$, or $c$.
> 
> **Spatial Points in a Set** (For [[#Scalar Fields|Scalar Fields]])
> A spatial point is a specific location in a coordinate system that serves as the domain of a function.
> 	For a scalar function $f: \mathbb{R}^n \to \mathbb{R}$, where $\mathbb{R}^n$ is a spatial coordinate system, points are coordinates in $\mathbb{R}^n$.
> 		Example: Consider the 2-dimensional coordinate system $\mathbb{R}^2$.
> 			A point in this system could be $(x, y)$, where $x, y$ \in $\mathbb{R}$.
##### Output of Scalar Functions
**Codomain**: The output is a single scalar value in the real number field $\mathbb{R}$.
- - -
## Spatial Fields as a Subset of Functions
Fields, within various mathematical contexts, can be understood as specific types of functions. 
	They describe how quantities are distributed over a domain, often physical or abstract spaces, and are crucial in areas like physics, engineering, and mathematics.

From a functional perspective, fields can be seen as functions that provide a systematic way to describe variations of quantities over space and time. 
	This approach is essential in fields like calculus and physics, where the behavior of physical systems is studied through their spatial and temporal variations.
#### *See the Following for More Detailed Information:*
[[Fields|Fields]]
[[Abstract Mathematical Spaces#The Sequential Generation of the Field of Real Numbers and the Vector Space|The Sequential Generation of the Field of Real Numbers and the Vector Space]]
[[Abstract Mathematical Spaces#Spatial Fields|Spatial Fields]]

- - -

