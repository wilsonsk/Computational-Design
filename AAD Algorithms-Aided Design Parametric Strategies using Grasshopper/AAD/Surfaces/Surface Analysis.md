---
up:
  - "[[Surfaces]]"
related:
  - "[[Notion of Surface Curvature]]"
  - "[[Surface Strategies]]"
  - "[[Mean Curvature]]"
  - "[[Gaussian Curvature]]"
  - "[[Curves]]"
  - "[[Surface Decomposition]]"
  - "[[Surface Creation]]"
  - "[[SubD Surface Patterns]]"
  - "[[Grids]]"
date created: 2024-03-25
---
# Surface Analysis:
Parametric Representation is used to find points on a surface
## Finding points on a surface:
### **Evaluate Surface** component:
Extract a **single point** on a given surface with a given *uv* coordinate.
- I.e. Evaluate local surface properties at a single given *uv* coordinate.

![[Pasted image 20240324000017.png|500]]
- **Inputs**:
	- **(S)**: A surface to analyze.
	- **u and v coordinates** (LCS): Are scalar values between 0-1.
		- Therefore, remember to **reparametrize** your surface input or the **Evaluate surface** component itself. 
- **Outputs**:
	- **(P)**: A point expressed in WCS.
	- **(N)**: A normal vector at *P*.
	- **(F)**: A tangent plane at *P*.
	![[Pasted image 20240324000034.png|400]]
## [[Nurbs Curves#World Coordinate System (WCS)|World]] to [[Surfaces#Local Coordinate System|local]] Conversion:
### Surface CP: 
**Surface Closest Point**
Can be used to **convert** a point *P* on a surface expressed in the WCS to a point expressed in the LCS.
- **More specifically** it finds the closest point *P'* on a surface, given an external point *P*. 
	- The **displacement distance** between points *P'* and *P* is output by **(D)**.
	- But when the component is used to convert between WCS and LCS, then *P'=P* and *D=0*.
- **Inputs**:
	- (P): Sample point.
	- (S): Base surface
- **Outputs**:
	- (P): Closest point of surface to the sample point.
	- (uvP): *uv* coordinates of the closest point.
	- (D): Distance between the sample point and the closest point on the surface.
	![[Pasted image 20240324000636.png|500]]
## Extracting the [[Surfaces#Isocurves/Isoparametric Curves|Isocurves]] (i.e. the curves):
### Iso
Refers to isoparametric curves on a surface, indicating that the trimming or segmentation is based on constant parameter values of either *u* or *v* on the surface.
### Isocurve component:
**Extracts** (i.e. outputs) the **isocurves** of a surface at a specific point (P), given its local coordinates (*u, v*).
- Isocurves U (parallel to the *u* direction) and isocurves V (parallel to the *v* direction) are extracted separately.
- The U or V isocurves can be visualized independently by connecting a curve component to the U or V output and hiding the Isocurve component. 
- **Inputs**:
	- (S): Base surface.
	- (uv): *uv* coordinate on surface for isocurve extraction.
- **Outputs**:
	- (U): Isocurves in the *u* direction.
	- (V): Isocurves in the *v* direction.
![[Pasted image 20240324002620.png|500]]
#### How the Isocurve Component is Used to Analyze a Surface
##### 1. Parametric Structure
Isocurves reveal the underlying parametric grid of a surface. 

By examining isocurves, users can understand how the surface is defined in its parametric *u* and *v* space. 

