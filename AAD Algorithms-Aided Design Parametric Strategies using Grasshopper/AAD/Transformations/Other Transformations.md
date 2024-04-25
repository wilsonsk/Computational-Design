---
up:
  - "[[Transformations]]"
related:
  - "[[Curves]]"
  - "[[Surfaces]]"
  - "[[Vectors]]"
  - "[[Data Relationships]]"
  - "[[Points]]"
  - "[[Data Control]]"
  - "[[Numbers]]"
  - "[[Parameters]]"
date created: 2024-03-29
---
# Other Transformations

## Box Morph Transformation
### Box Morph component
Uses a reference "pliable" box to deform geometry to a target box.
**Inputs**:
- (G): Geometry to morph.
	- The geometry can consist of a set of geometric entities to morph. 
		- In the case of enclosing an entire set of geometries:
			- The **Bounding Box** component must be to *Union Box* mode via contextual menu. ^953bd4
- (R): A reference box, which encompasses the geometry to morph.
	- Can be defined by the **Bounding Box** component.
- (T): A target box. 
	- Can be created using Grasshopper box-components.
Works by **mapping** the geometric relationship between the reference box and the target box.
- The original geometry, which fits within the reference box, is then transformed according to this map.
- The **transformation** **adapts the geometry to fit within the target box**, preserving the relative proportions and orientations as defined by the relationship between the reference and target boxes. 
- **Pliable**: Meaning the dimensions and orientations (of a geometry) are used as a flexible reference framework, not that the geometry itself physically changes or deforms. 
- I.e.:
	- It transforms the reference box (R) into the target box (T), modifying the contained geometry (G). 
		![[Pasted image 20240330015557.png|500]]
#### Bounding Box component:
Used to create a box that tightly encloses a given geometry or set of geometries.
- Represents the smallest volume capable of containing the entire input geometry.
	- Aligned with the WCS or specific coordinate system.
		- Its primary purpose is to provide a simple, rectilinear volume that summarizes the spatial extent of the complex shapes.
			- Making it easier to perform various spatial, organization or analytical operations.
Solves oriented geometry bounding boxes.
- Inputs:
	- (C): Geometry to contain.
	- (P): Orientation plane of bounding box.
- Outputs:
	- (B): Aligned bounding box in WCS.
	- (B): Bounding box in orientation plane coordinates.
		
Multiple geometries can also be simultaneously morphed to primitive or non-primitive boxes.
- To morph multiple objects, the **Bounding Box** component must be set to *Union Box mode* via contextual menu.
##### *Example*: Target geometry is a Twisted Box:
###### **Twisted Box** component

- The bounding points can be defined in Grasshopper or set in Rhino. 
	- In this example geometries are referenced from Rhino.
		- **Bounding Box** component is set to *[[#^953bd4|Union Box mode]]* in order to enclose all the geometries. 
			- The Target geometry was creating by setting eight points (drawn in Rhino) using the local setting.
				- If these points are adjusted, the geometry will deform accordingly.
	![[Pasted image 20240409132732.png|500]]

### Paneling
**Extends** the **Box Morph** logic to **multiple target boxes**.
- Given an arbitrary surface with a set of twisted **target** boxes, a surface-panelization can be defined using a single or a set of merged geometries. 
	![[Pasted image 20240409131448.png]]
- Consists of two steps:
	1. Creating a set of (twisted boxes) target boxes (T) on an arbitrary freeform surface.
		- The **Surface Box** component generates twisted boxes on a surface with a defined bi-dimensional [[Domain|domain]] (D) and a (H) height. 
			- ###### Surface Box component:
				- Create a twisted box on a surface patch.
					- Inputs:
						- (S): Base surface.
						- (D): Surface domain (i.e. the "patch" on the surface containing twisted boxes).
						- (H): Height of surface box.
					- Outputs:
						- (B): Resulting surface twisted box.
	1. Morphing a geometry (G) that is encompassed by a reference box, to a target box. 
	![[Pasted image 20240409131431.png]]

	- *Example*:
	- A grid of 20 x 20 surface boxes.
		- As specified by the bi-dimensional domain.
			- With a height of 0.5 units are created on the surface using the **Surface Box** component. 
				- The Surface Boxes are the Target Boxes for morphing.
		![[Pasted image 20240409131638.png]]
		- Morphing **manipulates** the base geometry to match the target geometry (surface boxes in this case).
			- Creating **panels**.
		![[Pasted image 20240409131804.png]]
		- If random values are assigned to the (H) input of the **Surface Box** component:
			- Different heights are assigned to the target boxes.
		![[Pasted image 20240409131529.png]]