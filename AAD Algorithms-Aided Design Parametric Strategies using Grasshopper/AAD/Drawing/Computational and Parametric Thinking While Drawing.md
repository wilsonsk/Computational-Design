Draw lines and relationships with the concepts of transformations, algorithms (if, then) and parameters that drive the form. 

Dont aimlessly draw lines, but think mainly. The marks are the expression of a form of thinking. 

Utilize the perspective and isometric techniques, but dont think in those terms.

Think in terms of parameters, relationships, transformations, and computations and then any lines or marks made are just simply expressed in the rules of perspective/isometric but not determined by them.

this relates to [[Functions as Geometric Transformations]]

[[Functions and Motion]]


## [[Functions and Motion|Drawing with Functions]]
Inflection points help one estimate the function of a given curve.
### Curve Fitting
When visually estimating the curves or edges of general objects, you can use several heuristics and rules of thumb to guide your observations and help match a curve’s shape to a function. 
#### 1. Identify Key Points
##### [[Functions and Motion#Inflection Point|Inflection Points]]
Look for points where the curve changes its concavity.
	These points indicate where the curve switches from bending upwards to downwards or vice versa.
##### [[Derivatives#Critical Points|Critical Points]]
Identify local maxima and minima, where the curve reaches its highest or lowest points within a region.
#### 2. Analyze Segments
##### Curve Segmentation
Break down the curve into simpler segments, each of which can be approximated by a basic function (e.g., linear, quadratic, cubic).
##### [[Tangent Line|Tangent Lines]] (i.e. Components of [[Components of Motion#2D Components of the Velocity Vector|Tangent Lines]] and [[Components of Motion#2D Components of the Acceleration Vector|Tangent Lines]])
Observe the tangent lines at various points to understand the local behavior of the curve.
#### 3. Assess the Overall Shape
##### Symmetry
Check if the curve exhibits any symmetry. 
	Symmetrical curves can often be described by simpler functions.
##### Periodic Patterns
Identify if the curve has repeating patterns, suggesting a periodic function (e.g., sine or cosine functions).
#### 4. Matching Curves to Functions
##### Straight Lines
If the curve looks like a straight line, a linear function (y = mx + b) is a good starting point.
##### Parabolic Shapes
If the curve resembles a parabola, a quadratic function (y = ax^2 + bx + c) may be appropriate.
##### S-Shapes
For S-shaped curves, consider cubic functions (y = ax^3 + bx^2 + cx + d) or sigmoid functions.
##### Wave Patterns
For curves that oscillate, trigonometric functions (y = a sin(bx + c) or y = a cos(bx + c)) might be suitable.
#### 5. Visual Heuristics
##### Slope and Curvature
Estimate the slope at different points to understand the steepness and direction of the curve.
##### Uniformity: 
Determine if the curvature is uniform, suggesting a circular or elliptical shape, or if it varies, indicating a more complex function.
### Practical Steps
#### Step 1: Initial Observation
- Sketch the curve or edge.
- Mark key points, such as inflection points, peaks, and valleys.
#### Step 2: Segment Analysis
- Divide the curve into segments where the behavior is relatively consistent.
- For each segment, note whether it appears linear, quadratic, cubic, or follows another recognizable pattern.
#### Step 3: Function Matching
- Start with simple functions and fit them to the segments.
- Adjust the function type if the initial guess does not fit well.
- Use inflection points and the number of bends to guide the choice of function (e.g., one bend for a quadratic, two bends for a cubic).
#### Step 4: Refinement
- Overlay the function on the curve to see how well it matches.
- Adjust parameters (e.g., coefficients in polynomial functions) to improve the fit.
#### Step 5: Validation
- Compare the fitted function to additional points on the curve to ensure accuracy.
### Step 1: Identify Parameters
Parameters are measurable attributes or variables that define the characteristics of the object or curve you are analyzing. For a curve, typical parameters might include:
1. **Control Points**: Key points that define the shape of the curve (e.g., start point, end point, inflection points, maxima, minima).
2. **Curvature**: The degree of bending at different points on the curve.
3. **Length**: The total length of the curve.
4. **Slope/Gradient**: The rate of change of the curve at different points.
5. **Amplitude**: For oscillatory curves, the height from the centerline to the peak.
6. **Frequency**: For periodic curves, the number of cycles per unit length.
### Step 2: Observe Relationships
Understand how these parameters interact with each other. The relationships might be linear, proportional, or more complex.
1. **Direct Relationships**:
    - As the length of the curve increases, the total number of control points might increase.
    - The curvature might be directly proportional to the amplitude in a periodic curve.
2. **Inverse Relationships**:
    - An increase in frequency might lead to a decrease in wavelength.
    - Higher curvature might indicate shorter radii of circles fitting the curve at those points.
3. **Functional Relationships**:
    - Slope and curvature are related through derivatives (the slope is the first derivative of the curve, and curvature is related to the second derivative).
### Step 3: Segment the Curve
Divide the curve into manageable segments where the behavior of the parameters is consistent.
1. **Linear Segments**: Straight lines or parts of the curve with constant slope.
2. **Quadratic/Cubic Segments**: Parabolic or cubic sections with constant curvature or inflection points.
3. **Oscillatory Segments**: Periodic parts of the curve.
### Step 4: Establish Proportionality
Determine the proportionality between parameters within each segment.
1. **Linear Proportionality**:
    - If the segment is linear, the relationship between length and slope is constant.
    - For quadratic segments, the relationship between curvature and the square of the distance might be constant.
2. **Non-linear Proportionality**:
    - For oscillatory curves, the amplitude might be proportional to the sine or cosine of the position.
### Step 5: Calculate Transformations
Estimate how changes in parameters will affect the curve. Use basic mathematical transformations:
1. **Translation**: Shifting the curve without changing its shape.
    - y(x)→y(x)+ky(x) \rightarrow y(x) + ky(x)→y(x)+k, where kkk is the translation amount.
2. **Scaling**: Changing the size of the curve.
    - y(x)→a⋅y(x)y(x) \rightarrow a \cdot y(x)y(x)→a⋅y(x), where aaa is the scaling factor.
3. **Rotation**: Rotating the curve around a point.
    - x′=xcos⁡(θ)−ysin⁡(θ)x' = x \cos(\theta) - y \sin(\theta)x′=xcos(θ)−ysin(θ)
    - y′=xsin⁡(θ)+ycos⁡(θ)y' = x \sin(\theta) + y \cos(\theta)y′=xsin(θ)+ycos(θ)
4. **Reflection**: Flipping the curve across an axis.
    - Reflect across the x-axis: y(x)→−y(x)y(x) \rightarrow -y(x)y(x)→−y(x)
    - Reflect across the y-axis: y(x)→y(−x)y(x) \rightarrow y(-x)y(x)→y(−x)