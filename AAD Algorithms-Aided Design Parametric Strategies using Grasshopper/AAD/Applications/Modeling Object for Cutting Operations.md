---
up:
  - "[[Digital Fabrication]]"
related:
  - "[[Printable Objects]]"
date created: 2024-04-24
---
# Modeling Object for Cutting Operations
Objects that are unable to be manufactured by means of [[Digital Fabrication#Additive Techniques|additive processes]] can be fabricated using [[Digital Fabrication#(2D) Bi-dimensional Cutting|cutting (i.e. subtractive processes)]] based operations.
## Sectioning
Refers to contouring (contour/section lines) a model in one direction, typically parallel to a chosen axis.
It is a common technique used to build complex shapes by defining planar [[Gaussian Curvature#Developable Surfaces|developable surfaces]].
![[Pasted image 20240424230003.png|600]]
*For example*: A freeform **surface** can be **sliced** into **a set of parallel and planar sections based on an interval equal to the thickness of the material** to be [[Digital Fabrication#CNC Milling machines|milled]].
	Upon gluing the **sections** together in sequence, the original surface can be approximated.
If the same surface was milled from a single block of material, it the [[Digital Fabrication#Undercutting|undercuts]] would require the use of 3D milling machines. 
### Continuity Parallel to Section Planes
Sectioning creates [[Continuities|Continuity (i.e. when curves join)|continuity]] (i.e. the smoothness or seamlessness of the surface along and across the sections) parallel to the cut section and .

In the direction parallel to the section planes (i.e. along the face of each slice), the continuity is more straightforward to maintain.
	As each section represents a "snapshot" of the profile of the object at that specific slice. 
	When these slices are aligned and [[Digital Fabrication#Assemblies|assembled]], the continuity along the plane of each section can be visually and physically coherent because the adjacent edges of each section directly correspond to each other. 
### Limited Continuity in the Normal Direction of the Section Planes 
It is actually impossible to get continuity in the direction normal (i.e. perpendicular) to the section-planes.
This is because this relatively perpendicular direction cuts across the natural continuity of the original surface.  
Each section plane is essentially discrete, isolated along the slicing axis. 
	There is no material continuity between these slices.
		They are separate pieces of the same material or different materials entirely. 

A common fabrication technique is to leave a space between each section to create the illusion of continuity in the normal direction. 
	By allowing the viewer’s eye to fill in the gaps, especially if viewed from a distance or certain angles.
![[Pasted image 20240424230133.png|600]]
![[Pasted image 20240424232407.png|600]]