# Fields
The term "field" (denoted as $F$) refers to a set along with two operations, addition and multiplication, that satisfy the field axioms. 
	A field is a mathematical structure used in linear algebra to define scalar values for vector spaces.
	
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