# Computational Methodology

[[Elemental Building Blocks#Points Point as the Fundamental Building Block of Form|Point as the Fundamental Building Block of Form]]

[[Elemental Building Blocks#Transformations Measures the change between two Points points *P(x,y)* and *P'(x',y')* Transformations of Points as the Fundamental Operation of Generation of Form|Transformations of Points as the Fundamental Operation of Generation of Form]]
## Involves the following four steps:
1. Decomposition:
	1. Breaking something into smaller parts.
2. Pattern Recognition:
	1. Look for similarities, trends, and patterns.
3. Abstraction:
	1. Focus on what’s important and ignore what is unnecessary.
4. Algorithmic Thinking:
	1. Create step-by-step instructions to solve the problem.

## Base Principles:
1. [[Elemental Building Blocks]]
2. [[Data Trees#Data Structures|Data Structures]]
3. [[building-complexity]]
4. [[unitization]]
## Decomposition
Very general method: Parametric/Computational Analysis
1. Observe system/object.
2. Abstract the system/object being observed.
	1. Decomposition of the sets of geometries.
3. Identify and extract the critical parameters.
4. Implement the critical parameters into the computational design model

Computational Methodology:
	1. Starting point: [[decomposition]] of the end design goal (many to one).
		2. intentionality
		3. reverse engineering the problem, to breakdown complexity
			1. [[analysis-sketches]]
				1. element feature exploration
					1. [[Surface Analysis|Features]]:
						1. Simplest geometrical features we can "see"
					2. [[Parameters]]:
						1. Main dimensions and setting out parameters
					3. [[Elemental Building Blocks|Components]]:
						1. Ideas for potential geometrics we might use
	2. Storyboarding:
		1. Ordering the sketches into an approximation with a direction (ie rough story)
			1. This acts as the Guiding Map + [[structure]]

### Abstracting a Geometry aka [[Rationalizing a Geometry]]
Refers to the process of simplifying complex geometric forms into a series of manageable, quantifiable, and often repeatable elements that can be more easily analyzed, constructed, or fabricated.
- The abstract mindset or perspective in this context involves viewing architectural forms not as monolithic wholes but as assemblages of discrete, parametrically defined components.

## Identifying the Most Fundamental Parameters of a Geometry
To intuitively decompose an object down to its fundamental parameters just from observation, it's  effective to start with generator curves and directrices, and then distill further down to the points translated to form these curves. 

This method aligns well with parametric design principles, where the simplest geometric and transformative operations serve as the building blocks for more complex forms. Here’s a more structured approach to help visualize and implement this concept:

1. **Identify the Simplest Geometric Features**: Begin by observing the simplest visible forms and shapes of the object. This could be basic geometries like lines, curves, or circles. In architectural terms, these might be the structural or design outlines.
    
2. **Identify Transformations**: Once you've identified these basic forms, consider how they are transformed or manipulated to achieve the final design. Transformations could involve translations, rotations, or scaling of points and lines. For example, a curve might be defined by a series of points (control points in parametric terms) that are manipulated to form a spline or bezier curve.
    
3. **Decompose to Points and Relationships**: Break these curves or shapes further down into their constituent points. Consider how these points are related or how they influence the overall geometry through their positioning and movement. This is crucial because it defines how the object can be manipulated or parameterized.
    
4. **Parametrize the Relationships**: Convert these observations into parametric terms. For example, if a curve is defined by points that are equidistant or follow a mathematical rule (like a sine wave), these relationships can be parametrized. The parameters might be the distances, angles, or mathematical functions governing their layout.
    
5. **Reconstructing from Parameters**: Using the identified parameters and their relationships, reconstruct the object parametrically. This involves setting up parametric equations or functions that describe each component's placement and transformation based on the underlying parameters.
    
6. **Iterative Refinement**: Finally, refine your parametric model by adjusting the parameters and observing how changes affect the overall design. This iterative process is key in fine-tuning the design to meet specific aesthetic or functional requirements.
## Identifying Key Parameters of the Geometry
### 1. **Core Functionality and Purpose Identification**

- **Direct Observation**: Start by observing the primary function and purpose of the design. Ask, "What is this design fundamentally trying to achieve?"
- **Intuitive Simplification**: Use intuition to strip the design down to its most basic functional requirements. Consider which elements are absolutely necessary for the design to fulfill its purpose.

### 2. **Environmental Interaction Analysis**

- **Contextual Factors**: Consider how the design interacts with its environment. This includes physical factors (like wind, light, and gravity) and social factors (like user flow and interaction).
- **Adaptive Elements**: Intuitively identify which parts of the design might need to adapt to these factors. These become prime candidates for parameterization.

### 3. **Structural Considerations**

- **Load Path Visualization**: Mentally visualize how forces travel through the design. Elements in this load path are key to the design's structural integrity and thus important parameters.
- **Material and Method Constraints**: Think about the materials and construction methods to be used. Consider which geometrical or dimensional aspects are constrained by these choices.

### 4. **Aesthetic and Spatial Experience**

- **Dominant Visual Themes**: Identify the dominant visual themes or experiences intended in the design. Parameters that control these aspects can greatly affect the design's aesthetic appeal.
- **User Interaction and Flow**: Consider how users will move through or interact with the space. Parameters affecting paths, viewpoints, and user interfaces are crucial.

### 5. **Modularity and Repetition**

- **Repetitive Elements Identification**: Look for patterns or repetitive elements in the design. These often signify underlying parameters that dictate the repetition rate, spacing, or scaling.
- **Modularity as a Parameter**: For modular designs, the dimensions and interfaces of modules are key parameters for ensuring fit and function.

### 6. **Flexibility and Adaptability**

- **Change Anticipation**: Consider which aspects of the design are most likely to need changes during further development. These areas should be parameterized for ease of adjustment.
- **Scalability**: Identify dimensions or elements that might need to scale up or down. Parameters controlling these aspects can provide flexibility in adapting the design to unforeseen requirements.

### Developing an Intuitive Heuristic:

- **Reflective Practice**: Regularly engage in reflective practice, analyzing past design projects to understand which parameters ended up being key to successful outcomes.
- **Cross-Disciplinary Inspiration**: Look to other fields (e.g., biology, engineering) for principles that dictate form and function. Nature, for instance, optimizes structures and forms efficiently, guiding intuition towards key functional parameters.
- **Iterative Experimentation**: Use parametric tools to experiment with different parameters on smaller scale projects. This hands-on approach can sharpen intuition about which aspects of a design are most impactful when varied.

By integrating these strategies, designers develop an intuitive heuristic for identifying key variables that balance the logical with the creative, ensuring that parametric models are both functionally effective and aesthetically meaningful. This heuristic is personal and evolves with experience, becoming a powerful tool in the designer's toolkit for tackling complex design challenges.
## Rational Geometry Vs Non-Rational Geometry

[[Grids|Grids]] which define edges, edges which are then transformed, and a surface that is generated between the original edges and the new transformed edges
## Form Finding
Form finding refers to the process of discovering the shape of a physical structure through the exploration of its equilibrium under specific conditions and forces. It's a concept rooted deeply in both architecture and engineering, where the optimal form of a structure is determined not solely by aesthetic preference but by how it naturally responds to physical forces, such as gravity, tension, compression, and environmental factors.

This process often results in shapes that are efficient, structurally sound, and sometimes mimic natural forms, reflecting the principle that form follows function. The idea is to allow the structure's material and environmental conditions to guide the determination of its shape, leading to designs that are inherently optimized for their intended purpose.

