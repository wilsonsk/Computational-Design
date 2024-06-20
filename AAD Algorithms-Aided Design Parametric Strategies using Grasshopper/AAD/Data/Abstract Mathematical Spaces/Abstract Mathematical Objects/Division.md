---
up:
  - "[[Abstract Mathematical Objects]]"
related: 
date created: 2024-05-31
---
# Division
Can be thought of as simply the amount of one quantity of a "thing" that is associated with a separate quantity of another "thing".
	I.e.  A ratio.

Division can be conceptualized as the operation of **distributing or partitioning one quantity by another**, thereby determining how many times the divisor is contained within the dividend.

Consider two quantities, a and b. 
	The division of a by b, $\LARGE {a\over b}$ seeks to determine the factor by which b must be scaled to obtain a. 
		This operation answers the question: "How many units of b are there in a?"
#### Abstract Interpretation
###### Distribution 
Division distributes the total quantity a into equal parts of size b. 
	*For example*, if a represents a collection and b the size of each subset, division tells us how many such subsets can be formed.
###### Measurement
Division measures the quantity a using the unit b. 
	If b is a standard unit, division indicates how many times this unit fits into a.
## Contracting
A transformation $T$ is called a **contracting transformation** (or simply a **contraction**) if there exists a constant $k$ with $\LARGE 0≤k<1$ such that for all points $x$ and $y$ in the space, the distance between $T(x)$ and $T(y)$ is strictly less than the distance between $x$ and $y$, scaled by $k$. 
###### Mathematically, this can be expressed as:
	$$\LARGE d(T(x),T(y))≤k⋅d(x,y)$$
		Where $d(\cdot, \cdot)$ represents the distance metric in the space.
###### Transformation $T$
This is a function that maps points in a space to other points in the same space.
###### Constant $k$**
This is the contraction constant, which must satisfy $0 \leq k < 1$. 
	The value of $k$ determines the degree of shrinking.
###### Distance $d(\cdot, \cdot)$
This is the metric used to measure the distance between two points in the space.
###### Euclidean Geometry
If you scale a figure by a factor $k$ where $0 \leq k < 1$, every point of the figure is moved closer to a fixed point (usually the origin), and the entire figure is reduced in size. This is a contraction.
###### Linear Algebra
A matrix representing a linear transformation is a contraction matrix if the norm of the matrix is less than 1.
###### Functional analysis
A contraction mapping on a metric space is a function that brings points closer together by a fixed ratio $k$ less than 1.

## Contraction by a Scalar
When we talk about contraction in the context of scaling with a scalar less than 1, we mean that we are effectively reducing the original quantity. 
	In mathematical terms, scaling a variable $p$ by a factor of $\frac{1}{k}$ (where $k > 1$) results in a smaller quantity.
#### Understanding $x = p \times \frac{1}{k}$
Given the equation $x = p \times \frac{1}{k}$, you can visualize or understand this as the total force $p$ being split into $k$ equal groups, where each group contains $x$ amount of the original $p$.
### Step-by-Step Mental Image
1. **Total Force $p$:**
    - Picture the total force $p$ as a large block or total quantity.
2. **Dividing into $k$ Groups:**
    - Divide this large block into $k$ smaller, equal groups.
    - Each group represents a fraction of the total force.
3. **Deflection Contribution $x$:**
	- The quantity $x$ represents the size or amount of each of these smaller blocks.
	- Mathematically, $x = p \times \frac{1}{k}$ shows that $x$ is the portion of $p$ contained in each of the $k$ parts.
    - Each group contains an amount of deflection $x$.
    - The total deflection $x$ is the portion of $p$ that each group contributes.
#### Mathematical Interpretation
The equation $x = p \times \frac{1}{k}$ can be rewritten as:
$$\LARGE x = \frac{p}{k}$$

This indicates that each of the $k$ groups contributes an equal amount $x$ from the total force $p$.

But also, if we then scale the $x$ amount contained by each of the $k$ pieces of $p$, then we obtain $p
	Where we would have $k$ many pieces of $x$ amount.