This is particularly useful for evaluating how modifications to the surface parameters will affect the overall shape and flow of the geometry.
##### 2. Continuity and Smoothness
Isocurves provide visual cues about the continuity and smoothness of a surface. Continuous and smooth isocurves typically indicate a well-defined surface with good continuity properties. Abrupt changes or kinks in isocurves might suggest issues with surface continuity or unwanted sharp transitions, which are crucial for both aesthetic and functional aspects of design.
##### 3. Curvature
The distribution and curvature of isocurves help in assessing the surface's curvature. Tightly packed isocurves can indicate areas of high curvature, while widely spaced isocurves suggest flatter areas. Understanding the curvature through isocurves is essential for applications that require precise control over surface properties, such as in aerodynamic design or in creating ergonomic products.
##### 4. Surface Deformations
Any irregularities or deformations in the surface can often be detected through anomalies or distortions in the isocurves. This is useful for quality control in product manufacturing, ensuring that the surfaces are correctly modeled and manufactured without unintended deformations.
##### 5. Texturing and Material Application
In digital modeling and rendering, isocurves help in applying materials or textures. By aligning textures with isocurves, one can achieve more natural-looking results where the texture follows the logical structure of the surface. This alignment is crucial for realistic rendering in visualizations and animations.
##### 6. Tool Path Generation
For manufacturing processes, especially in CNC machining or 3D printing, isocurves can guide the creation of tool paths. Ensuring that tool paths align with isocurves can lead to more efficient material removal and better surface finish, particularly on complex geometrical shapes.
## Dividing a Surface into Points:
### Divide Surface component:
Generates a grid or **set of *uv* points** on a given surface with given **number of *uv* segments**. 
- The Points (P) are the **intersection vertices** of a grid of **isocurves** calculated by dividing the *u* and *v* axes **evenly** by a positive integer.
- **Inputs**:
	- (S): Surface to divide.
	- (U): Number of segments in the *u* direction.
	- (V): Number of segments in the *v* direction.
- **Outputs**:
	- (**P**): Set/grid of points on the **input** surface.
	- **(N):** Normal vectors at points (P).
	- **uv**: The local coordinates of those output points.
![[Pasted image 20240414091434.png]]
## Splitting a surface into Sub-Surfaces:
Is an operation consisting of a **Divide Domain$^2$** components (S) output, fed into a **Subsrf** component's (D) input. ^isotrim-subsrf-operation

The **SubSrf** component is used in **conjunction** with the **Divide Domain^2** component. 
![[Pasted image 20240324003930.png|500]]
Splits a surface into a **set** of **contiguous sub-surfaces** based on a grid of splitting **isocurves**.
![[Pasted image 20240324003657.png|500]]
#### Divide Domain$^2$ component:
Extracts (i.e. outputs) **subdomains** (segmented or subdivided domain) from a given 2D domain.
	- Segments/Subdivides a given domain (area) into smaller, **equally sized** subdomains (sub areas), according to specified parameters.
- **Defines** the **number of divisions** in both *u* and *v* directions.
- Generates an **even** **cutting-grid** on the surface for the **SubSrf** component to work with. 
- **Inputs**:
	- (I): Base Domain.
	- (U): Number of segments in the *u* direction.
	- (V): Number of segments in the *v* direction.
- **Outputs**:
	- (S): Individual segments.

