# Perspective Projection
![[Pasted image 20240708065933.png|400]]
### Key Concepts:

1. **Eye Point (e)**: The location of the observer's eye or camera.
2. **Principal Point (m)**: A point on the horizon line where the projection lines converge.
3. **Projection Plane (P)**: The plane onto which the 3D object is projected to form a 2D image.
	Also called the "**Picture Plane**".

### Detailed Summary of Primary Factors in Perspective Projection

### Primary Factors of Perspective Projection:

1. **Angle of Projection Rays (Determined by Object Distance)**:
    
    - **Description**: The angles at which projection rays from the station point (S) intersect the projection plane (P).
    - **Object Distance (D1)**: The distance between the object (O) and the projection plane (P).
    - **Determining Factors**:
        - **Closer Objects (Smaller D1)**: The projection rays intersect the projection plane at wider angles.
        - **Farther Objects (Larger D1)**: The projection rays intersect the projection plane at narrower angles.
    - **Effects on Image**:
        - **Wider Angles (Close Objects)**: The object appears larger and more distorted on the projection plane.
        - **Narrower Angles (Far Objects)**: The object appears smaller and less distorted on the projection plane.
2. **Field of View (FOV) (Determined by Perspective Distance)**:
    
    - **Description**: The angular extent of the observable scene captured by the projection plane, visualized as a cone extending from the station point to the edges of the projection plane.
    - **Perspective Distance (D2)**: The distance between the station point (S) and the projection plane (P).
    - **Determining Factors**:
        - **Closer Station Point (Smaller D2)**: Results in a wider FOV.
        - **Farther Station Point (Larger D2)**: Results in a narrower FOV.
    - **Effects on Image**:
        - **Wider FOV (Close Station Point)**: Captures more of the scene but with increased distortion.
        - **Narrower FOV (Far Station Point)**: Captures less of the scene with reduced distortion.

### Amplifying and Contrasting Effects: Three Scenarios

#### Scenario 1: Fixed Station Point, Decreasing Object Distance (Increasing Perspective Distance)

- **Setup**:
    
    - The station point (S) is fixed.
    - The projection plane (P) moves closer to the object (O), decreasing the object distance (D1).
    - This also increases the effective perspective distance (D2) relative to the object.
- **Effects**:
    
    - **Angle of Projection Rays**: As the object distance decreases, the projection rays intersect the projection plane at wider angles.
        - **Result**: The object appears larger and more distorted on the projection plane.
    - **Field of View (FOV)**: As the projection plane moves closer to the object, the FOV narrows.
        - **Result**: The projection plane captures a smaller portion of the scene around the object, focusing more on the object itself.
- **Combined Effect**: The object appears significantly larger and more distorted, with a narrow focus on the object and less of the surrounding scene visible.
    

#### Scenario 2: Fixed Projection Plane, Decreasing Perspective Distance

- **Setup**:
    
    - The projection plane (P) is fixed.
    - The station point (S) moves closer to the projection plane, decreasing the perspective distance (D2).
    - The object distance (D1) remains constant.
- **Effects**:
    
    - **Angle of Projection Rays**: The object distance remains the same, so the angles at which the rays intersect the projection plane do not change.
        - **Result**: The size and distortion of the object on the projection plane remain the same.
    - **Field of View (FOV)**: As the station point moves closer to the projection plane, the FOV widens.
        - **Result**: The projection plane captures a larger portion of the scene, making the object appear smaller within a broader context.
- **Combined Effect**: The object maintains its size and distortion, but it appears smaller within a wider scene due to the increased FOV.
    

#### Scenario 3: Fixed Perspective Distance, Decreasing Object Distance

- **Setup**:
    
    - The distance between the station point (S) and the projection plane (P) is fixed, maintaining a constant perspective distance (D2).
    - Both the station point and the projection plane move together closer to the object (O), decreasing the object distance (D1).
- **Effects**:
    
    - **Angle of Projection Rays**: As the object distance decreases, the projection rays intersect the projection plane at wider angles.
        - **Result**: The object appears larger and more distorted on the projection plane.
    - **Field of View (FOV)**: The perspective distance remains the same, so the FOV does not change.
        - **Result**: The projection plane captures the same angular extent of the scene.
- **Combined Effect**: The object appears larger and more distorted, but the overall field of view remains the same.
    

### Conclusion:

In perspective projection, the angle of projection rays and the field of view are primary factors that dictate how an image looks. The angle of projection rays, determined by the object distance (D1), affects the size and distortion of the object on the projection plane. The field of view, determined by the perspective distance (D2), affects how much of the scene is visible. By manipulating these distances, you can control the visual impact and spatial relationships in a perspective projection.

