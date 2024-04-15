---
up:
  - "[[Data]]"
related:
  - "[[Data Operations]]"
  - "[[Data Control]]"
  - "[[Numbers]]"
  - "[[Elemental Building Blocks]]"
date created: 2024-03-20
---
# Data Relationships
## Ratios
A relationship can be defined as a ratio of two quantities. 
	Quantifies how a change in one quantity affects the other quantity, or how quantities compare.
		- I.e. How two quantities relate to each other in scale, intensity or magnitude. 
			- This relationship can help in analyzing patterns.
But more broadly a ratio conveys a relationship, that is how things are connected or behave in respect to each other. 

## "In principle any conceivable network of relations between a given set of element attributes can be constructed".
-P. Schumacher, The Autopoiesis of Architecture, A New Framework fo r Architecture, Cohn Wiley & Sons, 2010), vol. I, p. 353.

##### Mathematics and logic are the basis of complex 3D models.
##### Data relationships are about **defining** **how** data elements **interact** with each other within the design system.

##### Data relationships can be seen as the **static** rules or **equations** that **describe** the **connections** between **parameters**.

##### Data relationships provide the **structure** or **framework** of the design, establishing the rules of interaction.

##### Data relationships are defined by equations involving numbers. 

##### Elemental Building Blocks are defined by the relationships of their parameters:
## Definition and Role: 
Data relationships define how pieces of data are connected or associated with each other. 

They describe the dependencies between different data elements, such as how one parameter might influence another or how changes in one aspect of a design affect other aspects. 

These relationships are often articulated through mathematical equations or logical rules.
## Examples: 
An example of a data relationship is the equation that relates the radius of a circle to its circumference (𝐶=2𝜋𝑟C=2πr). 

In a parametric design context, if the radius of a cylindrical column is adjusted, a data relationship would automatically update the column's surface area or volume based on predefined mathematical formulas.

Euler Polyhedra Formula:
	*F + V = E + 2*
	(F): Faces.
	(V): Vertices.
	(E): Edges.
*The **Deconstruct Brep** component outputs each of these variables based on a input Brep.*
## Purpose: 
The primary purpose of establishing data relationships is to capture the inherent or desired connections between different aspects of a design.

This allows for a coherent and integrated approach to design where changes propagate through the system in a predictable and controlled manner.

## Graphical Representation of Relationships:
Each point, line, curve, surface, or volume in computational is a representation of relationships between parameters. 