In the context of "Splitting a surface", it is used to define sub-domains upon a surface from when sub-surfaces can be "**[[Surfaces#Trimmed Surface|trimmed]]**".
	**Subdomains**: 
		- A list of smaller two-dimensional domains. Each subdomain is defined by a pair of intervals, each specifying the bounds in the u and v dimensions. These subdomains are systematic partitions of the original domain, organized in a grid that corresponds to the specified number of divisions in u and v directions.
		- These subdomains are useful for further operations where you might need to apply transformations, generate geometry, or perform evaluations separately within each segmented area of a larger domain. For instance, if applied to a surface, these subdomains can dictate where specific features or panels are placed, allowing for a controlled and parametric approach to design variations.
	**Each subdomain** [[#To be Parametrized According to Their Parent Domains|corresponds to a specific portion of the domain]], defined by its own range of *u* and *v* parameters.
#### Isotrim aka SubSrf Component
Trims/Extract an isoparametric subset (i.e. set of sub-surfaces) of a surface.
- I.e. Outputs a set of untrimmed sub-surfaces that are [[#To be Parametrized According to Their Parent Domains|parametrized according to the parent-surface]].
	**Iso**: 
		Refers to isoparametric curves on a surface, indicating that the trimming or segmentation is based on constant parameter values of either *u* or *v* on the surface.
			Which the component uses to define the **boundaries** of the **sub-surfaces** it **trims**.
				The input domain specifies the start and end points along the *u* and *v* directions, which correspond to isocurves on the surface. 
					Isotrim effectively trims the surface along these isocurves, isolating a portion (i.e. Sub-surface) of the surface bounded by them.
	**Trim**: 
		Refers too the act of cutting or segmenting the surface within these defined isoparametric bounds.
	**Sub**: 
		Indicates a subset or a smaller part derived from something larger.
	**Srf**: 
		Stands for surface, indicating the component deals with surface geometry.
- **Inputs**:
	- (S): Base surface.
	- (D): Domain of subset.
- **Outputs**:
	- (**S**): a **set** of **untrimmed** surfaces **parametrized** [[#To be Parametrized According to Their Parent Domains|according to the domain of the parent-surface]]. 
		- Notice that the **parent Srf** component is **reparametrized**, therefore the sub-surfaces have the **same reparametrized domain** as the parent- that is if or until the sub-surface itself is reparametrized. 
##### Isotrim and Domain: 
When you use Isotrim with a surface, you're essentially **specifying** a new **domain** **within** the **existing** U and V domains of the **parent** **surface**. 
- Isotrim then creates sub-surfaces based on these specified subdomains. 

Because the operation is **defined parametrically** through **domains** rather than geometric cutting, the resulting sub-surfaces **are inherently untrimmed**. 
- They are new, complete surfaces within their own right, defined within the parameter space of the original surface.
###### Parent Surface Parametrization Influence: 
The **untrimmed sub-surfaces** maintain a parametric relationship with the parent surface because they are defined directly from the parent's domain. 
- This means their geometry is a direct, unaltered extrapolation of parts of the original surface, with their own parameters scaled relative to the specific subsection of the parent's domain they represent.
###### To be Parametrized According to Their Parent Domains:
**The domain of a parent surface**:
- Is the **range** of U and V parameters that define the entire area of that surface. 
	- This domain is like a grid that covers the surface, where any point on the surface can be located by a U,V coordinate within this domain.

	**When a new subsurface** is created via  the **Isotrim** operation:
		- It is said to be "parametrized according to their parent domains,"
			- It means the subsurface’s definition is derived from a specific subset of the parent surface's U and V domain.
			- Essentially, you are defining a new, smaller surface within the confines of the larger original surface by specifying a new domain within the original’s domain. 
			- The subsurface is thus a portion of the parent surface, redefined and scaled according to the specified subdomain.

	**Relative to the Parent Domain**: 
	- The sub-surface's 0 to 1 domain corresponds to a specific portion of the parent surface's domain. 
		- For example, if the subsurface represents the middle quarter of the parent surface, the sub-surface's 0 to 1 domain maps to 0.25 to 0.75 of the parent surface's domain.

	**Reparameterization**: 
		- This is essentially a reparameterization process.
			- Even though the subsurface has its own 0 to 1 domain, this domain is a scaled version of a specific portion of the parent surface's domain. 
			- The operation scales the chosen subdomain of the parent surface to a new full 0 to 1 domain for the subsurface.

	***Parent Parametrization Example***: 
		The **domain** of the identified sub-surface is [0;0.1] in the *u* direction and [0;0.2] in the *v* direction: 
		- When the sub-surface is extracted out of the parent, the [0.1;0.2] is the domain of that sub-surface- **parametrized corresponding** to according to its parent surface.
		- If that sub-surface is **reparametrized**: then its domain (min and max) are **remapped** to 0 and 1, where 0.1 in the U = 1 and the 0.2 in the V = 1.
			![[Pasted image 20240324004146.png|400]]	
			![[Pasted image 20240324004318.png|400]]
		- Each sub-surface can be **parametrized** between 0-1 via the **reparametrize** option of the component. 
### Uneven Splitting:
Divide Domain$^2$ creates an evenly spaced grid because the component **divides the *u* and *v* axes evenly**.
To generate **unevenly** spaced grids, the distribution of the points along *u* and *v* must be adjusted.
- **Deconstruct Domain$^2$**:
	- **Divides** the **bi-dimensional** **domain** into its **mono-dimensional** **components** U and V. 
- **Graph Mapper** component:
	- Changes the distribution of points within the two separate domains U and V. 
- **Construct Domain$^2$**:
	- Reassembles the mono-dimensional domains back into a bi-dimensional domain.
- **Isotrim** component:
	- The surface is then split based on the newly adjusted U and V domains now expressed as a *uv* domain.  
		![[Pasted image 20240324101006.png|500]]
