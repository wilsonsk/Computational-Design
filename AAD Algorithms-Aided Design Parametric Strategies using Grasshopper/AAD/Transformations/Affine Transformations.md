---
up:
  - "[[Transformations]]"
related:
  - "[[Vectors]]"
  - "[[Data Relationships]]"
  - "[[Points]]"
  - "[[Parameters]]"
  - "[[Curves]]"
  - "[[Surfaces]]"
  - "[[Numbers]]"
date created: 2024-03-29
---
# Affine Transformations
Include scaling, shearing, projection and mapping components.

## Scaling component (uniform scaling):

### Scale component:
Is a geometric transformation that **enlarges** or **reduces** objects **uniformly** in the x, y, and z directions. 
- It resizes an **initial geometry (G)** by a **scale factor (F)** relative to and maintaining its distance from a **center of scaling point (C)**. 
	- **Center of scaling point**: ^center-of-scaling-point
		- The center of scaling can be any point.
			- It is the reference point from which the scaling operation is applied to the geometry. 
				- Meaning, that the **distance** from this point to **any point** on the geometry will be scaled by the scaling factor.
				- It does **not** have to be **on** the geometry being scaled. 
					- The point can be **anywhere** in the **3D space** relative to the geometry. 
						- When the point is off the geometry, it creates an expanding or contracting effect towards or away from that point. 
							![[Pasted image 20240329150520.png|400]]
		- How it works:
			1. Grasshopper determines the **distance** and **direction** via a **vector** for each point of the geometry to the **center of scaling point**.
			2. The **scaling factor** is applied to the **length** of this vector.
				1. If different scaling factors are provided for the x, y, and z directions, then the components of the vector in each direction are scaled accordingly. 
			3. The **new length** of the vector (after scaling) determines the **new position** of the **point** of the geometry. 
			4. Repeats this process for all points that constitute the geometry, thus maintaining the proportions and orientations. 
	- A scalar is a positive number and cannot be 0. 
		- 0< (F) < 1 : reduces object size; this is in essence *division*.
		- (F) = 1 : object size does not change.
		- (F) > 1 : increases object size.
- Scaling can also be performed on several objects, simultaneously. 
	- The entire set of geometry will be scaled by the same proportion. 
- Alternatively, **different** scaling factors can be applied to each geometry entity. 
	![[Pasted image 20240329152728.png|400]]
	- *More complex forms of (numerical) sequences of scaling factors can be generated using the the mathematical functions of the **Graph Mapper** component.*
		- *Custom mathematical equations can be used also.*
			![[Pasted image 20240329155019.png|500]]
			![[Pasted image 20240329155621.png|400]]


### Image Sampler component
Converts the chromatic information of an image into numerical values.
- Every rectangular picture can be visualized as a bi-dimensional domain ranging by default between 0 and 1. 
	- If a rectangular grid is superimposed onto the image, then each grid point *P* - defined by its *uv* coordinates in the LCS - provides and **intensity** value as an output.
		- **Intensity**: 
			- Measures the **color** values of the image at *P* dependent upon the specific *color model*: RBG, grayscale, etc.  and outputs a value.
				- For example: the grayscale model measures the intensity of a pixel and outputs values ranging from **0 (black) to 1 (white)** with fractional grayscale values in between. 
- Used via **loading** an **image**, **selecting a color model** and specifying whether to **interpolate**. 
	- **Interpolation** in this context is used to determine or estimate the color values at a point in the image that does **not correspond directly** to the **pixel grid**. 
		- Is a way of *blending* of gradations, affecting the *smoothness* of the output values.
			- Nearest Neighbor interpolation: 
				- Simply used the color data of the nearest pixel to the sample point **without** any **blending**. 
				- Fast computation.
				- Blocky, low resolution outputs.
			- Bilinear Interpolation: 
				- Takes a weighted average of the four closest pixels to the sample point. 
				- Provides smoother transitions between pixels (colors).
				- Medium computation efficiency.
			- Bicubic Interpolation:
				- Takes a weighted average of the 16 closest pixels (4x4 area) around the sample point. 
				- Results in an even smoother output result. 
				- More computationally intensive. 
- **Inputs**:
	- Set of points with *uv* coordinates.
		- Usually requires the **Surface CP** component to convert points of a geometry from WCS to LCS.
			- From which the LCS points (*uv*) can be input into the *uv* input of the **Evaluate Image Sampler** component. 
- **Outputs**:
	- A list of numbers or **intensity values**.
	- Can be used as **scaling factors** for a transformation.
		- ***Remember***: 
			- If a **grayscale** color model is used, then the **surface** must **reparametrized** to match the 0-1 domain of the model.
			- Pure black pixels return **null** intensity values (i.e. 0). 
				- Can use **Maximum** component to replace 0 with a different value (such as 0.1).
		![[Pasted image 20240329162016.png|500]]
		![[Pasted image 20240329162202.png|400]]
- The **Image Sampler** component can be used as input for **different transformations**.
	- For example:
		- Moving and rotating bricks of a wall relative to a grayscale image.
			- The brick's **gravity points** (whose coordinates were reparametrized) were used as *uv* points for the **Image Sample** component.
- For **color**:
	- RGB values can be split into four channels using the **ARGB** component. 
		- **Outputs**: values between 0-1 by default (range can be adjusted to [0,255] in the context menu)
			- (A): Alpha channel.
			- (R): Red channel.
			- (G): Green channel.
			- (B): Blue channel.
	- For example: "**Offsetting**" (creating a parallel or concentric copy of a geometry at a specified **distance**) a variable offset from a flat surface using a color image (specifically the red area of the image):
		- **Surface Closest Point** component is used to extract the *uv* coordinates of a point on the geometry (relative to a sample point). 
			- I.e. used to convert a WCS coordinated surface to LCS.
		- The output *uv* coordinates are passed in to the **Image Sampler** component. 
			- The output of the **Image Sampler** component is then fed into the **ARGB** component.
				- The generated list of numbers from this component composes the **scaling factors** of a move transformation. 
					![[Pasted image 20240329222006.png]]