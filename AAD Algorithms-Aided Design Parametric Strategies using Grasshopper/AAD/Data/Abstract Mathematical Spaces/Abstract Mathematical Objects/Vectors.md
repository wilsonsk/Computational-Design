---
up:
  - "[[Analysis]]"
related:
  - "[[2D Parametric Equations]]"
  - "[[3D Parametric Equations]]"
  - "[[Parameters]]"
  - "[[Numbers]]"
  - "[[Data Relationships]]"
  - "[[Elemental Building Blocks]]"
date created: 2024-03-27
---
# Vectors 

## Components
Used to **create** and **modify** vectors.

### Vector 2Pt component:
Creates a vector between two described points:
- Inputs:
	1. (A): Start point.
	2. (B): End point.
	- (U): [[Unitize]] output (Boolean).
- Outputs:
	- (V): The produced vector.
	- (L): *Length* i.e. quantity/magnitude. 
- **Vector Display** component can be used to display the vector.
### Unit Vector component:
Can be used to **unitize** the vector or **change** the **magnitude** to **1** **unit**, without modifying the direction.
	- Given a vector with a specified **direction** and **magnitude** (L) described by **two points**.
		![[Pasted image 20240327230412.png]]
### Amplitude component:
Sets the magnitude (i.e. length as described by Grasshopper) of a given vector to an input value (A).
	- I.e. Modifies the magnitude of a given vector to a specified value. 
		- Outputting a new vector with the modified magnitude. 
		- Maintains original direction and sense.
			- However, sense will change when inputting a negative (A) value.
- ###### Sense: 
	- Specifies whether the vector **points** in the **positive/negative** direction along that angle.
		- Though the sense is not necessarily **the** direction.
	- The sense of a vector is **specified** by the **order** of the **two points** on a **line parallel** to the **vector**. 

### Scalar Multiplication component:
Scalar multiplication refers to the multiplication of a vector by a scalar number ***N***.
- I.e. Scales the vector. 
	- If *N > 0* then a vector in the same sense will result. 
	- If *N < 0* then a vector in the opposite sense will result.
	- The vector's **new magnitude** is **equal** to the **product** of the **initial vector's length** and **N***.
		![[Pasted image 20240327232525.png|600]]

### Unit X, Unit Y, Unit Z component:
Define unit vectors along the x, y, and z axes. 
	- (F) input: can be used to set a length through embedded scalar multiplication. 