## Relation to Focal Length:

1. **Station Point (e)**: The position of the photographer (or the camera sensor).
2. **Projection Plane (P)**: The plane where the image is captured, which is effectively controlled by the camera lens.

### Roles:

1. **Photographer (Station Point Control)**:
    
    - The photographer physically controls the station point by moving closer to or farther from the object or scene.
    - Changing the station point changes the perspective from which the scene is viewed.
    - Moving the station point closer to the object increases perspective distortion and captures more of the surroundings in a wide view (similar to a wide-angle lens effect).
    - Moving the station point farther from the object decreases perspective distortion and captures a narrower, more focused view of the scene (similar to a telephoto lens effect).
2. **Camera Lens (Projection Plane Control)**:
    
    - The lens controls the effective position of the projection plane relative to the object or scene.
    - A shorter focal length (wide-angle lens) moves the projection plane closer to the station point, increasing the field of view and capturing more of the scene.
    - A longer focal length (telephoto lens) moves the projection plane farther from the station point, narrowing the field of view and magnifying the subject, capturing less of the surroundings.

### Visualization:

- **Wide-Angle Lens (Short Focal Length)**:
    
    - **Projection Plane**: Closer to the station point.
    - **Effect**: Wider field of view, more perspective distortion, captures more of the scene.
    - **Photographer's Role**: Can move closer or farther from the object to adjust the perspective.
- **Telephoto Lens (Long Focal Length)**:
    
    - **Projection Plane**: Farther from the station point.
    - **Effect**: Narrower field of view, less perspective distortion, magnifies the subject.
    - **Photographer's Role**: Can move closer or farther from the object to adjust the perspective, but the lens's focal length will always limit the field of view to a narrower range.

### Practical Example:

1. **Photographer’s Positioning (Station Point)**:
    
    - If a photographer wants to capture a building from a distance, they might stand farther away, reducing perspective distortion.
    - If they want a dramatic effect with pronounced perspective, they might move closer to the building.
2. **Lens Choice (Projection Plane)**:
    
    - Using a wide-angle lens (e.g., 24mm) while close to the building will exaggerate the perspective, making the building appear larger and more distorted.
    - Using a telephoto lens (e.g., 300mm) from the same distance will compress the perspective, making the building appear flatter and closer to other objects in the scene.

### How Focal Length Affects the Perspective:
### Key Concepts:

1. **Focal Length (f)**: The distance between the lens and the image sensor when the subject is in focus. It determines the field of view.
2. **Field of View (FOV)**: The extent of the scene captured by the camera, which is inversely proportional to the focal length.
3. **Projection Plane (Image Plane)**: The plane onto which the image is projected inside the camera, typically where the sensor or film is located.

For example:
- For a 24mm lens, the effective projection plane distance is approximately 24mm from the station point.
- For a 300mm lens, the effective projection plane distance is approximately 300mm from the station point.

1. **Wide-Angle Lens (Short Focal Length)**:
    - Captures a wider field of view.
    - The projection plane can be imagined as being closer to the station point to encompass a larger area of the scene.
2. **Telephoto Lens (Long Focal Length)**:
    - Captures a narrower field of view.
    - The projection plane can be imagined as being farther from the station point, focusing on a smaller area of the scene with greater detail.

### Effective Changes in Position:

- **Long Focal Length (Telephoto Lens)**:
    - **Primary Effect**: It effectively moves the projection plane forward, closer to the object. This is because a telephoto lens compresses the scene and captures a narrower field of view.
    - **Station Point**: Remains fixed. The position of the camera or the observer does not change.

### Visualization:

1. **Wide-Angle Lens (e.g., 24mm)**:
    
    - Imagine the projection plane is very close to the eye point.
    - This plane captures a wide area due to the large cone of vision.
2. **Telephoto Lens (e.g., 300mm)**:
    
    - Imagine the projection plane is much farther from the eye point.
    - This plane captures a narrow area due to the small cone of vision.
    - The object appears larger and more compressed, as if the projection plane has moved forward towards the object.
### Calculation Steps:

1. **Determine the Field of View (FOV)**:
    
	- The horizontal, vertical, and diagonal fields of view can be calculated using the focal length and the dimensions of the camera sensor.
	- For a full-frame sensor (36mm x 24mm), the calculations can be done as follows:
	    - Horizontal FOV: $\text{FOV}_h = 2 \cdot \arctan\left(\frac{\text{sensor width}}{2 \cdot f}\right)$
	    - Vertical FOV: $\text{FOV}_v = 2 \cdot \arctan\left(\frac{\text{sensor height}}{2 \cdot f}\right)$
	    - Diagonal FOV: $\text{FOV}_d = 2 \cdot \arctan\left(\frac{\text{sensor diagonal}}{2 \cdot f}\right)$
	    - Sensor diagonal: $\text{sensor diagonal} = \sqrt{\text{sensor width}^2 + \text{sensor height}^2}$

