---
up:
  - "[[Points]]"
related:
  - "[[Nurbs Curves]]"
  - "[[Bezier Curves]]"
  - "[[Surfaces]]"
  - "[[Notion of Surface Curvature]]"
  - "[[Gaussian Curvature]]"
  - "[[Mean Curvature]]"
  - "[[Grids]]"
  - "[[Elemental Building Blocks]]"
  - "[[Surface Decomposition]]"
date created: 2024-03-20
---
# Curves
Curves are exemplary parametric objects
Understanding how they work gives insight into both the form-making possibilities of curves and into parametric modeling in general.
## Lines and "Graphs"
A line is an ordered set of points in between two bounding points.
A line expresses the [[Data Relationships#Ratios|ratio]] of directly proportional changes between two variables.
- I.e. A "straight" line is a **linear** [[Data Relationships#Graphical Representation of Relationships|relationship]] between two variables (typically represented in a Cartesian coordinate system as $x$ and $y$).
	- Linear: 
		- Meaning **direct proportion** between two variables (i.e. quantities).
			- Where a change in one variable (i.e. quantities) results in a change in the other variable at a constant rate. 
				- I.e. constant rate of change- graphed as a straight line.
![[Pasted image 20240414205341.png|300]]

A "graphic" representation of a line is a mark connecting two points, and defining all the points in between the bounding points (i.e. the "start" and "end" points).

*For example:* A [[Derivatives#^1f0a97|tangent line]]  or a **"slope"** is the **rate of change**, is a ratio, that is a linear relationship.
	The "vertical" change between any two points along a line, divided by the corresponding horizontal change. 
## Curves
A line is an ordered set of points in between two bounding points.
A curve expresses the [[Data Relationships#Ratios|ratio]] between two variables.
- But a curve is a **non-linear** relationship between two variables.
	- Non-linear:
		- Meaning a variable rate of change, where a change in one variable (i.e. quantity) does not necessarily result in a directly proportional change in the other variable (i.e. quantity).
*For example*: 
- **Quadratic Curves**: Represented by equations like $y=ax2+bx+c$ where $a≠0$. The graph is a parabola, which does not maintain a constant slope.
- **Exponential Curves**: Functions like $y=e^x$ or $y=ax$ (where $a>0$) exhibit exponential growth or decay, drastically different from linear growth.
- **Circular and Elliptical Curves**: Described by equations involving both $x$ and $y$ terms, such as $x^2+y^2=r^2$ for a circle, representing a completely different kind of relationship involving squaring of terms.
![[Pasted image 20240414205435.png]]
## Free Form Curves: 
Facilitate the expression of polynomial curves (that is constrained, relational numbers- polynomial expressions).

Curves can be described by a specifying a set of points objects or points that form an **abstract** representation of a curve. 

An algorithm then computes the curves from these objects. 
	For example a **circle** can be described as a **center**, a **radius** and a **plane** to the which the circle is **parallel**. 
## Conic sections:
- Are circles, parabolas, hyperbolas, and ellipses are described by polynomial equations of maximum degree 2. 
	- Are easy to construct and can be **joined** without obvious **kinks** (i.e. first order continuity), **but**
		- **Cannot achieve** higher smoothness (**smooth connections**)
## Interpolation vs. Approximation:
#### Interpolation: 
Curve algorithms that interpolate, **compute** curves that **go through** the **input points**.

In the context of computational design and geometry, interpolation is a mathematical and computational technique used to estimate or construct new data points within the range of a discrete set of known data points. It's a fundamental concept in creating smooth transitions between known values, such as points, lines, and surfaces, in both 2D and 3D modeling environments. Here’s how it is commonly applied:

1. **Point Interpolation**: If you have two known points, interpolation allows you to find intermediate points that lie on the straight line segment connecting these two points. This basic form of interpolation is linear and straightforward.
    
2. **Curve Interpolation**: This involves estimating points on a curve given a set of discrete points that the curve must pass through. The aim is to construct a smooth path that flows through or near these points. Common methods of curve interpolation include:
    
    - **Polynomial Interpolation**: Fitting a polynomial curve that passes exactly through all given points.
    - **Spline Interpolation**: Using piecewise polynomials called splines that pass through the points, typically ensuring smoothness at the joins (continuity in the first and possibly second derivatives). Bézier curves and B-splines are popular spline techniques used in graphic design and CAD software.
3. **Surface Interpolation**: Extending the concept to three dimensions, surface interpolation involves creating a surface that passes through or approximates a set of given points in 3D space. Techniques often used include:
    
    - **Bilinear and Bicubic Interpolation**: Extending linear and cubic interpolation into two dimensions, useful for textures and image processing within 3D modeling tools.
    - **NURBS (Non-Uniform Rational B-Splines)**: A mathematical model providing great flexibility and precision in describing both standard analytical shapes (like cones) and complex free-form shapes.
4. **Mesh Interpolation**: In more complex models like those used in finite element analysis (FEA) or complex 3D animations, interpolation between mesh points allows for the simulation of deformations and other effects based on physics.
##### Approximate: 
Curves algorithms that approximate, **place** curves "near" the **input points**. 
- Generally the most dominant mode. 
	- The reason being, they tend to be geometrically more **predictable** and "well-behaved", and are mathematically more **simple**. 
##### Input Points: 
Are the **control points** and the (possible open) polygon the control points define is the curve's ***control polygon*.**
- **Control Polygon:**
	- Is defined by the straight lines between consecutive control points.
##### Linear Interpolation == *tweening* 
The **fundamental constructor** for many kinds of curves utilizes the concept of *linear interpolation* or *tweening*. 
- Abstractly interpolation moves a value **within** a set of other values.
	- **Linear** interpolation moves this values *smoothly* and in **constant proportion**. ^linear-interpolation
## Parametric Motion of a Point: 
In its simplest form, [[Euclidean Transformations#Elemental Building Blocks Transformations Measures the change between two Points points *P(x,y)* and *P'(x',y')* Transformations of Points as the Fundamental Operation of Generation of Form Generative Point Transformations|transforming a point]] into a curve can be thought of as the trace of a point's path as it moves according to some rule or function. 

This is often described using parametric equations where $x$ and $y$ coordinates of the point are functions of a parameter $t$. 
	For example, the motion of a point in a circle might be described by $x(t)=rcos(t)$ and $y(t)=rsin(t)$, where $r$ is the radius of the circle and $t$ varies from 0 to $2π$.
### Parametric curves:
Are generated by linearly interpolating a parameter (i.e. moving a value within a set of other values) in an equation to produce the points on the curve.
- **Parametric lines**: the point and the parameter have a **direct** relationship 
	- ==**Equal increments** between **parameter values** produce corresponding **equal increments** between the **points** on the line.== 
- In contrast, in **curves** this relationship between increments of parameter values and increments of points is **indirect**. 
	- ==**Equal increments** between **parameter values** produce corresponding **UNEQUAL increments** between the **points** on the line.== 
		- This behavior has a **massive** implication on the form making process.
### **Parametric Curve Representation**:
Like parametric lines, parametric curves are defined by a point that moves with a **parameter, t**. 

Unlike lines, the movement is **not linear**
- The distance or intervals between one curve is not the same as another curve. The number of equal divisions of varying lengths of a curve themselves vary between curves. 
	- This is where uniform scaling/normalization/reparameterization come into play. As by rescaling a curves length to 0-1, the number of divisions can be equated between curves.
- **Geometric spaces** and **parametric spaces** are **different**.
	- See Parametric Representation of curves in [[Nurbs Curves#^65f47a|Parametric Representation]]
## Relating Curves to Objects:
In design, curves form relationships with other objects, and complex relationships are composed of simpler relationships. 

### Two basic relationships are defined by vectors:
#### 1. Tangent vectors
![[Pasted image 20240321003446.png|300]]
Almost every point p(t) on a curve has a family of vectors tangent to it. The sole exception is when the *first derivative* (from calculus) is not defined or is the zero vector.
- Of the infinitely many vectors tangent at a **parametric point** only **one** is *the* **tangent vector**. 
	- The reason is that the **length** of the tangent vector captures the **rate** at which *p(t)* **moves** along the curve as *t* changes. 
		- Therefore, the **lengths** of tangent vectors **vary** along the curve. 
	- The relative geometric distances (increments) between points along a curve, approximate the relative tangent vector lengths. 
		- When successive points are *close together*, the tangent vectors are correspondingly short. 
	
	- **Normalizing** the tangent vector gives the **unit tangent vector**.
#### 2. Normal vectors
 ![[Pasted image 20240321003419.png|300]]
In **2D space** a curve *almost* every **point** always has a **unique** direction vector **normal** (i.e. perpendicular) to the curve. 
- **Two** vectors, *pointing* (i.e. direction) to "to/away" from each side of the curve
- We *pick* the direction that *points* **into the curve.**
	- **It lies in the PLANE of the curve**
- In **3D** space, it is a more complicated situation.
	- A point on the curve and its tangent vector define a **plane** normal to the curve at that **point**.
	- **Every** vector **in this plane** is normal to the curve.
		- **However** there is a **specific vector** in that plane- the **normal vector** of the curve at *p(t)*.
			- It is a **unit of length** and it lies in the **osculating plane** of the curve at *p(t)*.
			- ![[Pasted image 20240323094815.png]]
			- Lying in this plane is the **osculating circle** which is the circle that is both tangent to and has the same curvature as the curve at *p(t)*.
				- The **radius** of the osculating circle is the **normal vector** of *P*. 
				- The **center point** of the osculating circles at each point along the curve define another curve called the **evolute**. ^osculating-circle
			- ![[Pasted image 20240323094731.png|300]]
###### Binormal Vector:
- Is the **cross product** of the **unit tangent vector** and the **normal vector**.
###### Frenet Frame:
- The **unit tangent vector**, **normal vector**, and the **binormal vector** can be **combined** into a structure that (with few exceptions) provides a sensible **coordinate** system at every point on the curve.
	- Each representing the x, y and z axix of the frame.
		- **unit tangent vector** = x axis
		- **normal vector** = y axis
		- **binormal vector** = z axis
- Is an **orthonormal frame** defined at (almost) every point on a 3D curve.
###### Inflection Point:
- The point of inflection or **flex**, is the point on a smooth curve where the curvature changes **sign**.
	- I.e. it's a point where the function changes from **concave** to **convex** or vice versa.
- The **problem** with frenet frames lies in their inflection points.
	- at a singular inflection points, Frenet frames are not defined. 
	- Inflection points rarely occur in 3D curves, instead **High Torsion** becomes something to deal with.
		- **High Torsion** is when a point crosses an inflection point, the Frenet frame seems to invert, instantaneously rotating or "twisting" 180 degrees around the **tangent vector**.
			- i.e. A curve that comes close to an inflection condition results in its Frenet frame **rapidly rotating around** the curve.
		- **The Solution**
			- Create a **reference direction** that not dependent on the local context of the point *p(t)* on the curve. 
			- Then place a frame on the curve:
				- With its **x vector** set to be the x vector of the Frenet frame.
				- Its **z vector** at **right angles** to the x vector
				- And its **z vector** **co-planar** with the x vector and the reference vector. 
###### Hodograph:
- Is a curve defined by the ends of the tangent vectors
- It is the **first derivation** of the curve.
	- The hodograph of the hodograph is the **second derivation**. ^01ae23
## [[Bezier Curves]] 
### Splines:
Is a **composite curves** composed of relating parts.
- **Problematic example**: Bezier curves **joined** together to make splines.
	- Reason for problems: despite simple geometry and math, the control is only **pseudo-local** and the order of a Bezier curve is the number of points in the control polygon.
#### Pseudo-local control
Meaning that **all points in a curve** **change** when **any** control point is **changed**.
- **Monomial**: a component element of a polynomial. A product of constants and variables raised to exponents that are positive integers. 
	- ex. 3x^2
- **Polynomials an Monomials** have **2 descriptors**:
	- **Degree (d):** the maximum (highest) exponent value in the polynomial.
	- **Order (n):** n= degree + 1
- Bezier curves take their order and thus degree from the number of **vertices** in the **control polygon**.
	- ex. an order 4 Bezier curve has a four-point control polygon, and order 3 Bezier curve has a three-point control polygon, etc.
- **Therefore**: The link between order and control points means that a complex design must be done with high-order curves and this creates problems in interactive editing:
	- it is easy to introduce local bumps and hard to make a curve visually fair.
	- the curve may also lie far from the control polygon, making it hard to predict how an editing action might affect the curve
##### SOLUTION:
- **All** of these problems can be addressed and **remedied** by **connecting a series of curves** into a **composite curve** - a **SPLINE CURVE**
	- Unfortunately, Bezier curves do not spline gracefully.
##### B-Splines: basically just a **framework** for **constructing** Bezier curves
Defined **ON** a control polygon.
- Are easily splined and thus address all the problems of Bezier curves. 
- So easily splined that often no distinction is made between a curve (one spline segment) and a spline (multiple segments).
The only **constraint** on the **order** of the curve is that it **must be less than or equal to the number of points in the control polygon**.
Provide **two new modeling controls** to the control points:
##### knots:
-Independent specification of order:
- Are essentially just a new way to specify a Bezier control polygon that, in turn, defines the intended curve. 

Curves have **one more control**: **WEIGHTS**, which are introduced in the step from B-Splines to Non Uniform Rational B-Splines ([[Nurbs Curves]]) 
