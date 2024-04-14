---
up:
  - "[[Surfaces]]"
related:
  - "[[Notion of Surface Curvature]]"
  - "[[Surface Strategies]]"
  - "[[Surface Decomposition]]"
  - "[[Surface Analysis]]"
  - "[[Gaussian Curvature]]"
  - "[[Curves]]"
  - "[[Mean Curvature]]"
date created: 2024-03-25
---
# Surface Creation
^surface-creation
## Section Curve:
### A cross section curve that is formed when a 3D surface is cut through by a plane.
- Revealing the section curve shape at the intersection.
- I.e. Is the curve of **intersection** between a **surface** and a **plane**. 
	- The *plane* is really just an angle or direction of the *cut* on the surface. 

Are the "individual" curves across a surface
![[Pasted image 20240323153232.png]]

## Edge Curve:
Is a dependent curve type that **lies** on the **boundary** of a surface.

![[Pasted image 20240323154658.png|300]]

## Profile Curve aka [[Notion of Surface Curvature#**Generatrix aka Generator aka Generating Curve**|Generator]]:
Refers to a 2D curve that acts as a **blueprint** or outline for creating 3D shapes. It essentially **defines** the shape of a slice or cross-section that can be used to generate more complex forms. 
- Defines the shape to be translated.
## Sweep Curve/Rail/Path or Axis of Rotation (depending on context i.e. operation) aka [[Notion of Surface Curvature#**Directrix aka Path aka Guide Curve aka Rail aka Trajectory**|Directrix]]:
Is the path/rail or axis of rotation along which the profile curve is translated (translational sweep or rotation). 
- **Defines** the **edge surface**:
	- Which refers to a surface created between two or more curves (directrices) that serve as the **boundaries**.
