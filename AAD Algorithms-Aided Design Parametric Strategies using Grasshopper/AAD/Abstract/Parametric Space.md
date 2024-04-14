---
up:
  - "[[Abstract Concept]]"
related:
  - "[[Geometric Space]]"
  - "[[Grids]]"
  - "[[Elemental Building Blocks]]"
  - "[[Parameters]]"
  - "[[Points]]"
  - "[[Curves]]"
  - "[[Number Systems]]"
  - "[[Data Relationships]]"
  - "[[2D Parametric Equations]]"
  - "[[3D Parametric Equations]]"
  - "[[Surfaces]]"
date created: 2024-04-07
---
# Parametric Space
Refers to an [[Abstract Concept|abstract]], mathematical space in which the shapes of geometry are described through [[Parameters|parameters]].
- The domain of parameters (*t* for curves, *u* and *v* for surfaces).
	- Used to define the geometry within that space.
- Is inherently a [[Surfaces#Local Coordinate System|local space]] (i.e. local coordinate system).
	- It defines the geometry relative to its own dimensions.
		- Which are not necessarily aligned with the Global Coordinate System.

## A conceptual environment :
- Were positions are defined by parameters, not by absolute coordinates.
	- As a way to **abstract the description of geometry**.
	- NURBS surfaces and curves are defined in parameters space.
	- Prior to being mapped to the 3D Cartesian coordinate systems.
		- This space is often referred to in terms o:
			- *uv* parameters for surfaces.
			- *t* parameter for curves.
	- Geometry is defined through [[Parametric Equations]].
	- That use one or more variables (i.e. parameters) to define the position along a curve or surface.
	- Is often defined by a domain.
	- Which is the bounds for a range of values that parameters can *take* (i.e. represent).

## Design Implications:
- Facilitates indirect geometric manipulation via parameter adjustments rather than through direct point manipulation in  space.
	- Enables high level of control.
- Enable Control points of curves and surfaces.
	- That utilize a "weighted" system of adjustment.
		- Allowing for smooth and continuous surfaces.
- Enable [[Surfaces#Isocurves/Isoparametric Curves|isoparametric curves]] 
- Facilitate *uv* mapping:
	- The process of projecting a 2D image onto a 3D model's surface.
		- Where the *u* and *v* correspond to the axes in the 2D texture space. 

## Relationship with the Local Coordinate System:
- The parametric space can be thought of as having its **own local coordinate system**.
	- Where parameters determine positions on a curve or surface.
- When geometry is created parametrically within a local coordinate system:
	- The parameters correspond to **locations** relative to that system.