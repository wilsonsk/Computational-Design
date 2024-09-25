# Linear Combinations
Linear combinations are a fundamental concept because they express how different quantities (in this case, the variables $x,y,z$) can be combined in a way that maintains [[#The Fundamental Property (i.e. Linearity)|linearity]] (no exponents or products of variables). 
	This ensures that the equations describe flat objects like lines and planes, which are inherently linear geometric entities.

Both equations ax+by=cax + by = cax+by=c and ax+by+cz=dax + by + cz = dax+by+cz=d are forms of linear combinations. 
	They are linear combinations of the variables xxx, yyy, and zzz, with the coefficients aaa, bbb, and ccc acting as the weights in this combination, which is why they represent straight lines and flat planes.
		 This is conceptually tied to how vectors work, but the equations themselves are linear combinations in their own right.

## Linear Combination of Two Vectors
When you take two vectors, say **u** and **v**, and form a linear combination with scalars λ1\lambda_1λ1​ and λ2\lambda_2λ2​, the result will indeed be another vector that lies in the plane (or line) defined by those two vectors.

w=λ1u+λ2v\mathbf{w} = \lambda_1 \mathbf{u} + \lambda_2 \mathbf{v}w=λ1​u+λ2​v

This means that the vector **w** is the result of "scaling" **u** by λ1\lambda_1λ1​ and **v** by λ2\lambda_2λ2​, and then summing them. 
	If **u** and **v** are not collinear, they span a plane, and **w** will be some vector in that plane. If **u** and **v** are collinear, then all linear combinations of **u** and **v** will lie along a line.
		Colinear meaning they are both expressions of the same line, by multiples (i.e. scalars).
### A Connection to [[Straight Lines|Lines]] and [[Planes|Planes]]
The equations of lines and planes in the forms ax+by=cax + by = cax+by=c and ax+by+cz=dax + by + cz = dax+by+cz=d can indeed be understood as linear combinations, and have a connection to vectors.

## Linear Equation of a Line
For the equation ax+by=cax + by = cax+by=c, this is a linear combination of xxx and yyy. The equation expresses that a certain weighted sum (via the coefficients aaa and bbb) of the xxx and yyy coordinates equals a constant ccc.

This form can be linked to vectors because if we think of (x,y)(x, y)(x,y) as coordinates in the plane, the coefficients aaa and bbb can be seen as components of a normal vector to the line. The equation is effectively saying that for any point (x,y)(x, y)(x,y) on the line, the dot product of the vector (x,y)(x, y)(x,y) with the normal vector (a,b)(a, b)(a,b) gives the constant ccc. This aligns with how a linear combination works because it’s a sum of terms where each term involves a scalar multiple of a variable (which you can associate with a direction in space, i.e., a vector).

### Connecting the Two Ideas:
In the vector scenario, the equation λ1u+λ2v=w\lambda_1 \mathbf{u} + \lambda_2 \mathbf{v} = \mathbf{w}λ1​u+λ2​v=w tells you that any vector w\mathbf{w}w can be written as a linear combination of two vectors u\mathbf{u}u and v\mathbf{v}v, meaning w\mathbf{w}w lies within the span (or plane) of u\mathbf{u}u and v\mathbf{v}v.

In the line equation, ax+by=cax + by = cax+by=c is similarly describing all points (x,y)(x, y)(x,y) that satisfy a certain linear relationship, meaning they lie along a line (which can be thought of as the span of a vector).

Both expressions are linear combinations:

- In the vector case, it’s a combination of the vectors u\mathbf{u}u and v\mathbf{v}v.
- In the line equation, it's a combination of the coordinates xxx and yyy, scaled by aaa and bbb.

### Why They Look Similar:

The key reason they look similar is that both are expressing **linear relationships**. Whether you're combining vectors to describe points in a plane (or line) or you're using coefficients to combine variables like xxx and yyy to describe a line, you're dealing with the same underlying mathematical structure: **linearity**.

- In vector form, λ1u+λ2v\lambda_1 \mathbf{u} + \lambda_2 \mathbf{v}λ1​u+λ2​v defines a linear space (a line or plane).
- In the standard equation form, ax+by=cax + by = cax+by=c defines a line as the set of points where the linear combination of xxx and yyy equals a constant.

### Geometrically:

- **In vector terms**: The set of all linear combinations of two vectors **u** and **v** defines a line or a plane, depending on whether the vectors are collinear or not.
- **In equation terms**: The standard form ax+by=cax + by = cax+by=c defines a line in a plane by constraining xxx and yyy to satisfy a particular linear relationship.
## Linear Equation of a Plane:

Similarly, for the equation of a plane, ax+by+cz=dax + by + cz = dax+by+cz=d, this is also a linear combination of the variables xxx, yyy, and zzz, where aaa, bbb, and ccc are the scalar coefficients.

Here, aaa, bbb, and ccc can be interpreted as the components of a normal vector to the plane, and the equation says that for any point (x,y,z)(x, y, z)(x,y,z) on the plane, the weighted sum (dot product) of the vector (x,y,z)(x, y, z)(x,y,z) with the normal vector (a,b,c)(a, b, c)(a,b,c) equals the constant ddd.

In both cases, the "linear combination" aspect comes from the fact that you're summing the products of scalar coefficients and variables (which can be associated with directions in the vector space). The result of this sum is set equal to a constant, and this structure is what defines a linear relationship between the variables.









A linear combination involves creating a new vector (or value) by multiplying a set of vectors (or numbers) by scalars and then summing the results. Formally, if you have vectors v1,v2,…,vn\mathbf{v_1}, \mathbf{v_2}, \ldots, \mathbf{v_n}v1​,v2​,…,vn​ and scalars a1,a2,…,ana_1, a_2, \ldots, a_na1​,a2​,…,an​, the linear combination is:
## The Fundamental Property (i.e. Linearity)
**Linearity**:
A linear proportion is a relationship between two variables where one variable is a constant multiple of the other. 

This property is preserved in linear combinations, which means that the sum of scaled vectors (or variables) will also maintain linear relationships.

**Constant Multiples**: 
Linear proportion shows that scaling one variable by a constant results in a directly proportional change in the other variable. In a linear combination, each term is scaled by a constant (scalar multiplier), preserving the linear relationship.
	**Example**: If you have two vectors v1\mathbf{v_1}v1​ and v2\mathbf{v_2}v2​, their linear combination a1v1+a2v2a_1\mathbf{v_1} + a_2\mathbf{v_2}a1​v1​+a2​v2​ is scalable. If v1\mathbf{v_1}v1​ and v2\mathbf{v_2}v2​ are scaled by constants, their combination remains linear.

**Additivity**:
- **Sum of Proportions**: In linear combinations, adding together multiple terms (each term being a scaled vector or variable) still results in a linear relationship. This is akin to combining multiple linear proportions.
- **Example**: If y1=k1xy_1 = k_1xy1​=k1​x and y2=k2xy_2 = k_2xy2​=k2​x, then the sum y=y1+y2=k1x+k2x=(k1+k2)xy = y_1 + y_2 = k_1x + k_2x = (k_1 + k_2)xy=y1​+y2​=k1​x+k2​x=(k1​+k2​)x also maintains a linear relationship with xxx.

## Linear Proportion as a Simple Linear Combination:

- A linear proportion can be viewed as a specific, simple case of a linear combination.
- Consider the linear proportion y=kxy = kxy=kx. This can be thought of as a linear combination where you have a single vector (or number) xxx and a single scalar kkk. Here, yyy is the result of the linear combination kxkxkx.

## Extension to Multiple Variables:

- Linear combinations generalize the concept of linear proportion to multiple variables. Instead of relating just two variables as in a linear proportion, a linear combination involves multiple terms.
- For example, in a linear combination like y=a1x1+a2x2+…+anxny = a_1x_1 + a_2x_2 + \ldots + a_nx_ny=a1​x1​+a2​x2​+…+an​xn​, each xix_ixi​ is weighted by a corresponding scalar aia_iai​, creating a new variable yyy that is the sum of these weighted terms.
- If we think of each xix_ixi​ as representing a different dimension, the linear combination yyy represents a linear proportion in a higher-dimensional space.