Acting as a **guide** or **trajectory** that determines the overall form of the final object when a profile curve is translate or rotated along it. 
## Extrusion (aka Extrude Operation):
A **specific case** of **translational surface generation**.
- It requires a **profile curve** (open or closed) (i.e. [[Notion of Surface Curvature#**Generatrix aka Generator aka Generating Curve**|generator]]) or a surface, to extrude along a vector known as the **extrusion path** (i.e. [[Notion of Surface Curvature#**Directrix aka Path aka Guide Curve aka Rail aka Trajectory**|directrix]]). 
	- I.e. The **directrix** is **always** the **vector** (linear curve - *line*).
	- Where the profile curve is *moved* along a **linear** (i.e. straight path) **directrix**.
		- Often **perpendicular** to the **plane** of the **profile curve**.
			- ###### If not perpendicular to the plane of the profile curve:
				- That is, an directrix **at an angle** relative to the plane containing the profile curve:
					- Each cross section **remains oriented perpendicular (i.e. normal)** to the **directrix** (i.e. extrusion path).
						- This is a fundamental aspect of how extrusion works.
							- Each point on the profile curve moves along the directrix, creating a new "slice" or section of the shape that is oriented perpendicular to the direction of motion.
						- Although the path is angled relative to the original plane of the profile curve (i.e. not perpendicular to the plane of the profile curve):
							- The extrusion operations effectively "carries" the profile curve's orientation along the path.
					- The cross sections of the extruded shape will **remain constant** in terms of their shape relative to the original profile curve.
						- I.e. The cross section shapes will match the original profile curve throughout the length of the extrusion.
					- Only the **direction** in which the profile curve is projected is affected.
		- Therefore, the **orientation** of the **profile curve** remains **constant** relative to the **direction of extrusion**. 
			- Effectively creating a **uniform** **cross section** along the **entire length** of the extruded shape.
				- I.e. Extrusion yields a constant section, that is, the cross sectional shape does not change as you move it along the length of the directrix (i.e. the length of the extruded shape). ^18bb28
					- *For example: if you extrude a circle, **every cross section** of the resulting cylinder is always a circle of the **same size** as the original profile circle (9)curve)*. 
- The easiest way to create a surface.
## Translational (NURBS) Surface Generation:
Aka **Sweep (1 and 2) Operation** which **generates** a surface by **translating** (or sweeping) a NURBS curve (i.e. generator / profile curve (P)) **along a path** (i.e. directrix).
- The **generator** (i.e. the original, profile curve (S)) is moved along a **directrix** or two directrices (i.e. another curve(s) / sweep path(s) / rail(s)).
	- The **directrix** can be a **complex** path or **curve**. ^d14a44
		- ###### The key differences between Translational (NURBS) Surface Generation and Extrusions:
			![[Pasted image 20240404074802.png]] ![[Pasted image 20240404074744.png]]
			- **Directrix complexity**: ^a9c163
				- The extrusion path (i.e. directrix) can only be linear/straight.
				- The sweep path/rail (i.e. directrix) can be complex, that is, curved. 
			- **Orientation to the Profile Curve**:
				- The profile curve's orientation can change if the directrix is not linear, which affects the resulting surface.
			- **Resulting Geometry**:
				- The geometry resulting from extrusion is typically simpler and more predictable.
					- Contains sides that are parallel to the directrix (i.e. extrusion path).
					- The ends are the shape of the original profile curve.
	- The surface is formed by the "trail" it leaves in its motion. 
- This technique can produce complex shapes that are difficult to achieve through other means.
	![[Pasted image 20240323161851.png]]
	![[Pasted image 20240406140948.png]]
## Rotational (NURBS) Surface Generation:
Aka **Rotation Operation** which generates a surface by revolving a NURBS curve (i.e. generator / profile curve (P)) around an axis (i.e. directrix).
- In this case, the **directrix** is no longer a sweep rail/path, but is an **axis of rotation**. 
- The resulting surface is smooth.
- It can represent shapes like bottles, glasses, vases, or even complex fluted columns. 
	- Depending on the profile curve used.
	![[Pasted image 20240323161946.png]]
	![[Pasted image 20240406141005.png]]
## Boundary Surface:
Creates a trimmed or untrimmed **planar** surface from a collection of **boundary edges**.
- It Boundary surface requires **planar** and **continuous** **closed curves** to result in a surface.
	![[Pasted image 20240323161134.png]]
## Lofted (NURBS) Surface Generation:
Aka a Loft operation.
Creates a surface **through** a **set** of **ordered section curves**:
- Via **geometric interpolating or blending** the points between the set of curves. 
- Has a "starting profile curve" (i.e. a starting generator) and an "ending profile curve" (i.e. an ending generator).
- There is no defined directrix.
![[Pasted image 20240323161124.png]]
A Form-Generating Transformation:
Generates new forms or shapes from existing profiles or cross-sections..
The transformation here involves creating a continuous surface through the interpolation of shapes along a path, which alters the original shapes' spatial configuration to create a new unified object.

NURBS Surface from Lofting:
When the curves used for lofting are NURBS curves, the resulting surface is a NURBS surface. 

This is because the lofting operation inherits the mathematical properties of the NURBS curves, providing the ability to represent complex geometries smoothly and with a high degree of control over shape precision.
## Surface from points:
Creates a surface from a **grid** of points. 
- It is useful for creating surfaces **from other surface**.
- It is useful for creating surfaces **from mathematical functions**.
- **Inputs:**
	- (**P**): a set of points of a curve or grid.
	- (**U**): the number of points in the *u* direction.
		- example: if 9 points in (P) and number 6 in (U), then it creates a surface from a 9x6 grid. 
![[Pasted image 20240323161111.png|500]]
## Edge Surface:
Creates a surface from two, three or four curves. 
- **Interpolates** a surface from ordered edge curves. 
![[Pasted image 20240323161056.png|500]]
## Patch:
Fits a surface through a set of points, or curves that are open or closed. 
- Generates a series of perpendicular curves, **called spans**, from input curves which compose a trimmed or untrimmed surface. 
	- **Span curves** are rarely parallel to any edge of the output surface, therefore the Patch component is used when its *not* possible to perform other methods.
![[Pasted image 20240323160324.png]]

## Network Surface: 
Operates on **two sets** of ordered curves to create a single surface. 
- It requires curves in the *u* direction and in the *v* direction. 
- (**C**) input: specifies **type** of **surface continuity**  (0=Loose, 1=Position, 2=Tangency, 3=Curvature).
- Facilitates more **control** of edge surfaces in comparison to the Loft component.
![[Pasted image 20240323161031.png|600]]
