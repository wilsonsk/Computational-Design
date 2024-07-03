# [[Mapping|Mapping]] as Geometric Transformations

relates to [[Computational and Parametric Thinking While Drawing]]... and [[Functions and Motion]]
The parametric relationships (equations) in parametric design are not necessarily linear; they can be linear, quadratic, cubic, or even more complex, depending on the design requirements and the nature of the relationships between parameters. The choice of these equations is influenced by the visual and functional transformations they represent, rather than being a mere coincidence. Here’s how different types of equations can come into play:

### Linear Equations

Linear equations are often used when the relationship between two parameters is straightforward and proportional. For example:

- **Height vs. Width**: If the width of a table increases proportionally with its height, a linear equation like W=kHW = kHW=kH (where kkk is a constant) might be used.
- **Scaling**: If a design element scales uniformly, the relationship between the original and new sizes can be described linearly.

### Quadratic Equations

Quadratic equations are used when the relationship involves squared terms, often to represent area or to achieve a parabolic shape:

- **Curved Surfaces**: The equation of a parabola y=ax2+bx+cy = ax^2 + bx + cy=ax2+bx+c can describe the profile of a curved surface.
- **Structural Analysis**: When analyzing the bending of beams or deflection of materials, quadratic relationships can describe how stress or strain varies with position.

### Cubic Equations

Cubic equations are used for more complex curves and volumes:

- **Bezier Curves**: Cubic Bezier curves, which are widely used in computer graphics and design, are defined by cubic equations.
- **Volume Relationships**: When dealing with volumes and more complex geometric transformations, cubic equations can accurately represent the relationships.

### Non-Linear Equations

Non-linear equations (exponential, logarithmic, sinusoidal, etc.) are used for even more complex transformations:

- **Growth Patterns**: Exponential equations can model growth patterns seen in nature, such as the branching of trees or the expansion of populations.
- **Wave Forms**: Sinusoidal equations are used to describe wave-like patterns, such as the undulating form of a canopy or the oscillations in a dynamic structure.

### Choosing Equations Based on Visual Transformations

The choice of equation type is guided by the desired visual and functional outcomes:

- **Visual Aesthetics**: To achieve certain aesthetic qualities, such as smooth transitions, flowing curves, or intricate patterns, designers select equations that naturally produce these effects.
- **Functional Requirements**: Functional aspects, such as structural integrity, load distribution, and ergonomic comfort, also influence the choice of equations. For example, a quadratic equation might be chosen to ensure that a surface has the right curvature for strength.

### Examples in Design

1. **Bezier Curves**:
    
    - **Equation**: P(t)=(1−t)3P0+3(1−t)2tP1+3(1−t)t2P2+t3P3P(t) = (1-t)^3 P_0 + 3(1-t)^2 t P_1 + 3(1-t) t^2 P_2 + t^3 P_3P(t)=(1−t)3P0​+3(1−t)2tP1​+3(1−t)t2P2​+t3P3​
    - **Use**: This cubic equation defines a Bezier curve, used for smooth and controllable curves in design and animation.
2. **Parabolic Arches**:
    
    - **Equation**: y=ax2y = ax^2y=ax2
    - **Use**: Used in architecture for arches and bridges to distribute weight evenly.
3. **Sinusoidal Waves**:
    
    - **Equation**: y=Asin⁡(Bx+C)y = A \sin(Bx + C)y=Asin(Bx+C)
    - **Use**: Used to create wave-like structures and patterns, adding dynamic visual interest to designs.

### Conclusion

The choice of parametric relationships is intentional and based on the specific visual and functional needs of the design. Whether linear, quadratic, cubic, or more complex, the equations are selected for their ability to represent the desired transformations accurately. Understanding the mathematical foundations allows designers to manipulate forms with precision and creativity, achieving both aesthetic and practical objectives.
- - - 
## Linear Transformations

Linear equations represent transformations where changes in parameters result in proportional changes in the design elements.

- **Scaling**: If you scale a design element, such as resizing a table proportionally, the relationship is linear. For example, doubling the height and width of a table maintains its proportions.
    - **Equation**: W=kHW = kHW=kH, where kkk is a constant that defines the proportionality.

### Quadratic Transformations

Quadratic equations represent transformations where the relationship involves squared terms, creating parabolic or hyperbolic shapes.

