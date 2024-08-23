# Rotational Surfaces
The transcript and image provided are discussing rotational surfaces, specifically focusing on the functions of two variables, which result in 3D surfaces when visualized.

Let’s break it down:

1. **Functions:**
   - **\( f(x, y) = \sqrt{x^2 + y^2} \):** This function represents a cone. The expression inside the square root, \( x^2 + y^2 \), is the distance from the origin (0,0) in the xy-plane. The square root of that distance forms the z-coordinate, creating a circular symmetry around the z-axis. When plotted, it forms a conical shape, specifically the upper part of the cone since z is non-negative (z ≥ 0).
   - **\( g(x, y) = x^2 + y^2 \):** This function represents a paraboloid. Here, the value of z increases as the square of the distance from the origin increases, producing a parabolic surface that also exhibits rotational symmetry about the z-axis.

2. **Rotational Surfaces:**
   - Both functions depend on the distance from the origin in the xy-plane, which means that they are symmetrical around the z-axis. This symmetry is why they are referred to as rotational surfaces. Essentially, if you rotate the graph of the function around the z-axis, the surface remains unchanged. This happens because the value of the function at any point \((x, y)\) depends only on the distance \( \sqrt{x^2 + y^2} \) from the origin, and not on the direction.

3. **The Concept of Rotation:**
   - The teacher emphasizes that since the functions depend only on the distance from the origin, they exhibit circular symmetry. If you draw a circle of any radius centered at the origin in the xy-plane, the function’s value (and thus the height z) will be the same at all points on that circle. This is why these surfaces are called rotational surfaces.

4. **Visual Interpretation:**
   - The cone is formed by the function \( f(x, y) = \sqrt{x^2 + y^2} \), and it has a sharp tip at the origin, gradually opening up as you move away from the origin.
   - The paraboloid, formed by the function \( g(x, y) = x^2 + y^2 \), is smoother and gradually curves upward as you move away from the origin, similar to a bowl shape.

Your teacher is trying to help you visualize how these functions produce 3D surfaces by revolving around the z-axis, where each level curve (or contour) in the xy-plane is a circle, and the height (z-value) is determined by the distance from the origin.

Would you like further clarification on how these equations relate to their geometric interpretations, or how this concept fits within the broader scope of multivariable calculus and design thinking?

## Distance Only
Let’s go deeper into what is meant by a function "depending on the distance \( \sqrt{x^2 + y^2} \) from the origin and not on the direction." This concept is essential for understanding rotational surfaces, so we'll break it down step by step.

### Understanding Distance from the Origin

In two-dimensional space (the xy-plane), the distance from any point \( (x, y) \) to the origin (0, 0) can be found using the Pythagorean theorem. This distance is:

\[
r = \sqrt{x^2 + y^2}
\]

This equation gives the radial distance \( r \), which measures how far a point \( (x, y) \) is from the origin. 

#### What does "depending on the distance" mean?

For a function \( f(x, y) \) or \( g(x, y) \) that depends **only on the distance** \( r = \sqrt{x^2 + y^2} \), this implies that the output of the function (the z-coordinate, in this case) is determined solely by how far the point \( (x, y) \) is from the origin, **regardless of the direction**. 

To clarify:

- **Direction** refers to the angle the point \( (x, y) \) makes with the x-axis (this angle is typically denoted as \( \theta \) in polar coordinates).
- **Distance** (or radius, \( r \)) refers to how far the point is from the origin.

When a function depends **only on the distance** \( r = \sqrt{x^2 + y^2} \), it means that all points that are the same distance from the origin will produce the same function value (z-value), no matter what direction they lie in.

### Contrast with Conventional Functions

In a more conventional function of two variables, the output might depend both on the **distance** from the origin and the **direction** of the point.

For example:

- A function like \( f(x, y) = x + y \) does **not** depend solely on the distance from the origin. The output (z-value) depends on the specific values of x and y. If you move around in a circle (keeping the distance from the origin constant but changing direction), the function value changes because the specific values of x and y change.
- On the other hand, for a function like \( f(x, y) = \sqrt{x^2 + y^2} \), the output (z-value) is the same for all points that are the same distance from the origin, even if those points lie in different directions.

### Symmetry and Rotational Surfaces

Because these functions depend only on the distance from the origin (and not the direction), they exhibit **rotational symmetry** around the z-axis. 

1. **Rotational Symmetry**: If you take a surface generated by such a function and rotate it around the z-axis, the surface remains unchanged because all points that lie on a circle centered at the origin have the same z-value.

2. **Example: The Cone** 
   - The cone described by \( f(x, y) = \sqrt{x^2 + y^2} \) has rotational symmetry because for any point \( (x, y) \), the height \( z \) is just the distance from the origin. 
   - Imagine all the points at a distance \( r \) from the origin in the xy-plane. These points form a circle, and every point on that circle will have the same z-value (height), creating a cone when extended along the z-axis.

3. **Example: The Paraboloid**
   - The paraboloid described by \( g(x, y) = x^2 + y^2 \) has a similar rotational symmetry. Here, the z-value is proportional to the square of the distance from the origin. All points at the same distance from the origin will lie on a circle in the xy-plane, and they will all have the same height (z-value), creating a smooth parabolic surface that opens upward.

### Connecting to Polar Coordinates

To further understand this, consider polar coordinates \( (r, \theta) \):

- \( r = \sqrt{x^2 + y^2} \) is the radial distance from the origin.
- \( \theta = \arctan(y/x) \) is the angle the point makes with the positive x-axis (the direction).

