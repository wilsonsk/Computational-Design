# Mapping ($n : m$)
A mapping is a broad concept that refers to **any rule or process that associates elements of one set with elements of another set**. 
	This can include a wide variety of correspondences, not necessarily adhering to strict rules of uniqueness or well-defined behavior.

The broadest concept, encompassing any rule that associates elements of one set with elements of another. This includes functions, relations, and transformations.
###### Mappings Are Not Restricted to Be Represented by Ordered Pairs
They include any of the associations.
## [[Abstract Mathematical Spaces#Structured Set (i.e. Space)|Sets]]
A set is a well-defined **collection of distinct objects**, considered as an entity in its own right (and thus an element of some superset).  
	The items which constitute a particular set are called the elements or members of the set.
		Sets are one of the fundamental building blocks in mathematics and are used to define domains, codomains, and the relationships between them.
## Domain
The domain of a mapping (or function) is the **set of all possible input values**. It is the set from which the first elements of the ordered pairs are taken.
## Codomain
The codomain of a mapping (or function) is the **set of all potential output values**. 
	It is the set that contains all possible results of the mapping, whether or not all elements in the codomain are actually produced by elements of the domain.
## Range
The range (or image) of a mapping (or function) is the **set of all actual output values** that are produced by applying the function to every element in the domain. 
	The range is always a subset (or equal to) the codomain.
## Associations
Associations define how elements of one set (the domain) are related to elements of another set (the codomain). 
	These associations can vary based on the number of elements in the domain that are related to elements in the codomain and vice versa.
### One to One, ($\LARGE 1:1$)
Each element in the domain set $A$ is related to exactly one unique element in the codomain set $B$, and each element in $B$ is related to exactly one unique element in $A$.
			$$\LARGE \text{Let } A = \{1, 2, 3\} \text{ and } B = \{a, b, c\}$$
			$$\LARGE \text{A one-to-one relation can be } R = \{(1, a), (2, b), (3, c)\}$$
### One to Many, ($\LARGE 1:n$ )
An element in the domain set $A$ can be related to multiple elements in the codomain set $B$.
	 $$\LARGE \text{Let} A = \{1, 2\} \text{ and } B = \{a, b, c\}$$
	  $$\LARGE \text{A one-to-many relation can be } R = \{(1, a), (1, b), (1, c), (2, a)\}$$
### Many to One, ($\LARGE n:1$)
Multiple elements in the domain can be related to the same single element in the codomain.
$$\LARGE \text{If } A = \{1, 2\} \text{ and } B = \{a\}$$
$$\LARGE \text{A many-to-one relation could be } R = \{(1, a), (2, a)\}.$$
### Many to Many, ($\LARGE n:m$)
Multiple elements in the domain set $A$ can be related to multiple elements in the codomain set $B$.
$$\LARGE \text{Let } A = \{1, 2, 3\} \text{ and } B = \{a, b\}$$
$$\text{A many-to-many relation can be } R = \{(1, a), (1, b), (2, a), (2, b), (3, a), (3, b)\}$$
## Relationships as a Subset of Mappings ($1 : n$)
A relation between two sets is a collection of ordered pairs, where each pair consists of one element from each set. 
	The key characteristic of a relation is that it explicitly involves ordered pairs, showing the association between elements of the two sets.
		A relation allows an element in the domain to be associated with multiple elements in the codomain.
			It generalizes the concept of a function by allowing an element in the domain to be associated with multiple elements in the codomain.
#### Associations of Relations
## Functions as a Subset of Relations ($1 : 1$, $m:1$)
A function is a specific type of relation where each element in the domain is associated with exactly one element in the codomain.
	Functions are well-defined mappings with unique outputs for each input.
#### Associations of Functions
Functions **can** be
$\LARGE 1:1$ or $\LARGE m:1$.

But **not** $\LARGE 1:m$ or $\LARGE n:m$.
#### Standard Function
A function $\mathbb{R} \to \mathbb{R}$ maps real numbers to real numbers.
- **Input and Output**: The input is a real number, and the output is a real number.
## Transformations as a Subset of Functions ($1:1$, $m:1$)
A transformation is a type of function, often used to emphasize changes or operations applied to the elements of a set. 
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
- **Linear Transformation**: T(x)=AxT(\mathbf{x}) = A\mathbf{x}T(x)=Ax, where AAA is a matrix.
- **Affine Transformation**: T(x)=Ax+bT(\mathbf{x}) = A\mathbf{x} + \mathbf{b}T(x)=Ax+b, where AAA is a matrix and b\mathbf{b}b is a vector.
- **Non-linear Transformation**: T(x)=x3T(x) = x^3T(x)=x3.
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

## Functions as Ratios
## Functions on Functions (i.e. Functional)
A different concept is a functional, which is a function whose input is another function. This is more closely related to the concept of functional analysis, which deals with function spaces.

- **Functional**: A functional FFF maps a function fff to a scalar. For example, the integral of a function over a specified interval is a functional.