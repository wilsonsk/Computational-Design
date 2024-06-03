# Dimensional Analysis
Dimensional analysis is a mathematical technique used in physics and engineering to analyze the relationships between different physical quantities by considering their dimensions (such as length, mass, time, etc.).
	This method helps to simplify complex physical problems, check the consistency of equations, derive relationships between variables, and convert units.

We call “dimensional analysis” the process of working out the dimensions of a quantity in terms of the base [[Data/Abstract Mathematical Spaces/Physics/Basic Concepts/Measurement#Dimensions|dimensions]] and a model prediction for that quantity. 

A few simple rules allow us to easily work out the dimensions of a derived quantity. 
	Suppose that we have two quantities, X and Y, both with dimensions. 
		We then have the following rules to find the dimension of a quantity that depends on X and Y:

###### Addition/Subtraction
You can only add or subtract two quantities if they have the same dimension: [X+Y]=[X]=[Y][𝑋+𝑌]
###### Multiplication
The dimension of the product, [XY][𝑋𝑌], is the product of the dimensions: [XY]=[X]⋅[Y][𝑋𝑌]
###### Division
The dimension of the ratio, [X/Y][𝑋/𝑌], is the ratio of the dimensions: [X/Y]=[X]/[Y]
#### Dimensions and Units
Every physical quantity can be expressed in terms of basic dimensions such as length (L), mass (M), time (T), electric current (I), temperature (Θ), amount of substance (N), and luminous intensity (J). Units are the standard quantities used to measure these dimensions, such as meters for length, kilograms for mass, and seconds for time.
#### Dimensional Homogeneity
An equation describing a physical phenomenon is dimensionally homogeneous if all terms in the equation have the same dimensions. This is a fundamental requirement for the equation to be physically meaningful.
#### Dimensional Consistency
Ensuring dimensional consistency involves verifying that the dimensions on both sides of an equation match. This helps in identifying errors in derivations or formulations of equations.
## Method of Applying Dimensional Analysis
Dimensional analysis can be applied through the following steps:

1. **Identify the Relevant Variables**: List all the physical quantities involved in the problem. Identify the dimensions of each variable in terms of the basic dimensions (L, M, T, etc.).
    
2. **Express the Dimensions**: Write the dimensions of each variable using the notation [Variable] = L^a M^b T^c, where a, b, and c are the powers corresponding to the dimensions of length, mass, and time, respectively.
    
3. **Formulate the Dimensional Equation**: Combine the dimensions of the variables to form a dimensional equation. Ensure that the dimensions on both sides of the equation match.
    
4. **Derive Dimensionless Groups (if applicable)**: Use the Buckingham π theorem to derive dimensionless groups. This theorem states that if you have a physical problem with n variables and k fundamental dimensions, you can form (n - k) independent dimensionless groups (π groups).
    
5. **Solve the Problem**: Use the dimensionless groups or the dimensional equation to solve the problem. This might involve deriving relationships between the variables, simplifying equations, or checking the consistency of derived formulas.

## Example 1
Acceleration has SI units of ms−2 and force has the dimension of mass multiplied by acceleration. What are the dimensions and SI units of force, expressed in terms of the base dimensions and units?

###### Solution

We can start by expressing the dimension of acceleration, since we know from its SI units that it must have the dimension of length over time squared.

[acceleration]=LT2[𝑎𝑐𝑐𝑒𝑙𝑒𝑟𝑎𝑡𝑖𝑜𝑛]=𝐿𝑇2

Since force has the dimension of mass times acceleration, we have:

[force]=[mass]⋅[acceleration]=MLT2[𝑓𝑜𝑟𝑐𝑒]=[𝑚𝑎𝑠𝑠]⋅[𝑎𝑐𝑐𝑒𝑙𝑒𝑟𝑎𝑡𝑖𝑜𝑛]=𝑀𝐿𝑇2

and the SI units of force are thus:

SI[force]=kg⋅m/s2𝑆𝐼[𝑓𝑜𝑟𝑐𝑒]=𝑘𝑔⋅𝑚/𝑠2

Force is such a common dimension that it, like many other derived dimensions, has its own derived SI unit, the Newton [N][𝑁].

## Abstract Interpretation of Dimensions as Ratios
In dimensional analysis, dimensions are typically expressed in terms of fundamental quantities such as length (L), mass (M), time (T), and others. 
	When these dimensions are considered as ratios, it means that we are comparing different quantities that have the same or different fundamental units.

#### Abstract Definition
In the context of dimensional analysis, when dimensions are ratios, they provide a way to compare and understand different physical quantities in relation to one another. This approach uses fundamental units to construct dimensionless quantities or relative measures, revealing the underlying structure and relationships within physical systems.

This abstraction is crucial for both theoretical insights and practical applications, allowing for the development of scaling laws, predictions of system behavior, and a deeper understanding of the fundamental principles governing physical phenomena.
#### Basic Concept
- **Dimensionless Quantities**: A dimensionless quantity is a ratio of two quantities with the same dimensions, resulting in a pure number. For example, the ratio of two lengths 𝐿1𝐿2L2​L1​​ or the ratio of two masses 𝑀1𝑀2M2​M1​​.
- **Relative Dimensions**: When dimensions are expressed as ratios, they often represent relative measures. For example, speed is the ratio of length to time 𝐿𝑇TL​, and density is the ratio of mass to volume 𝑀𝐿3L3M​.
### Examples of Dimensions as Ratios
#### Speed
- **Definition**: Speed is defined as the ratio of distance traveled to the time taken.
- **Dimensional Form**: [𝑣]=𝐿𝑇[v]=TL​, where 𝑣v is speed, 𝐿L is length, and 𝑇T is time.
- **Interpretation**: This dimension indicates how much distance is covered per unit of time, making it a ratio that describes motion.
#### Density
- **Definition**: Density is the ratio of mass to volume.
- **Dimensional Form**: [𝜌]=𝑀𝐿3[ρ]=L3M​, where 𝜌ρ is density, 𝑀M is mass, and 𝐿3L3 is volume.
- **Interpretation**: This dimension provides a measure of how much mass is contained in a given volume, illustrating a ratio that describes material compactness.

#### Frequency
- **Definition**: Frequency is the number of occurrences of a repeating event per unit time.
- **Dimensional Form**: [𝑓]=1𝑇[f]=T1​, where 𝑓f is frequency and 𝑇T is time.
- **Interpretation**: This dimension indicates how often an event occurs within a specified time period, showing a temporal ratio.
### Practical Applications
#### Scaling Laws
- **Example**: The Buckingham π theorem is a key result in dimensional analysis that uses dimensionless ratios to derive scaling laws for physical systems.
- **Application**: By analyzing the ratios of different dimensions, engineers can predict how changing one aspect of a system will affect others, such as how altering the size of a model affects its behavior under similar conditions.
#### Fluid Mechanics
- **Reynolds Number**: A dimensionless ratio that compares inertial forces to viscous forces in fluid flow, given by 𝑅𝑒=𝜌𝑣𝐿𝜇Re=μρvL​, where 𝜌ρ is density, 𝑣v is velocity, 𝐿L is characteristic length, and 𝜇μ is dynamic viscosity.
- **Interpretation**: The Reynolds number helps predict flow patterns in different fluid flow situations, illustrating how the ratio of these dimensions determines the flow regime.