$$\LARGE xk = p$$
#### Example
Suppose $p = 6$ and $k = 2$:

- **Total Force $p = 6$:**
    - You have a total force of 6 units.
- **Dividing into $k = 2$ Groups:**
    - You divide this force into 2 equal groups.
    - Each group has $\frac{6}{2} = 3$ units.
- **Deflection Contribution $x$:**
    - Each group of 3 units of force contributes to the total deflection.
    - Thus, the total deflection $x$ is 3 units
#### Hooke's Law and Contraction Example
Hooke's Law states that the force $F$ needed to extend or compress a spring by some distance $x$ is proportional to that distance.
	The law can be written as:
$$F=kx$$
where:
- $F$ is the force applied to the spring,
- $k$ is the spring constant (a measure of the stiffness of the spring),
- $x$ is the displacement or deflection of the spring from its equilibrium position.
##### Understanding $x = \frac{F}{k}$
Rearranging Hooke's Law to solve for $x$ (the deflection), we get:
$$x = \frac{F}{k}$$
In this equation:
- $F$ represents the total force applied,
- $k$ represents the spring constant,
- $x$ represents the resulting deflection of the spring.
##### Visualizing Contraction
To understand $x = \frac{F}{k}$ as a form of contraction:
1. **Total Force $F$:**
    - Think of $F$ as a single large block representing the total force applied to the spring.
2. **Spring Constant $k$:**
    - The spring constant $k$ acts as a divisor, indicating how many parts the force $F$ is split into based on the stiffness of the spring.
3. **Resulting Deflection $x$:**
    - The deflection $x$ is the portion of the total force $F$ that results in the displacement of the spring. It is calculated by dividing the total force $F$ by the spring constant $k$.
##### Detailed Verbal Explanation
Imagine you have a certain amount of force $F$ (like pushing on a spring) and you want to see how much the spring stretches. 
	The spring constant $k$ tells you how stiff the spring is, and this stiffness affects how much the spring stretches when you apply the force.
1. **The Whole Quantity $F$:**
    - Picture $F$ as the total force you apply to the spring. This is a complete, undivided amount of force.
2. **Dividing into $k$ Equal Parts:**
    - The spring constant $k$ divides this total force into $k$ smaller, equal parts. If $k$ is large (a stiff spring), each part is small, meaning the spring doesn't stretch much. If $k$ is small (a less stiff spring), each part is larger, meaning the spring stretches more.
3. **Each Part’s Contribution to Deflection $x$:**
    - The deflection $x$ is the amount of stretch that each of these $k$ parts contributes to the total stretch of the spring. Essentially, $x = \frac{F}{k}$ tells you how much each part of the force contributes to the overall deflection.
#### Abstract Thinking about Division
To understand division abstractly, think about it in a similar way to multiplication:
1. **Multiplication:**
    - When we multiply $a$ by $b$, we are scaling $b$ to have $a$ many instances of $b$. 
	    - For example, $a \times b$ means we have $a$ groups, each containing $b$ units.
1. **Division:**
    - When we divide $a$ by $b$, we are scaling $a$ down by distributing it into $b$ equal parts. 
	    - For example, $a / b$ means we split $a$ into $b$ groups, each containing $\frac{a}{b}$ units.
#### Practical Examples
###### Number Division
10/2​=5 indicates that 10 can be divided into 5 parts, each of size 2.
###### Vector Scaling
Dividing a vector 𝑣⃗ by a scalar k scales the vector by k1​, effectively shrinking or expanding it inversely.
	Just as multiplication scales one quantity by another, division as a ratio scales down one quantity by the other, showing the extent to which one is a fraction of the other.
###### Function Division
For functions f(x) and g(x), g(x)f(x)​ determines how the values of f compare to those of g point by point.
## Ratio	
That is a relationship between two quantities, expressed as the quotient of one divided by the other.
	I.e. Division as a ratio is the operation that defines the comparative relationship between two quantities, a and b, expressed as ba​. 
		This ratio reflects how many units of b are contained within a, providing a dimensionless measure of their relative magnitudes.