- **Curvature**: A parabolic curve in architecture, like the profile of an arch, can be represented by a quadratic equation.
    - **Equation**: y=ax2+bx+cy = ax^2 + bx + cy=ax2+bx+c, where aaa, bbb, and ccc define the specific curve.

### Cubic Transformations

Cubic equations represent more complex transformations involving cubic terms, which can create S-shaped curves or control the flow of a surface in three dimensions.

- **Bezier Curves**: Used in graphic design and animation, cubic Bezier curves provide precise control over the shape of the curve.
    - **Equation**: P(t)=(1−t)3P0+3(1−t)2tP1+3(1−t)t2P2+t3P3P(t) = (1-t)^3 P_0 + 3(1-t)^2 t P_1 + 3(1-t) t^2 P_2 + t^3 P_3P(t)=(1−t)3P0​+3(1−t)2tP1​+3(1−t)t2P2​+t3P3​, where P0P_0P0​, P1P_1P1​, P2P_2P2​, and P3P_3P3​ are control points.

### Non-Linear Transformations

Non-linear equations, such as exponential, logarithmic, or trigonometric, represent more complex transformations that can describe growth patterns, oscillations, and other natural phenomena.

- **Exponential Growth**: Used to model phenomena like population growth or the expansion of a network.
    
    - **Equation**: y=ekxy = e^{kx}y=ekx, where kkk defines the rate of growth.
- **Sinusoidal Waves**: Used to create wave-like structures and patterns.
    
    - **Equation**: y=Asin⁡(Bx+C)y = A \sin(Bx + C)y=Asin(Bx+C), where AAA is the amplitude, BBB is the frequency, and CCC is the phase shift.

### Applying Transformations in Design

To illustrate how these transformations apply to design, let’s revisit the table example:

**Step-by-Step Example: Generating a Table Design**

1. **Observation and Decomposition**:
    
    - Identify the geometric components: rectangular tabletop and four legs.
2. **Define Parameters**:
    
    - Tabletop length (LLL), width (WWW), thickness (TTT), leg height (HHH), leg thickness (ttt), and distance between legs (ddd).
3. **Establish Relationships**:
    
    - **Linear Relationship**: The leg thickness might increase linearly with the leg height for stability.
        - **Equation**: t=kHt = kHt=kH, where kkk is a proportional constant.
    - **Quadratic Relationship**: If the legs have a slight curve, the profile can be quadratic.
        - **Equation**: y=ax2+bx+cy = ax^2 + bx + cy=ax2+bx+c, describing the curvature of the leg.
4. **Implement Transformations**:
    
    - Use these relationships to generate the geometry.
        - For a leg height of 75 cm, if k=0.05k = 0.05k=0.05, then t=0.05×75=3.75t = 0.05 \times 75 = 3.75t=0.05×75=3.75 cm.
        - If the leg has a parabolic curve, set a=0.01a = 0.01a=0.01, b=0b = 0b=0, and c=0c = 0c=0, so the leg profile is y=0.01x2y = 0.01x^2y=0.01x2.
5. **Iterate and Experiment**:
    
    - Change LLL, WWW, and HHH to see how the table’s form changes.
    - Adjust aaa, bbb, and ccc to refine the leg’s curve.

### Visualization and Practical Application

Using a 3D modeling tool like Rhino and Grasshopper:

1. **Set Up Sliders** for LLL, WWW, TTT, HHH, and ttt.
2. **Create Geometry** based on parametric equations.
3. **Visualize Transformations** by adjusting the sliders and observing the changes in real-time.

### Conclusion

Parametric relationships indeed represent transformations. By selecting appropriate equations—linear, quadratic, cubic, or more complex forms—you can control how parameters influence the geometry and behavior of your design. This approach allows for precise and flexible design exploration, ensuring that the resulting forms are both aesthetically pleasing and functionally sound.
- - - 
- Yes, derivatives are often used in parametric and computational design to represent rates of change, optimize designs, and analyze dynamic behavior. Here are some ways derivatives are applied in these contexts:

### 1. Optimization

Derivatives are crucial in optimization problems, where the goal is to find the maximum or minimum values of a function.

- **Gradient Descent**: A method used to minimize functions by iteratively moving towards the steepest descent as defined by the negative of the gradient.
    - **Example**: Optimizing the shape of a bridge for minimum material use while maintaining structural integrity. The derivative of the cost function with respect to design parameters guides the optimization process.

### 2. Analyzing Curvature

Derivatives are used to analyze the curvature of surfaces and curves, which is important for aesthetics and functionality.