In polar coordinates, a function that depends only on \( r \) (and not on \( \theta \)) is **radially symmetric**. This is exactly what's happening with these functions \( f(x, y) = \sqrt{x^2 + y^2} \) and \( g(x, y) = x^2 + y^2 \). They only depend on \( r \), which means that all points with the same radius have the same z-value, no matter what \( \theta \) is. This leads to circular (or rotational) symmetry in the surface.

### Summarizing the Difference

- **Conventional Functions**: Functions like \( f(x, y) = x + y \) depend on both the specific x and y values, meaning the output changes if you change direction in the xy-plane, even if the distance from the origin stays the same.
  
- **Radial Functions (Rotational Symmetry)**: Functions like \( f(x, y) = \sqrt{x^2 + y^2} \) depend only on the distance from the origin. The function value remains the same for all points that are the same distance from the origin, resulting in a surface that is symmetric around the z-axis (rotational symmetry).

This rotational symmetry is what makes these surfaces "rotational surfaces," as the surface remains the same when rotated around the z-axis. 

The expression \( \sqrt{x^2 + y^2} \) represents the Euclidean distance from the origin in the xy-plane to the point \( (x, y) \). This distance is often denoted by \( r \), and it forms the basis of polar coordinates. Let's dive into this in detail to understand how this function "depends only on \( r \)."

### Step 1: Understanding the Expression \( \sqrt{x^2 + y^2} \)

1. **What does \( \sqrt{x^2 + y^2} \) represent?**
   - \( \sqrt{x^2 + y^2} \) is the formula for the distance between the origin (0, 0) and a point \( (x, y) \) in two-dimensional space. This distance is commonly denoted as \( r \), so:
     \[
     r = \sqrt{x^2 + y^2}
     \]
   - This distance does not care about the specific values of \( x \) or \( y \) independently; it only cares about how far the point \( (x, y) \) is from the origin.

### Step 2: Polar Coordinates

In polar coordinates, a point in the plane is described using the radius \( r \) (the distance from the origin) and the angle \( \theta \) (the direction from the origin to the point). The relationships between Cartesian coordinates \( (x, y) \) and polar coordinates \( (r, \theta) \) are:

\[
x = r \cos(\theta)
\]
\[
y = r \sin(\theta)
\]
\[
r = \sqrt{x^2 + y^2}
\]

- **\( r \)**: This is the radial distance from the origin, i.e., how far the point is from the origin.
- **\( \theta \)**: This is the angular direction, representing the angle between the positive x-axis and the line connecting the origin to the point \( (x, y) \).

### Step 3: Why Does \( \sqrt{x^2 + y^2} \) Only Depend on \( r \)?

When we say that the expression \( \sqrt{x^2 + y^2} \) "depends only on \( r \)", we mean that:

- The value of the expression \( \sqrt{x^2 + y^2} \) depends only on the distance from the origin, which is \( r \).
- It **does not** depend on the specific values of \( x \) and \( y \) individually, nor does it depend on the direction \( \theta \).

#### Key Concept: Radial Dependence

- **Direction \( \theta \)**: This is the angle that specifies where the point is located relative to the positive x-axis. Points with the same \( r \) but different \( \theta \) values lie on a circle centered at the origin.
- **Radial Dependence**: The function \( \sqrt{x^2 + y^2} \) only depends on \( r \), meaning it gives the same value for any point that is the same distance from the origin, regardless of the angle \( \theta \).

For example:
- The point \( (3, 0) \) has coordinates \( (r, \theta) = (3, 0) \), and the distance from the origin is \( r = 3 \).
- The point \( (0, 3) \) has coordinates \( (r, \theta) = (3, \frac{\pi}{2}) \), and the distance from the origin is also \( r = 3 \).

For both points, the function \( \sqrt{x^2 + y^2} \) will give the same output, \( 3 \), because they both have the same distance from the origin. The angle \( \theta \) (direction) does not matter—only the radial distance \( r \) matters.

This is what it means for the function to "depend only on \( r \) and not on the direction \( \theta \)."

### Step 4: Visualizing Radial Symmetry

Imagine plotting the function \( z = \sqrt{x^2 + y^2} \) in 3D. The function takes the distance from the origin as input and outputs the height \( z \). This means that all points at the same distance \( r \) from the origin will have the same height \( z \).

If you move around a circle centered at the origin (i.e., if you change \( \theta \)), the distance \( r \) remains the same, and so does the height \( z \). This is why the surface generated by this function has rotational symmetry around the z-axis—no matter which direction you move, as long as you stay at the same distance from the origin, the height remains constant.

### Step 5: Contrast with Non-Radial Functions

Consider a different function like \( f(x, y) = x + y \). This function does **not** depend solely on the distance \( r \). If you move around in a circle while keeping \( r \) constant, the values of \( x \) and \( y \) will change, and so will the function output.

For example:
- At \( (3, 0) \), \( f(3, 0) = 3 \).
- At \( (0, 3) \), \( f(0, 3) = 3 \).
- But at \( (1, \sqrt{8}) \), which also lies on the circle of radius 3, \( f(1, \sqrt{8}) = 1 + \sqrt{8} \), which is different.

This function depends on both \( x \) and \( y \), not just their combined distance from the origin, so it does not have rotational symmetry.

### Summary

- **\( \sqrt{x^2 + y^2} \) depends only on the distance from the origin**: This means that the function output is the same for any point that is the same distance from the origin, regardless of the direction. It only cares about how far you are from the origin, not where you are relative to the axes.
- **Radial Symmetry**: Because the function depends only on the distance, it exhibits rotational symmetry about the z-axis. Rotating the graph around the z-axis does not change the surface.

This radial dependence makes the function ideal for creating surfaces with circular symmetry, like cones and paraboloids, in 3D space.

Would you like to explore this concept with additional visual examples or applications in design and geometry?