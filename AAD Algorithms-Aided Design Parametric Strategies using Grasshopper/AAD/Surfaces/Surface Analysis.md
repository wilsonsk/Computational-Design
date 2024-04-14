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
date created: 2024-03-25
---
# Surface Analysis:
Parametric Representation is used to find points on a surface
## Finding points on a surface:
### **Evaluate Surface** component:

![[Pasted image 20240324000017.png|500]]
- **Inputs**:
	- **(S)**: a surface to analyze.
	- **u and v coordinates** (LCS): are scalar values between 0-1.
- Therefore, remember to **reparametrize** your surface input or the **Evaluate surface** component itself. 
- **Outputs**:
	- **(P)**: a point expressed in WCS.
	- **(N)**: a normal vector at *P*.
	- **(F)**: a tangent plane at *P*.
	![[Pasted image 20240324000034.png|400]]

## World to Local Conversion:
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


## Extracting the Isocurves:
### Isocurve component:
- Extracts the isocurves of a surface at a specific point (P), given its local coordinates (uv).
- Isocurves U (parallel to the *u* direction) and isocurves V (parallel to the *v* direction) are extracted separately.
- The U or V isocurves can be visualized independently by connecting a curve component to the U or V output and hiding the Isocurve component. 
![[Pasted image 20240324002620.png|500]]

## Dividing a surface:
### Divide Surface component:
Generates a grid of points on a surface. 
- the Points (P) are the **intersection vertices** of a grid of **isocurves** calculated by dividing the *u* and *v* axes **evenly** by a positive integer.
- Outputs:
	- (**P**): Set/grid of points on the **input** surface.
	- **(N):** Normal vectors at points (P).
	- **uv**: The local coordinates of those output points.

## Splitting a surface:
#### Isotrim-SubSrf component:
*Is actually an Isotrim **operation** consisting of a **Divide Domain$^2$** fed into a **Subsrf** component.* ^isotrim-subsrf-operation

Splits a surface into a **set** of **contiguous sub-surfaces** based on a grid of splitting isocurves.
	![[Pasted image 20240324003657.png|500]]

- The **SubSrf** component is used in **conjunction** with the **Divide Domain^2** component. 
	-   **Divide Domain$^2$** component:
		- Used to segment or subdivide a 2D domain (area) into smaller, **equally sized** subdomains (sub areas), according to specified parameters.
		- **Defines** the **number of divisions** in both *u* and *v* directions.
		- Generates an **even** **cutting-grid** on the surface for the **SubSrf** component to work with. 
		![[Pasted image 20240324003930.png|500]]
	- **Outputs**:
		- (**S**): a **set** of **untrimmed** surfaces **parametrized** according to the **domain** of the **parent-surface**. 
			- Notice that the **parent Srf** component is **reparametrized**, therefore the sub-surfaces have the **same reparametrized domain** as the parent- that is if or until the sub-surface itself is reparametrized. 
- ##### To be parametrized according to their parent domains:^parametrized-according-to-the-parent-surface
	- **The domain of a parent surface**:
		- Is the **range** of U and V parameters that define the entire area of that surface. 
			- This domain is like a grid that covers the surface, where any point on the surface can be located by a U,V coordinate within this domain.
		- **When a new subsurface** is created via  the Isotrim operation:
			- It is said to be "parametrized according to their parent domains,"
				- It means the subsurface’s definition is derived from a specific subset of the parent surface's U and V domain.
				- Essentially, you are defining a new, smaller surface within the confines of the larger original surface by specifying a new domain within the original’s domain. 
				- The subsurface is thus a portion of the parent surface, redefined and scaled according to the specified subdomain.
	- **Relative to the Parent Domain**: 
		- The subsurface's 0 to 1 domain corresponds to a specific portion of the parent surface's domain. 
			- For example, if the subsurface represents the middle quarter of the parent surface, the subsurface's 0 to 1 domain maps to 0.25 to 0.75 of the parent surface's domain.
		- **Reparametrization**: 
			- This is essentially a reparametrization process.
				- Even though the subsurface has its own 0 to 1 domain, this domain is a scaled version of a specific portion of the parent surface's domain. 
				- The operation scales the chosen subdomain of the parent surface to a new full 0 to 1 domain for the subsurface.

	-  **For example**: the **domain** of the identified sub-surface is [0;0.1] in the *u* direction and [0;0.2] in the *v* direction: 
		- When the sub-surface is extracted out of the parent, the [0.1;0.2] is the domain of that sub-surface- **parametrized corresponding** to according to its parent surface.
		- If that sub-surface is **reparametrized**: then its domain (min and max) are **remapped** to 0 and 1, where 0.1 in the U = 1 and the 0.2 in the V = 1.
			![[Pasted image 20240324004146.png|400]]	
			![[Pasted image 20240324004318.png|400]]
- Each sub-surface can be **parametrized** between 0-1 via the **reparametrize** option of the component. 
- **Isotrim and Domain**: 
	- When you use Isotrim with a surface, you're essentially **specifying** a new **domain** **within** the **existing** U and V domains of the **parent** **surface**. 
	- Isotrim then creates sub-surfaces based on these specified subdomains. 
	- Because the operation is **defined parametrically** through **domains** rather than geometric cutting, the resulting sub-surfaces **are inherently untrimmed**. 
		- They are new, complete surfaces within their own right, defined within the parameter space of the original surface.
- **Parent Surface Parametrization Influence**: 
	- The untrimmed subsurfaces maintain a parametric relationship with the parent surface because they are defined directly from the parent's domain. 
	- This means their geometry is a direct, unaltered extrapolation of parts of the original surface, with their own parameters scaled relative to the specific subsection of the parent's domain they represent.

**Uneven Splitting**:
Divide Domain^2 creates an evenly spaced grid because the component **divides the *u* and *v* axes evenly**.
To generate **unevenly** spaced grids, the distribution of the points along *u* and *v* must be adjusted.
- **Deconstruct Domain^2**:
	- **Divides** the **bi-dimensional** **domain** into its **mono-dimensional** **components** U and V. 
- **Graph Mapper** component:
	- Changes the distribution of points within the two separate domains U and V. 
- **Construct Domain^2**:
	- Reassembles the mono-dimensional domains back into a bi-dimensional domain.
- **Isotrim** component:
	- The surface is then split based on the newly adjusted U and V domains now expressed as a *uv* domain.  
		![[Pasted image 20240324101006.png|500]]