If we consider two variables a and b, the ratio of a to b is ba​.
	This abstraction applies whether a and b are elements of a set of numbers, vectors in a vector space, measures of physical quantities, or even more abstract entities such as functions or probabilities.

The significance of a ratio lies in its ability to provide a dimensionless measure of relative size or magnitude, enabling the comparison of different entities on a common scale. 
	This abstract conceptualization of a ratio extends to numerous fields, including geometry, algebra, probability theory, and more, where it serves as a fundamental tool for understanding proportional relationships and comparative analysis.
#### Abstract Interpretation of Division as a Ratio:
###### Comparison
Division as a ratio expresses the relative size of one quantity to another. 
	*For example*, the ratio ba​ shows how 𝑎a compares to b.
###### Proportionality
This relationship reveals the proportion of one quantity to another, often indicating a balance or imbalance between them.
#### Mathematical Context:
###### Basic Ratio
For quantities a and b, the ratio ba​ represents how many times b fits into a. 
	This can be interpreted as the factor by which b must be scaled to equal a.
###### Geometric Interpretation
In geometry, the ratio of two lengths ba​ describes their proportional relationship, which is fundamental in similarity and scaling transformations.
###### Probability
In probability theory, the ratio of favorable outcomes to possible outcomes defines the likelihood of an event occurring.

## Ratio in [[Dimensional Analysis|Dimensional Analysis]]
In Grigory Barenblatt's book "Scaling, Self-similarity, and Intermediate Asymptotics," a ratio in terms of dimensional analysis is typically viewed as a dimensionless quantity that characterizes the relative magnitudes of two quantities of the same dimension. Ratios play a critical role in scaling laws and similarity solutions because they allow for the comparison of different systems or phenomena in a normalized way.

### Key Concepts from Barenblatt’s Work:

1. **Dimensionless Numbers**:
    
    - A ratio in dimensional analysis often leads to the creation of dimensionless numbers, which are essential in understanding the scaling behavior of physical systems. Examples include Reynolds number, Froude number, and Mach number.
2. **Scaling Laws**:
    
    - Scaling laws involve relationships between dimensionless quantities. These laws reveal how different physical quantities scale with each other when the system's size or another relevant parameter changes.
3. **Self-Similarity**:
    
    - Self-similar solutions often depend on dimensionless ratios. Self-similarity implies that the shape of the solution does not change when rescaled by certain factors, which are expressed as ratios.
4. **Intermediate Asymptotics**:
    
    - In intermediate asymptotics, ratios of lengths, times, or other physical quantities are used to find similarity solutions that are valid in certain intermediate regimes of the physical problem.

### Practical Example from Barenblatt’s Work:

Consider the problem of fluid flow around a sphere. One important dimensionless ratio here is the Reynolds number (𝑅𝑒Re), which is the ratio of inertial forces to viscous forces in the fluid:

𝑅𝑒=𝜌𝑣𝐿𝜇Re=μρvL​

where:

- 𝜌ρ is the fluid density (dimension: [M L−3−3])
- 𝑣v is the velocity of the fluid (dimension: [L T−1−1])
- 𝐿L is the characteristic length (dimension: [L])
- 𝜇μ is the dynamic viscosity of the fluid (dimension: [M L−1−1 T−1−1])

By analyzing this ratio, one can determine the flow regime (laminar or turbulent) and predict the drag force on the sphere.

### Importance of Ratios in Dimensional Analysis:

1. **Normalization**:
    
    - Ratios normalize quantities, making it easier to compare systems of different scales.
2. **Similarity and Scaling**:
    
    - Ratios are fundamental in identifying similarity and scaling laws, which are used to generalize the behavior of physical systems.
3. **Reduction of Variables**:
    
    - Using dimensionless ratios reduces the number of variables in a problem, simplifying the analysis and leading to more general solutions.

In summary, according to Barenblatt, ratios in dimensional analysis serve as fundamental tools for creating dimensionless numbers, which are critical for understanding scaling laws, self-similarity, and the behavior of physical systems under various conditions. These concepts are extensively discussed in his work "Scaling, Self-similarity, and Intermediate Asymptotics."