2. **Calculate Effective Distance**:
    
	- To understand how the projection plane shifts, consider the following geometric relationship for field of view:
	    - If we assume the projection plane is perpendicular to the line of sight and parallel to the sensor, the effective distance (d) from the station point can be estimated using similar triangles.
	- Using the horizontal FOV for simplicity:
	    - $d = \frac{\text{sensor width}}{2 \cdot \tan\left(\frac{\text{FOV}_h}{2}\right)}$

### Practical Example:

Let's calculate the effective distance for two lenses, a 24mm wide-angle lens and a 300mm telephoto lens, on a full-frame sensor:

1. **Sensor Dimensions**:
    
    - Width = 36mm
    - Height = 24mm
    - Diagonal = 43.3mm (calculated using Pythagorean theorem)
2. **Field of View for 24mm Lens**:
	- Horizontal FOV: $\text{FOV}_h = 2 \cdot \arctan\left(\frac{36}{2 \cdot 24}\right) = 2 \cdot \arctan(0.75) \approx 74.05^\circ$

	- Effective Distance (d): $d_{24} = \frac{36}{2 \cdot \tan\left(\frac{74.05^\circ}{2}\right)} \approx \frac{36}{2 \cdot \tan(37.025^\circ)} \approx \frac{36}{1.50} \approx 24mm$

3. **Field of View for 300mm Lens**:

	- Horizontal FOV: $\text{FOV}_h = 2 \cdot \arctan\left(\frac{36}{2 \cdot 300}\right) = 2 \cdot \arctan(0.06) \approx 6.86^\circ$

	- Effective Distance (d): $d_{300} = \frac{36}{2 \cdot \tan\left(\frac{6.86^\circ}{2}\right)} \approx \frac{36}{2 \cdot \tan(3.43^\circ)} \approx \frac{36}{0.12} \approx 300mm$

## Drawing a Perspective Grid
By measuring the distance from the station point to the projection plane based on the focal length of the lens (50mm in this case), you can accurately set up a perspective grid. 
	This approach ensures that the perspective distortion and field of view are consistent with what would be captured by a 50mm lens, providing a realistic representation of depth and scale in your drawing.

*For example:* 
	Using a 50mm focal length, you can indeed use the focal length to determine the distance from the station point (eye point) to the projection plane. Here’s how you can set this up:

### Setting Up the Perspective Grid with a 50mm Focal Length:

1. **Station Point (Eye Point)**: This is the point where the observer’s eye or the camera sensor is located.
2. **Projection Plane**: This is the plane onto which the scene is projected. In perspective drawing, this is typically represented by the picture plane.

### Steps to Draw the Perspective Grid:

1. **Determine the Distance**:
    
    - For a 50mm lens, set the distance from the station point to the projection plane as 50mm. This distance will act as a scaling factor for your grid.
2. **Horizon Line and Vanishing Point**:
    
    - Draw the horizon line, which represents the viewer's eye level.
    - The center of view, or the principal vanishing point, is located on this horizon line directly in front of the station point.
3. **Measure the Distance**:
    
    - Measure 50mm from the station point (eye point) to the projection plane along the line of sight.
    - This point on the projection plane corresponds to the principal vanishing point.

### Drawing the Grid:

1. **Vertical Lines**:
    
    - Draw vertical lines at regular intervals to represent objects receding into the distance.
    - Ensure these lines converge towards the principal vanishing point on the horizon line.
2. **Horizontal Lines**:
    
    - Draw horizontal lines to create the grid pattern.
    - These lines should also converge towards the vanishing points on the horizon line for accurate perspective.
3. **Depth Lines**:
    
    - To draw lines indicating depth, use the 50mm measurement as a guide.
    - These lines should converge towards the vanishing point, creating the sense of depth.

### Example:

Let's create a simple example of a perspective grid with a 50mm focal length:

1. **Establish the Station Point**:
    
    - Mark a point as the station point (eye point).
2. **Draw the Projection Plane**:
    
    - Measure 50mm from the station point along the line of sight and mark this as the projection plane's intersection on the horizon line (principal vanishing point).
3. **Draw the Horizon Line**:
    
    - Draw a horizontal line through the principal vanishing point.
4. **Add Vertical and Horizontal Grid Lines**:
    
    - Draw vertical lines that converge towards the principal vanishing point.
    - Draw horizontal lines that also converge towards the vanishing point.
