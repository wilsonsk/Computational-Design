---
up:
  - "[[Computational Methodology]]"
related:
  - "[[Parameters]]"
  - "[[Elemental Building Blocks]]"
date created: 2024-04-07
---
# Rationalizing a Geometry

Refers to the process of simplifying complex geometric forms into a series of manageable, quantifiable, and often repeatable elements that can be more easily analyzed, constructed, or fabricated.
- The abstract mindset or perspective in this context involves viewing architectural forms not as monolithic wholes but as assemblages of discrete, parametrically defined components.


### ## Intuitive Heuristic for Abstracting a Geometry
The process of mentally reverse-engineering an object or understanding its construction through geometric operations and transformations.

Many complex 3D forms can indeed be conceptualized, analyzed, and constructed from transformations of 2D entities.

1. Identify the **Profile Curve** (i.e. The Generator):
	**Define 2D Profiles**: 
	- The first step often involves defining the 2D profiles or curves that serve as the foundational elements of the form. These profiles capture the essential contours or cross-sections of the 3D shape.
	
	- A geometry with a [[Surface Creation#^18bb28|constant cross section of the original profile curve]] - that is, a profile curve that moves along a **linear** path:
		- Was constructed via a [[Surface Creation#Extrusion (aka Extrude Operation)|Translational Extrusion]].
	- A geometry with a profile curve that moves along a [[Surface Creation#^d14a44|complex or curve/path (i.e. has variable cross sections of the original profile curve)]]:
		- Was constructed via [[Surface Creation#Translational (NURBS) Surface Generation|Translational Surface Generation]]  or a [[Surface Creation#Rotational (NURBS) Surface Generation|Rotational Surface Generation]].
1. Identify the Transformation:
	**Transformation Operations**: 
	- By applying various transformation operations (extrusion, rotation, lofting, sweeping) to these 2D profiles, one can generate the complex 3D form. Each operation offers a different method for manipulating the 2D curve into a three-dimensional object.
	- **Surface Directionality**:
	    - Determine if the surfaces have a primary direction (e.g., mostly vertical or horizontal). This can hint at the direction of the profile curve’s movement during generation.
	    - Surfaces wrapping around an axis point towards rotational generation, while surfaces extending in one direction suggest translational generation.
	- **Surface Continuity**:
	    - Smooth, continuous surfaces often result from NURBS-based generations. Look for signs of curvature continuity to distinguish between simple extrusions and more complex surface generations.
1. Analyze Faces/Surfaces:
2. Decompose and Extract Compositional Elements of the Faces/Surfaces:
3. Identify Parameters of the Extracted Components. 





### 2. Analyze Faces/Surfaces:




### 3. Decompose and Extract Compositional Elements of the Faces/Surfaces:

- **Break Down Complex Forms**:
    
    - Identify simpler geometric forms that compose the complex geometry. This step involves mentally or digitally "slicing" the geometry to reveal its basic compositional elements.
    - Recognizing these elements helps in understanding the assembly logic and potential modularization for rationalization.
- **Segmentation for Modular Analysis**:
    
    - Consider how the geometry can be segmented into repeatable modules. This is particularly useful for geometries that hint at a generative repetition or pattern.

### 4. Identify Parameters of the Extracted Components:

- **Defining Dimensional Parameters**:
    - Assign parameters to the dimensions of the extracted components, such as lengths, widths, heights, and radii. Consider how variations in these parameters might have generated different instances of the geometry.
- **Establishing Relational Parameters**:
    - Look for relational parameters that define the position or orientation of components relative to each other (e.g., spacing, angles, offsets).
- **Functional Parameters**:
    - Some components may have parameters defined by their function (e.g., window sizes for light requirements, column sizes for load-bearing). Identifying these can aid in rationalizing form based on functional optimization.

### Implementing the Heuristic:

1. **Visualization Tools**:
    
    - Use sketches, diagrams, or computational design software to visualize the identified profile curves, surfaces, and components. This helps in abstracting the geometry for analysis.
2. **Computational Modeling**:
    
    - Employ parametric or computational modeling tools to recreate the geometry based on identified generative processes and parameters. Experiment with modifying parameters to observe effects on the overall form.
3. **Optimization and Rationalization**:
    
    - Leverage optimization algorithms or manual adjustments to refine the parameters for material efficiency, structural integrity, or aesthetic objectives, aiming for a rationalized design that balances form and function.

By following these steps with an intuitive and analytical mindset, you can effectively rationalize complex geometries, making them more accessible for analysis, fabrication, or further design exploration. This approach not only simplifies the geometry but also retains its essential characteristics and functionality.
## General Heuristic
### 1. Identifying the Geometric Basis of the Form

- **Cataloging Basic Shapes**: Begin by identifying the basic shapes that make up the form. This includes recognizing primary geometric forms such as planes, cubes, spheres, cylinders, and more complex surfaces like splines, NURBS (Non-Uniform Rational B-Splines), or meshes.
- **Understanding the Composition**: Document how these basic shapes are combined or intersect to create the overall form. Pay attention to unions, intersections, subtractions, and any deformations applied to these shapes.

### 2. Component Breakdown

- **Segmentation**: Divide the form into logical segments or modules that repeat or vary across the design. This might be influenced by structural considerations, aesthetic patterns, or functional zones.
- **Hierarchy Establishment**: Determine a hierarchy of components, identifying primary structural or spatial elements and secondary supporting elements. This step is crucial for understanding the relational importance of different parts of the form.

### 3. Geometric Relationships and Dependencies

- **Mapping Relationships**: Map out spatial and structural relationships between components, such as adjacency, alignment, nesting, and support.
- **Identifying Dependencies**: Note any dependencies between geometric components, where the modification of one may necessitate changes in another. This includes proportional relationships, alignments, or spacing requirements.

### 4. Functional Analysis

- **Identifying Functional Zones**: Break down the form into areas based on function, understanding how geometric components contribute to or define these zones.
- **Assessing Form-Function Integration**: Assess how the geometry of components is influenced by functional requirements, including accessibility, circulation, and spatial hierarchies.

### 5. Structural Analysis (If Applicable)

- **Load Path Identification**: Identify primary load-bearing components and their paths through the form. This includes understanding how forces are transferred through the structure.
- **Material Considerations**: Note any geometric implications of material choices, such as span limitations, joint requirements, or fabrication constraints.