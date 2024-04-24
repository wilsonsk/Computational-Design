---
up:
  - "[[Transformations]]"
related:
  - "[[Vectors]]"
  - "[[Data Relationships]]"
  - "[[Points]]"
  - "[[Parameters]]"
  - "[[Numbers]]"
  - "[[Curves]]"
  - "[[Surfaces]]"
date created: 2024-03-27
---
# Euclidean Transformations
Include translations, rotation, orientation, and mirror components.

## [[Elemental Building Blocks#Transformations Measures the change between two Points points *P(x,y)* and *P'(x',y')* Transformations of Points as the Fundamental Operation of Generation of Form|Generative Point]] Transformations:
These involve taking a point and applying a series of transformations based on some geometric rule or algebraic function, effectively **generating a curve**. 

This could be as simple as rotating a point around a fixed point at varying distances or moving a point along one line (the directrix) while controlling its motion via another rule or line (the generator).

## Translations: 

^a338b9

A type of transformation that **MOVES** **every point** in a figure or space by the **same distance** in a **specified direction**.
### Move Component:
Translates a geometric entity (G) according to a vector (T). 
- If (F) of the **Unit Z component** is connected with **multiple** numeric **values**, it will return multiple vectors. 
	- These vectors can be used to perform **multiple translations**.
		![[Pasted image 20240328001949.png|400]]
## Rotations:
The **motion** of a rigid body around:
-  a **fixed** point (i.e. rotation center).
-  a straight line (i.e. rotation axis).
### Rotate component:
Rotates a geometric entity (G) in a **plane**.
* I.e. rotating a geometry relative to its original **position** on an arbitrary **oriented plane/surface**.
* **Inputs**:
		- (G) The geometry to be rotated.
		- (A): Angle of rotation (in radians).
		- (P): Plane of rotation.
	![[Pasted image 20240328122045.png|500]]
		- *In this example*: 
			- The lower face of the geometry is extracted.
			- Then the approximated center point of that face is used to derive a normal vector 
			- That vector is then used to generate a plane normal to that vector.
			- Finally that plane is used as the relative plane of rotation.

**Plane Normal** component:
- Returns a plane that is **normal** (i.e. perpendicular) to a given **vector**.
	- **Input**:
		- (O): Origin of plane (i.e. a point).
		- (Z): Z-Axis direction of plane (i.e. a vector). 
### Rotate Axis component:
Rotates a geometric entity about an axis. 
- **Inputs**:
	- (G): The geometry to be rotated.
	- (A): Angle of rotation (in radians).
	- (X): Rotation axis (i.e. a **line**).
- **Outputs**:
	- (G): The rotated geometry.
	- (X): The transformation data.
- The axis can be defined by and **SDL Line** component that uses the specified point and normal vector of an evaluated surface.
	-  The line produced is fed into the (X) axis input of the **Rotate Axis** component.
		![[Pasted image 20240328123147.png|500]]
- A number list generating component can be used to produce multiple numbers that can represent and be used as multiple inputs of surfaces to create **progressive rotations**. 
	- *In this example*:
		- **Progressive** *moves* of the geometry are generated.
		- **Progressive** *angles of rotation* are generated. 
		- Utilizes **one** constant **axis** of rotation.
			- That being the *volume* center of the geometry in the *z* direction.
		- **Remember**: 
			- **Data lacing N:N**.
				- The number of incremental **volumes** **must equal** number of incremental **angles** of rotations.
					- I.e. The number of objects to rotate must equal the number of rotations.
			- **Volume component**:
				- Solves volume properties for closed Breps and meshes.
					- **Inputs**:
						- (G): Geometry (i.e. closed Brep or mesh) for volume computation.
					- **Outputs**:
						- (V): Volume of the geometry.
						- (C): Volume centroid of of the geometry.
			![[Pasted image 20240328123554.png|500]]
			![[Pasted image 20240328124407.png||200]]
		- **Calculating** the incremental **rotations** (i.e. the *relative angle* between consecutive geometries):
			- **Relative Angle**: ^relative-angle
				- Averages the *twist* across the entire **transformation** of the **generatrix**.
					- I.e. Gives a measure of **how much** the **generatrix** has *twisted* from the start to end of the **directrix**.
				- **Calculating** the Relative Angle: 
$$
\begin{align}
Relative \: Angle = Angle \: Value \: of \: First \: and \: Last \: Tangent \: to \: Generatrix \:
/
\: (Total \: Number \: of \: Geometries \: - \: 1)
\end{align} 
$$
					- Is a **function** of the **[[Notion of Surface Curvature#^twist-angle|twist angle]]**.
						- Where the the **geometry** is the **generatrix** and the **axis** is the **directrix**.
						- The twist angle being the change in orientation of the generatrix from its starting position to its end position.
						- Each incremental of the geometry can be viewed as a segment of the overall surface. 
					- The **angle value** between the **tangents** to the **start** and **end** positions of the **generatrix**.
						- Gives a measure of **how much** the **generatrix** has *twisted* from the start to end of the **directrix**.
							- Therefore, to calculate this relative value or **average** value, it is necessary to **extract** the **angle value** of the **tangent to** the **generatrix** of the first and last position.
								- Then by dividing by the total number of geometries minus 2, it produces:
									- An **average angle of twist per increment of the generatrix** (i.e. each incremental geometry).
					- *In this example:
						- The **equation** for **relative angle** is expressed as the combination of subtraction and division components.
							- They are then input in as the number of steps for the **Series** component.
								- The output is used as the **angle** input of the **Rotate Axis** component.*
						![[Pasted image 20240328153720.png|500]]
						
						![[Pasted image 20240328130005.png]]
						*Above is comparison of varying **twist angles***.

### Orient component
**Combines** **translations** and **rotations** into a **single transformation**.
- A geometric entity (G) arbitrarily oriented in space, can be oriented to a new position (G').
	- **Inputs**:
		- (G): A geometric entity.
		- (A): Source (i.e. Initial plane).
		- (B): Target (i.e. transformed plane).
	- **Outputs**:
		- (G): Reoriented geometry.
		- (X): Transform data.
- An **Evaluate Surface** component is used:
	- To **extract** an initial plane (i.e. source plane) via the **tangent plane (F) output** at a specified LCS point.
- An **XY Plane** component is used: 
	- To **describe** a target plane (final/transformed plane).
![[Pasted image 20240328165723.png|400]]

- The **Orient** component can also be used to **orient** a **list** of arbitrarily located **ribs-surfaces** to the XY plane. 
	![[Pasted image 20240328170251.png|500]]
	- The **Evaluate Surface** component is used to define a **source plane** derived from a referenced surface. 
		- A **series** component generates list of 12 numbers dividing the entire length of the referenced surface.
			- A **target plane** is derived from the **points** that move according to this list.  