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
	The division of a by b, seeks to determine the factor by which b must be scaled to obtain a. 
		This operation answers the question: "How many units of b are there in a?"
#### Abstract Interpretation
###### Distribution 
Division distributes the total quantity a into equal parts of size b. 
	*For example*, if a represents a collection and b the size of each subset, division tells us how many such subsets can be formed.
###### Measurement
Division measures the quantity a using the unit b. 
	If b is a standard unit, division indicates how many times this unit fits into a.

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