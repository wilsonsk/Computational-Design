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
In order to **define the curvature** of a surface, the **osculating circle** needs to be defined.
following a similar process used to define the osculating circle for planar curves (*Not the same as* [[Curves#Hodograph|hodographs]]). 
## Oscillating Circles
![[Pasted image 20240323094731.png|400]]
*A 2D Osculating Circle*

The osculating circle is a geometric concept that provides the best local approximation to a curve at a given point.
	It is the circle that has the same tangent and curvature as the curve at that point. 
		The center of the osculating circle is called the [[#Center of Curvature|center of curvature]], and its radius is called the [[#Radius of Curvature|radius of curvature]].

It refers to the circle that "kisses" the curve at a point, having the same tangent and curvature as the curve at that point. It is used to describe the local curvature of the curve.
	I.e. Refers to the circle that matches the curve's tangent and curvature at a point.
	
## Oscillating Circle a [[Newton's Second Law#Velocity|Velocity]]
![[Pasted image 20240630084804.png]]

The Oscillating Circle represents the [[Components of Motion#Velocity Vector|velocity vector]] in velocity space.
The Oscillating Circle shows how the velocity vector changes over time.
The Oscillating Circle is plotted in a different space (velocity space) than the actual trajectory of the particle.

![[Pasted image 20240630084728.png|300]]
##### Diagram Components
###### Point $P$
A point on the curve where the osculating circle is being considered.
####### [[Components of Motion#2D Components of the Velocity Vector|Tangent Vector]] ($\vec{s}$)
The vector tangent to the curve at point PPP. 
	This is the direction of the velocity vector if the curve represents the trajectory of a particle.
		Points in the direction of motion and is tangent to the curve.
###### Normal Vector ($\vec{n}$)
The vector perpendicular to the tangent vector at point $P$, pointing towards the center of curvature $C$.
	It is a component of the [[Components of Motion#2D Components of the Acceleration Vector|Acceleration]].
###### Osculating Circle
The circle that best approximates the curve at point $P$. 
	It has the same tangent and curvature as the curve at this point.
###### Center of Curvature ($C$)
The center of the osculating circle.
###### Osculating Plane
The plane in which the osculating circle lies.

For each point *P* belonging to an arbitrary freeform surface, a **normal vector** *n* can be calculated. 

An infinite number of **planes** called **sheaf of planes** (*pa, pb, ..., pi*) containing the normal vector *n* can found. I.e. planes where the normal vector is the axis of rotation that generates "infinite" sheaf of planes. 
![[Pasted image 20240324151532.png|400]]

Therefore, an infinite set of curves (*ca, cb, ..., ci*) can be found as the **intersection** between the planes and the surface. 

For each curve (*ca, cb, ..., ci*), the **curvature** can be calculated **at *P*** as the **reciprocal of the radius of the osculating circle**, resulting in a set of **curvature values**: *ka, kb, ..., ki.*
![[Pasted image 20240324152110.png|600]]

There is a **unique osculating circle** for a **given curve** at **point *P***.

A **curve** with a **positive** **curvature value** has its **osculating circle** on the "positive side" of the generatrix- that is **"on"** the surface.

A **curve** with a **negative** **curvature value** has its **osculating circle** on the "negative side" of the generatrix- that is **"outside"** (or "under") the surface.

Within the **set of curvature values** (*ka, kb, ..., ki*) for Point *P* and within the sheaf of planes used to generate the set of curves, a **Minimum Principal Curvature *k<sub>1</sub>*** and a **Maximum Principal Curvature *k<sub>2</sub>*** can be found. 
## Center of Curvature
The center of curvature is a point that lies on the normal line to the curve at a given point, and it is at a distance equal to the radius of curvature. 
	For a circular path, this point is the center of the circle.

It refers to the point that is the center of the "osculating circle" (the circle that best approximates the curve) at a given point on the path.
## Radius of Curvature
#### $\LARGE r = \frac{|\vec{v}|^2}{|\vec{a}_{\perp}|}$

The radius of curvature is the radius of the osculating circle at a given point on the path. 
	It represents how sharply the path is curving at that point.

The radius of the osculating circle provides a measure of the curve's "tightness" at a given point. A smaller radius indicates a tighter curve.

It refers to the distance from the point on the curve to the center of curvature. It quantifies the curvature of the path at that point.
## Curvature $k$
Curvature is defined as $k\LARGE = \frac{1}{r}$​.
	This definition makes intuitive sense because as the radius of the osculating circle decreases (indicating a tighter curve), the curvature increases.
		I.e. The smaller the radius, the fraction increases, and thus curvature, $k$  increases.
## Principal Curvatures
At any given point on a surface, the principal curvatures can be obtained by ***slicing* the surface with planes that contain the normal vector** to the surface at that point.
### The curve in which the Minimal Principal **curvature *k<sub>1</sub>*** is calculated: is called ***C<sub>1</sub>***
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
#### The two primary methods of defining curvature:
- **Gaussian Curvature** ([[Gaussian Curvature]])
	 - *G* =  *k<sub>1</sub>* *  *k<sub>2</sub>*
- **Mean Curvature** ([[Mean Curvature]])
	- =  (*k<sub>1</sub>* +  *k<sub>2</sub>*) / 2
- Both are significant to the theory of surfaces.
### Generatrix aka Generator aka Generating Curve:

^eb70ca

A component used in the **creation** of a complex surface or shape.
- Is **the curve** (or generator or generatrix) that **moves** or **rotates** or **sweeps** around the **guided path or curve** (i.e. the directrix) to **generate** a surface. 
- Therefore, the movement of the generator is in **relation** to the **directrix** and **together** they **define** **the form** of the the resulting surface.
- The generatrix adapts its position and orientation according to the directrix's path.
### Directrix aka Path aka Guide Curve aka Rail aka Trajectory:
- Is a **predefined path** or **curve** that **guides** the movement or generation of another shape (point, line, etc.) or curve to **generate** a surface or volumetric shape.
- Most commonly it guides the motion of the **generatrix**.
- Can have **multiple** directrices for a generatrix.
##### Frame
- A frame, as used in Grasshopper and computational design, is a more general term that refers to any reference geometry or structure used to guide the generation of other geometries.
- Frames can be points, lines, curves, or even complex surfaces that act as constraints or boundaries within which other elements are generated.
- In the example of the [[Form-Finding Strategies Using Kangaroo#Catenary Curves and Particle-Spring Systems (i.e. PSS) Particle Spring Systems|catenary curves]], the frames are the freeform curves that define the start and end points of the catenaries, guiding their overall shape.

So, while a directrix can be considered a specific type of frame used for guiding the shape of curves or surfaces, the term "frame" in algorithmic modeling encompasses a broader range of guiding geometries beyond just directrices.
### How to identify the Generatrix and Directrix (intuitively)
The line segment or curve segment between an apex and a base (i.e. directrix) is the a generatrix. 

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
### Surface [[Continuities|Continuity]]
![[Pasted image 20240425135925.png]]
###### G0: Two surfaces are connected, but only their positions match at the connection point.
###### G1: Two surfaces are connected, and their positions and tangents match at the connection point.
###### G2: Two surfaces are connected, and their positions, tangents, and curvatures match at the connection point.

#### Mathematical Perspective
###### G0: The functions representing the curves are not equal at any particular point.
###### G1: The first derivatives of the functions are equal, meaning they have the same slope.
###### G2: The second derivatives are equal, indicating the same rate of curvature.

##### Strategies:
[[Surface Strategies]]