- **Curvature Analysis**: The second derivative of a curve provides information about its concavity or convexity.
    - **Example**: In designing an ergonomic chair, the curvature of the seat and backrest can be analyzed using second derivatives to ensure comfort.

### 3. Motion and Dynamics

In dynamic systems, derivatives describe how a system evolves over time.

- **Velocity and Acceleration**: The first derivative of position with respect to time gives velocity, and the second derivative gives acceleration.
    - **Example**: In kinetic architecture, derivatives of the position function describe how parts of a building move and accelerate over time.

### 4. Sensitivity Analysis

Derivatives are used to understand how sensitive a design is to changes in parameters.

- **Sensitivity Analysis**: The partial derivative of a function with respect to a parameter shows how changes in that parameter affect the output.
    - **Example**: In a parametric model of a skyscraper, the sensitivity of structural stability to changes in the thickness of load-bearing columns can be analyzed using derivatives.

### 5. Slope and Tangent Lines

Derivatives provide the slope of tangent lines to curves, useful in constructing and modifying shapes.

- **Tangent and Normal Vectors**: The first derivative at a point on a curve gives the direction of the tangent, and the normal vector can be derived from it.
    - **Example**: In car design, the derivative of the body contour curve is used to ensure smooth transitions and aerodynamic efficiency.

### Practical Example: Using Derivatives in Parametric Design

Let's consider a practical example involving the design of a parametric curve, such as a Bezier curve.

1. **Bezier Curve Definition**:
    
    - A cubic Bezier curve is defined by four control points P0,P1,P2,P3P_0, P_1, P_2, P_3P0​,P1​,P2​,P3​.
    - The curve is given by: P(t)=(1−t)3P0+3(1−t)2tP1+3(1−t)t2P2+t3P3P(t) = (1-t)^3 P_0 + 3(1-t)^2 t P_1 + 3(1-t) t^2 P_2 + t^3 P_3P(t)=(1−t)3P0​+3(1−t)2tP1​+3(1−t)t2P2​+t3P3​
2. **First Derivative (Velocity)**:
    
    - The first derivative of P(t)P(t)P(t) with respect to ttt gives the tangent vector at any point on the curve: P′(t)=−3(1−t)2P0+3(1−t)2P1−6(1−t)tP1+6(1−t)tP2−3t2P2+3t2P3P'(t) = -3(1-t)^2 P_0 + 3(1-t)^2 P_1 - 6(1-t)t P_1 + 6(1-t)t P_2 - 3t^2 P_2 + 3t^2 P_3P′(t)=−3(1−t)2P0​+3(1−t)2P1​−6(1−t)tP1​+6(1−t)tP2​−3t2P2​+3t2P3​
    - This represents the direction and rate of change of the curve at each point.
3. **Second Derivative (Acceleration)**:
    
    - The second derivative of P(t)P(t)P(t) with respect to ttt gives the curvature of the curve: P′′(t)=6(1−t)P0−12(1−t)P1+6(1−2t)P2+6tP3P''(t) = 6(1-t) P_0 - 12(1-t) P_1 + 6(1-2t) P_2 + 6t P_3P′′(t)=6(1−t)P0​−12(1−t)P1​+6(1−2t)P2​+6tP3​
    - This helps in analyzing how sharply the curve bends.
4. **Applications in Design**:
    
    - **Smoothness and Aesthetics**: Ensure the curve transitions smoothly by analyzing the first and second derivatives.
    - **Structural Analysis**: Use derivatives to understand stress distribution along curved elements in structures.
    - **Dynamic Behavior**: For elements that move along a path defined by a Bezier curve, the derivatives provide velocity and acceleration profiles necessary for controlling motion.

### Visualization

Using tools like Rhino and Grasshopper, you can visualize and manipulate these derivatives:

1. **Define Control Points**: Create sliders for control points P0,P1,P2,P3P_0, P_1, P_2, P_3P0​,P1​,P2​,P3​.
2. **Compute the Curve**: Use Grasshopper to compute and display the Bezier curve.
3. **Visualize Derivatives**: Add components to compute and visualize the first and second derivatives at various points on the curve.

### Conclusion

Derivatives play a significant role in parametric and computational design, enabling precise control over shapes, optimization of structures, analysis of dynamic behavior, and sensitivity analysis. By understanding and applying derivatives, designers can create more efficient, functional, and aesthetically pleasing designs.