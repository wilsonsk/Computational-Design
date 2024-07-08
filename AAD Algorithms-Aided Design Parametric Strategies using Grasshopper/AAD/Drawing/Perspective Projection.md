# Perspective Projection
![[Pasted image 20240708065933.png|400]]
I don’t understand how the distance of the perspective view affects the image when the eye point moves but plane is constant moves closer or farther from object of projection and then when the eye point is constant but the plane moves closer or farther from object of projection.

To understand how the distance of the perspective view affects the image when the eye point moves but the projection plane is constant, and vice versa, let's analyze the principles of perspective projection.

### Key Concepts:

1. **Eye Point (e)**: The location of the observer's eye or camera.
2. **Principal Point (m)**: A point on the horizon line where the projection lines converge.
3. **Projection Plane (P)**: The plane onto which the 3D object is projected to form a 2D image.

### Two Scenarios:

#### 1. Fixed Eye Point, Changing Distance of the Projection Plane:

- **Fixed Eye Point (e):** The observer or camera stays in the same position.
- **Changing Projection Plane Distance (P):** The plane moves closer or farther from the object being projected.

In this scenario:
##### Smaller Distance of the Projection Plane to the Object
- When the projection plane moves **closer** to the object, the image appears larger because the projection plane intercepts a larger section of the projection rays.
- When the projection plane is closer to the object, the portion of the object that is captured in the image is determined by the angles at which the projection lines intersect the plane.
- The closer the plane is to the object, the larger the angle between the projection lines, causing more of the object to be included in the image. This is why the image captures more of the object, despite the plane being closer to the object.
##### Larger Distance of the Projection Plane to the Object 
- When the projection plane moves **farther** from the object, the image appears smaller as it intercepts a smaller section of the projection rays.
- When the projection plane moves farther from the object, the projection lines become more parallel. This results in a smaller section of the object being captured in the image, as the angles between the projection lines narrow.
#### 2. Moving Eye Point, Fixed Projection Plane:

- **Moving Eye Point (e):** The observer or camera moves closer or farther from the object.
- **Fixed Projection Plane (P):** The plane remains at the same position.

In this scenario:
##### Smaller Distance of the Eye Point to the Object
- When the eye point moves **closer** to the object, the perspective effect becomes more pronounced. The object appears larger and more parts of it come into view.
- The closer the eye point is to the object, the wider the angles at which the projection lines intersect the projection plane. This captures more of the object in the image but can result in more distortion.
##### Larger Distance of the Eye Point to the Object
- When the eye point moves **farther** from the object, the perspective effect diminishes. The object appears smaller, and less of it is visible due to a narrower viewing angle.
- This typically means the object appears smaller overall because the projection lines are more parallel, reducing the angles at which they intersect the projection plane.
- However, the entire object can still be captured within the field of view, leading to a larger and more unified image of the object with less distortion.
### Visualization of the Effects:

#### Top Row of Images:

1. **Image 1 to Image 3**: These images demonstrate how changing the projection plane's distance affects the image size. The eye point remains fixed, but as the projection plane moves closer, the projected image becomes larger.

#### Bottom Row of Images:

1. **Image 4 to Image 6**: These images show the effect of moving the eye point while keeping the projection plane fixed. As the eye point moves closer, the image enlarges and more detail is visible. As the eye point moves farther, the image contracts.
#### Image 4:

- **Eye Point e4e_4e4​** is closest to the object.
- **Projection Plane PPP** is fixed.
- The closer eye point results in a more pronounced perspective distortion, capturing a wider vertical section of the object. This causes the object to appear stretched and more of the object’s height is visible.

#### Image 5:

- **Eye Point e5e_5e5​** is at an intermediate distance.
- **Projection Plane PPP** is fixed.
- The intermediate distance balances the perspective effect, reducing distortion compared to Image 4. The captured image is more proportional but less of the object is visible compared to Image 4.

#### Image 6:

- **Eye Point e6e_6e6​** is farthest from the object.
- **Projection Plane PPP** is fixed.
- The farther eye point causes the projection lines to become more parallel. This results in a smaller, more uniform section of the object being visible with less distortion. However, the object appears larger overall because it fits more cohesively within the frame.
### Summary:

- **Fixed Eye Point, Moving Projection Plane**: Affects the magnification of the image. Closer plane means a larger image, and farther plane means a smaller image.
- **Moving Eye Point, Fixed Projection Plane**: Affects the perspective and field of view. Closer eye point results in a more pronounced perspective and larger image, whereas a farther eye point results in a reduced perspective effect and smaller image.

Understanding these principles helps in controlling the perspective projection in both architectural visualizations and 3D modeling to achieve the desired visual effects.