5. **Define Depth**:
    
    - Use the 50mm measurement to determine the scale for depth, ensuring all lines recede accurately towards the vanishing point.

## Parallel Projection
In parallel (orthographic) projection, the key concept is that the projection lines are parallel and do not converge, regardless of the distance between the station point (observer) and the projection plane. 
### Terms and Concepts:

1. **Station Point (Eye Point)**: The hypothetical point where the observer's eye or the camera sensor is located.
2. **Projection Plane**: The plane onto which the 3D object is projected to form a 2D image.
3. **Distance Between Station Point and Projection Plane**: This distance is crucial in perspective projection but in parallel projection, it’s typically considered infinite to eliminate perspective distortion.

### Parallel (Orthographic) Projection:

- **Projection Lines**: In parallel projection, these lines are parallel and perpendicular to the projection plane.
- **Infinite Distance**: Conceptually, the distance between the station point and the projection plane is considered infinite. This makes the projection lines parallel and removes any perspective effects.
- **No Perspective Distortion**: Objects are represented in true scale, maintaining their actual dimensions regardless of their depth in the scene.

### Arbitrary Distance in Parallel Projection:

- The **projection plane** can be set at any arbitrary distance from the object.
- In parallel projection, the distance between the station point and the projection plane is not explicitly defined because it’s conceptually infinite.
- **Infinite Distance Assumption**: This assumption means that no matter where the projection plane is placed, the projection lines remain parallel. Thus, the station point and the projection plane are infinitely far apart in conceptual terms.

### Key Points:

1. **In Perspective Projection**:
    
    - The distance between the station point and the projection plane affects the perspective distortion.
    - This distance is finite and is often referred to as the **focal length** in photography, or the **distance from the eye point to the picture plane** in drawing.
2. **In Parallel Projection**:
    
    - The distance between the station point and the projection plane is theoretically infinite.
    - The term for this distance is often **conceptually infinite distance** or simply **infinite distance**.
    - Setting the projection plane at any practical distance does not change the fact that the projection lines are parallel.

## Projection Plane in Parallel Projection
By adjusting the projection plane’s position relative to the object, you can control the level of detail and the portion of the scene captured in your drawing, all while maintaining the parallel nature of the projection and avoiding perspective distortion.
- **Movable Projection Plane**: In parallel projection, the projection plane can be moved closer to or farther from the object/scene.
- **Maintaining Parallel Lines**: The infinite distance assumption ensures that the projection lines remain parallel, regardless of the projection plane's position relative to the object.
- **True Dimensions**: Moving the projection plane changes the portion of the object captured but retains the true dimensions and proportions of the object without perspective distortion.
### Moving the Projection Plane:

1. **Arbitrary Positioning**:
    
    - The projection plane (picture plane) can be moved closer to or farther from the object/scene without affecting the parallel nature of the projection lines.
    - This does not alter the relationship between the projection lines and the station point, as they remain parallel regardless of the projection plane’s position.
2. **Closer Projection Plane**:
    
    - When you move the projection plane closer to the object, the size of the projected image of the object increases. This is because the plane intercepts more of the parallel projection lines at a closer range, effectively enlarging the details of the object in the image.
	    - Enlarges the object or scene details in the projected image.
		- Shows fewer elements but with more detail.
		- Narrower FOV in terms of the portion of the scene captured.
1. **Farther Projection Plane**:
    
    - Conversely, when you move the projection plane farther from the object, the size of the projected image decreases. The plane captures a larger portion of the scene, but individual details are smaller.
	    - Reduces the size of the object or scene details in the projected image.
		- Shows more elements but with less detail.
		- Wider FOV in terms of the portion of the scene captured.
1. **Effect on the Image**:
    
    - Moving the projection plane closer to the object: The projected image will show a smaller portion of the object but in greater detail.
    - Moving the projection plane farther from the object: The projected image will show a larger portion of the object but in less detail.
### Field of View (FOV) in Parallel Projection:

- In parallel projection, the FOV is not influenced by the concept of convergence as it is in perspective projection. Instead, it is determined by the size of the projection plane and its position relative to the object.
- Moving the projection plane closer effectively narrows the FOV to a smaller portion of the scene but increases the detail (scale) of that portion.
- Moving the projection plane farther widens the FOV to include more of the scene, but reduces the detail (scale) of each part.
### Impact of Infinite Distance:

- The infinite distance between the station point and the projection plane ensures that the projection lines remain parallel, eliminating perspective distortion.
- This means that while the station point is conceptually infinitely far away, the position of the projection plane relative to the object is what changes the captured image size and detail level.