---
up:
  - "[[Surfaces]]"
related:
  - "[[Surface Strategies]]"
  - "[[Gaussian Curvature]]"
  - "[[Mean Curvature]]"
  - "[[Curves]]"
  - "[[Surface Analysis]]"
  - "[[Surface Decomposition]]"
  - "[[Surface Creation]]"
  - "[[Nurbs Curves]]"
date created: 2024-03-20
---
# Notion of Surface Curvature
## The **curvature** of a surface at a point *P* **measures** how the **surface deviates** from the **tangent plane** at *P*.

### In order to **define the curvature** of a surface, the **osculating circle** needs to be defined.
following a similar process used to define the osculating circle for planar curves (*see* [[Curves#^01ae23|oscualting circles]]). 

- A 2D Osculating Circle:
![[Pasted image 20240323094731.png|400]]
- For each point *P* belonging to an arbitrary freeform surface, a **normal vector** *n* can be calculated. 
- An infinite number of **planes** called **sheaf of planes** (*pa, pb, ..., pi*) containing the normal vector *n* can found. I.e. planes where the normal vector is the axis of rotation that generates "infinite" sheaf of planes. 
	![[Pasted image 20240324151532.png|400]]
- Therefore, an infinite set of curves (*ca, cb, ..., ci*) can be found as the **intersection** between the planes and the surface. 
- For each curve (*ca, cb, ..., ci*), the **curvature** can be calculated **at *P*** as the **reciprocal of the radius of the osculating circle**, resulting in a set of **curvature values**: *ka, kb, ..., ki.*
	- There is a **unique osculating circle** for a **given curve** at **point *P***.
	- A **curve** with a **positive** **curvature value** has its **osculating circle** on the "positive side" of the generatrix- that is **"on"** the surface.
	- A **curve** with a **negative** **curvature value** has its **osculating circle** on the "negative side" of the generatrix- that is **"outside"** (or "under") the surface.
	![[Pasted image 20240324152110.png|600]]
- Within the **set of curvature values** (*ka, kb, ..., ki*) for Point *P* and within the sheaf of planes used to generate the set of curves, a **Minimum Principal Curvature *k<sub>1</sub>*** and a **Maximum Principal Curvature *k<sub>2</sub>*** can be found. 
## **Principal Curvatures**:
At any given point on a surface, the principal curvatures can be obtained by ***slicing* the surface with planes that contain the normal vector** to the surface at that point.
### The curve in which the **Minimal Principal** **curvature *k<sub>1</sub>*** is calculated: is called ***C<sub>1</sub>***
The **tangent vector** to curve ***C**<sub>1</sub>* at point *P* is called, the **Minimum Principal Curvature Direction $\vec{k_1}$**
- If ***C<sub>1</sub>*** is a **straight line**, then the ***k<sub>1</sub> = 0*** at that point *P*.
### The curve in which **Maximum Principal curvature *k<sub>2</sub>*** is calculated: is called ***C<sub>2</sub>*** 
The **tangent vector** to curve *C<sub>2</sub>* at point *P* is called, the **Maximum Principal Curvature Direction $\vec{k_2}$**
- If ***C<sub>2</sub>*** is a **straight line**, then the ***k<sub>2</sub> = 0*** at that point *P*.
![[Pasted image 20240324155441.png|500]]

#### The Min and Max Principal Curvatures are always perpendicular to each other:
- Imagine holding a curved, thin shell or a piece of paper that you can bend. At any point, you can bend it more steeply in one direction than in any other. 
- The direction where the bending is steepest and the direction where it's shallowest are naturally perpendicular to each other. 
- This is because bending in one direction does not influence the bending in the perpendicular direction due to the surface's local geometric properties.
#### Curvature value *k* for a curve *C*:
- The **larger** the radius, the **smaller** the curvature.
- ***Curvature value = 1 / radius***
- ***radius = 1 / curvature***
#### The two **primary methods** of defining curvature:
- **Gaussian Curvature** ([[Gaussian Curvature]])
	 - *G* =  *k<sub>1</sub>* *  *k<sub>2</sub>*
- **Mean Curvature** ([[Mean Curvature]])
	- =  (*k<sub>1</sub>* +  *k<sub>2</sub>*) / 2
- Both are significant to the theory of surfaces.
### **Generatrix aka Generator aka Generating Curve**:

^eb70ca

A component used in the **creation** of a complex surface or shape.
- Is **the curve** (or generator or generatrix) that **moves** or **rotates** or **sweeps** around the **guided path or curve** (i.e. the directrix) to **generate** a surface. 
- Therefore, the movement of the generator is in **relation** to the **directrix** and **together** they **define** **the form** of the the resulting surface.
- The generatrix adapts its position and orientation according to the directrix's path.
### **Directrix aka Path aka Guide Curve aka Rail aka Trajectory**:
- Is a **predefined path** or **curve** that **guides** the movement or generation of another shape (point, line, etc.) or curve to **generate** a surface or volumetric shape.
- Most commonly it guides the motion of the **generatrix**.
- Can have **multiple** directrices for a generatrix.
### How to identify the Generatrix and Directrix (intuitively)
Understand the Surface Type:
- [[Gaussian Curvature#Developable Surfaces|Developable]] Surfaces
- Ruled Surfaces
Use Geometric and Visual Cues:
- Parallelism and Convergence:
	- Observe any parallel lines or converging towards a point - generatrix.
- Surface Flow:
	- Observe the overall **flow** of the surface.
		- It can sometimes reveal the path of the directrix. 
			- For example: a surface that twists or spirals might indicate a helical directrix. 
#### **Ruled Surfaces**:
Are surfaces that are generated via **generatrix** that is a **straight line**. 
- Every point on a ruled surface can be found on a straight line that lies entirely on the surface.
- Not the same as Developable Surface, but there is commonality and overlap:
- **All Developable Surfaces** are Ruled Surfaces.
- But **not all Ruled Surfaces** are Developable Surfaces.
- A Ruled Surface is Developable when **unique tangent planes** can be **calculated along a ruling (i.e. straight generator)**.
	- I.e. the **twist angle** between tangents at rulings' end points is **null** (in this case a ruling is called a **torsal ruling**).
		- **Twist angle**: ^twist-angle
			- Refers to the angle between the tangents to a generatrix (a straight line that generates the surface) at its endpoints as it moves along one or two directrices (guiding curves). 
			- Essentially, it measures how much the orientation of the generatrix changes as it sweeps along the directrices to generate the surface.
		- **Torsal ruling**: 
			- Refers to a specific characteristic of a ruled surface where each ruling (generatrix) is a torsion-free geodesic. 
			- Torsion here describes the rate of change of the binormal vector to a curve with respect to its arc length, which for a straight line (and thus a torsion-free geodesic) is zero. 
			- A geodesic is the shortest path between two points on a surface; it's the curve of minimal curvature on that surface.
		- For example: 
			- To **create** a **developable** **ruled** **surface** starting from an arbitrary curve (*rail curve 1*), the **geometry** of the **second curve** (*rail curve 2*) is **dependent upon outputting a null twist angle**.
			![[Pasted image 20240325004241.png|400]]
		- To create a developable ruled surface starting from **two** arbitrary and **fixed rail curves**: it is not enough to divide both curves into equal parts and connect the resulting points though the "ruling" lines. As it is not guaranteed that the **twist angle** is **null** for each ruling. 
			- In this case, plugins (specific algorithms) must be implemented to **search for the developing ruling lines** which have **no twist**.
			![[Pasted image 20240325101537.png|400]]
		
### Principal Curvature component:
Calculates the Principal curvature for surfaces.
- Outputs:
	- C^1: Minimum Principal Curvature value.
	- C^2: Maximum Principal Curvature value.
	- K^1: Minimum Principal Curvature Direction.
	- K^2: Maximum Principal Curvature Direction.
	- F:
- **Surface Curvature** component:
- Calculates the Gaussian and Mean curvature for surfaces.
- Outputs:
	- G: Gaussian Curvature value.
	- M: Mean Curvature value.
![[Pasted image 20240325095531.png|500]]

##### Strategies:
[[Surface Strategies]]