A [[Curves#Lines and "Graphs"|line]] being a representation of a relationship between two variables. 
	In a broader sense, every geometric transformation in a parametric model symbolizes a set of underlying equations or constraints that describe how the design behaves or changes with varying parameters.
## Connections, Dependencies: (i.e. Correlations): 
Data Relationships represent the **structures** that **define** the **associations** between [[numbers]] (i.e. numerical values). 
## **Functions**: (i.e. **mappings**)
Data Relationships are usually represented or defined by functions.
##### Functions: **Map input parameters** **to outputs**
###### Can range from:
- Linear mappings
- Complex non linear functions
- Conditional logic
###### Each defining different outcomes based on specific constraints or conditions.
- Numerical constraints can include:
	- Bounding possible values parameters can be (domain and codomains)
		- For Example: A function of **one** variable has a **domain** of values in the **x axis** and a **codomain** of values in the **y axis**, meaning for each input value (x) the function provides an output value (y).
	- Logical criteria

These functional mappings are essential for translating design intentions into computational models that can be explored and optimized. 
##### Evaluate F(x) component:
- **(F) input**: A function (relationship) between some other inputs (data).
- **(x) input**: Single or list of values for the x variable of the function.
- **(y) input**: Single or list of values for the y variable of the function.
- **(r) output**: The **codomain** of the function (set of all **possible** values of the equation).
## Conditions:
Determine a flow of data dependent on logical criteria
##### Evaluate F(x) component:
- Can be used to **define** **conditions**
	- **(F) input**: A **condition** that can include an arbitrary number of **variables** (x, y, ... inputs).
		- **Conditions:** Are defined using variables and logical comparison operators (=, <, >, ...).
	- **Logical Operators/Boolean Values**: 
		- Determine if a condition is satisfied.
			- Return "True" or "False" values.
	- Can be used in unison with **Cull Patterns**:
		- For example: Can **cull** all "*true*" values, etc.
	- **Dispatch Component**: Can be used to **filter** data with a corresponding Boolean values list. 
		- Returns 2 Lists:
			- **List A**: Contains data which returned *True*, i.e. met the conditional statement.
			- **List B**: Contains data which returned *False* i.e. did not meet the conditional statement.
	- **Concatenate**: Can be used to **join** 2 or more multiple fragments of text.
		- In the context of conditional statements, Concatenate can be used to "write" a "parametric" condition by concatenating the text of a conditional statement concatenated with a dynamic value.
	- **If/Then:** Can be used as (F) inputs
		- Syntax: if (x>5, y, "something")
			- "If x>5": is the conditional statement.
			-  ,y,"something": The values returned if condition is not met.
	- **Contains**: Tests whether the string *p* is in the list of data, *s*
		- Syntax: Contains(s, "p")
			- "s": is the list of data to be examined.
			- "p": is the string which is determined to exist or not exist within *s*.
		- Can also be used to **find specific geometries within a list**
			- **Panel**: Must be used as a "bridge" between *Geometry* and the *x input* of the Evaluate Component.
				- Syntax: Contains(x, "line"):
					- x: Is the input containing the data to be examined.
					- "line": Is the type of geometry to identify or not within the x input
				- The text or description within the panel is the data under examination which determines the outcome of the conditional statement.
##### Remap Numbers component: 
Evaluates a list of numbers ranging from A to B and **resizes** them **proportionally** to a new numeric domain A to B. Can be used to "reparametrize" a number system.
- I.e. Remap numbers into a new numeric domain.
	**Inputs**:
		- (V): The list to be remapped.
		- (S): A source domain
			- Can be **identified**/codified using the **Bounds** component attached to a number list generating component (series, etc.).
		- (T): a target domain
			- Is **defined** via the **Construct Domain** component
	- It is also used to perform **distance-based transformations** utilizing **attractors**.
	- **Outputs**:
		- (R): Remapped number.
		- (C): Remapped and clipped number.
##### Attractor: 
A geometric entity (point, curve or other element) used to modify the geometry around it within the defined limits. 
- The **impact** an **attractor** has on other geometry **depends** on the **distance** **between** the defined **attractor** and the **object** it is **manipulating**.
- The **remapped** domain is used as the **scaling factors**:
	- **Scale** component:
		- Scales geometry **(G) input** according to **(C) input**, a center of scaling, and **(F) input**, a scaling factor.
		- As the attractor point position moves, the respective distances change and the scaling correspondingly updates.
		- **Boundary** component: creates planar surfaces from closed curves. 
		- **Gradient** component: can be used to display the respective scaling factors graphically by via a color gradient.
	- General attractor point sketch:
		- Get centroids of grid geometry via area component
		- Get distance of centroid relative to an attractor point
		- Get bounds of that distance list as the source domain
		- Create a target domain (0-1)
		- Input both into a remap component
		- Scale grid geometry 
			- (G): Moved geometry
			- (C) Input (i.e. center of scaling): centroids of grid geometry (from area component)
			- (F) Input (scaling factor): remapped domain of distances of grid geometry relative to the attractor point.
		- Input scaled geometry into a boundary component
	- Can also use a curve as an attractor via a **Curve Closest Point** component. I.e., swapping out the *distance component* for the *curve closest point component*.
		- Which measures the distance (D) between each of the grid geometry's centroids relative to the closest point on the curve (i.e. the perpendicular angle of centroid point to curve)
	- **Main Idea:** The **remap component** can be used to influence/effect (move, scale, etc.) the relative geometry. 
		- For Example: Inputting remapped domain into a vector along the z axis and then moving the relative points...
	- To **Limit** the **effect** of an attractor:
		- The distance Between the point and centroids can be **divided by an arbitrary number**
			- Which becomes the **operating range** of the **attractor**.
		- **Minimum** component: Can be used to test whether a list of numbers are larger than a comparison number (**B**)
			- Values that satisfy the component are replaced with the minimum value (B).
			- So within the attractor context, the dividend of a distance is input into the **minimum** component as alternative to the remap component