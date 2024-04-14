---
up:
  - "[[Surfaces]]"
related:
  - "[[Surface Strategies]]"
  - "[[Surface Creation]]"
  - "[[Surface Decomposition]]"
  - "[[Surface Analysis]]"
  - "[[Nurbs Curves]]"
  - "[[Notion of Surface Curvature]]"
  - "[[Mean Curvature]]"
  - "[[Gaussian Curvature]]"
  - "[[Curves]]"
date created: 2024-03-25
---
# Surface Strategies:
## Developable Test:
### Definition:
##### The method or algorithms used to **determine** whether a **given surface** is **deployable**.
### Approach: 
##### Developable **primitives** (*Planes, cylinders, cones, and surfaces obtained by bending a flat sheet without stretching it*) can be used to **isolate** developable **sub-surfaces**.
- I.e. Developable primitives are **used** as a **basis** for **comparison** or as tools **to isolate** **sections** of a **more complex surface** to **assess** their **developability**. 
	- *However, this method can **lead to false results** if the geometry is **not trimmed** from the a primitive.* 
		- If not trimmed or "modified to fit" precisely within the bounds of the primitive, it might retain characteristics of the primitive - those characteristics would suggest developability, even if the target surface geometry is not developable on its own.
- By **comparing** the **target surface's** sections against these **primitives**, one can **assess** whether those sections are **developable**.
	- If a sub-surface (i.e. section) of the target surface can be closely matched or approximated by a developable primitive, it suggests that the section itself is likely developable.
- **Example**:
	- A complex surface as a target surface with a section or sub-surface that is seemingly similar to a side of a cylinder. 
### How:
##### To **identify** developable surfaces:
- **Osculating Circles** component:
	- Can be used to draw the two osculating circles at a generic point *P* expressed in the Local Coordinate System. 
##### If the surface is **developable** then at least one of the osculating circles will be a **straight line** at every point on the surface. 	
- A **Line** component connected to the *C<sub>1</sub>* and *C<sub>2</sub>* outputs, will be in "**correct**" status if an osculating circle is a straight line.
	![[Pasted image 20240325174040.png|600]]
##### To **generalize** this **method**:
- **Generate a grid of points** as the *uv* input of the **Divide Surface** component.
	- Then calculate the **osculating circles** of the ouputs.
		- A **Line** component connected to the *C<sub>1</sub>* and *C<sub>2</sub>* outputs, will be in "**correct**" status if an osculating circle is a straight line. 
			![[Pasted image 20240326113257.png]]

### Example: Curvature Pattern
##### Mean Curvature analysis can be used to generate complex patterns on surfaces by using measured curvature to inform a pattern.
###### Consider a referenced surface in Rhino:
- To create the pattern:
	1.  The set surface is reparametrized.
	2. Then the set surfaces is divided into a **set** of *N* sub-surfaces using **Divide Domain$^2$** component and **Isotrim-SubSrf** components. 
	3. The **Evaluate Surface** component is used in conjunction with a **MD Slider** to create a point positioned approximately in the center of the surface (0.5,0.5).
- To generate the pattern of **circles**:
	- The **C-input** and the **N-input** of a **Circle CNR** component are connected to the **P-output** and **N-output** of the **Evaluate Surface**, respectively. 
		- **Circle CNR** component:
			- **Inputs**:
				- (C): Center point.
				- (N): Normal vector of circle plane.
				- (R): Radius of circle
		![[Pasted image 20240326231724.png]]
- To generate the "curvature pattern":
	- The **R-input** is set to be dependent on the **mean surface curvature**.
		- Mean Curvature is calculated by the **M-output** of the **Surface Curvature** component.
			- *Because Mean Curvature can be negative, the resulting list of values must be **passed through** an **Absolute** component to produce positive values.* 
	- A **Minimum** component is used to set a maximum value (0.150 in this example) to the Mean Curvature output (of the **Curvature** component).
		- This *minimized* Mean Curvature value is passed into the Radius Input of the **Circle CNR** component (replacing the **Number Slider** component).
	- Finally, a **Cull Pattern** component **filters** only the **circles larger than a specified value**, set in the **Function (F)** component of an **Evaluate Expression** component. 
		![[Pasted image 20240327074539.png|500]]
		![[Pasted image 20240326233143.png]]
		- A **Surface Split** component can be used to split the initial surface using the circles as **trimming curves**.
			- The split initial surface will be index element 0 in the **Surface Split** component **output list**. 
				- The remaining list elements (1 to N) are the "scrap surfaces" whose boundaries are the cutting curve.
					- The split initial surface can be viewed by using the **List Item** component, set to 0.
				![[Pasted image 20240326233452.png]]
			![[Pasted image 20240326233533.png|400]]

### Example: Hexagonal Pattern