---
up:
  - "[[Digital Fabrication]]"
related:
  - "[[Printable Objects]]"
  - "[[Modeling Object for Cutting Operations]]"
date created: 2024-04-27
---
# Large Scale Projects
Large scale fabrications or objects have have potential additional technical, structural, or functional considerations, which require additional techniques to satisfy their articulation.

The fabrication of large scale objects usually involves the assembly of individually (i.e. smaller, more manageable pieces for practical fabrication) fabricated parts to [[#Ease of Assembly and Load Transfer|transfer loads]]. 
## Surface Discretization
Surface discretization involves dividing a complex surface into simpler, manageable parts. 
	In architectural and structural engineering, this is often required when the surface is too complex to be constructed from a single piece of material. 

By breaking it down into smaller segments, these segments can be individually fabricated and then assembled. [[#Meshes Defining Meshes by Triangulation Triangulation of a Surface|Discretization]] helps in simplifying the modeling, analysis, and fabrication processes.
	I.e. By discretizing a surface, you transform a complex geometry into a series of smaller [[#Planar Panels|planar panels]] or sections that can be individually manufactured.

The process of surface discretization is often achieved through planar panels, specifically [[#Meshes Defining Meshes by Triangulation Triangulation of a Surface|triangulation of a surface]].
### Planar Panels
Used as an approach to approximating a surface. 
Are commonly used in the surface discretization of complex architectural facades primarily because they help address several practical needs:
###### Manufacturing and Material Efficiency
- **Simplification of Fabrication**: Using planar panels simplifies the fabrication process. Curved panels, while aesthetically pleasing, require more complex, often custom molds and manufacturing techniques which can significantly increase cost and production time.
- **Cost Reduction**: Flat panels can be produced more economically and in larger quantities. They often require less specialized machinery and can frequently be fabricated using standard industrial processes.
###### Ease of Installation
- **Standardization**: Planar panels can be standardized, which facilitates easier and quicker installation. Standardization also allows for easier replacement or repair of panels if necessary.
- **Modularity**: Flat panels lend themselves well to modular construction techniques, where pre-fabricated panels are assembled onsite. This can speed up construction times and reduce onsite labor requirements.
###### Structural Performance
- **Predictability**: The structural behavior of flat panels is well-understood and can be easily predicted and modeled using standard engineering practices. This predictability helps in ensuring the structural integrity of the building.
- **Load Bearing**: Planar panels, especially when triangulated, can efficiently bear loads and transfer them to the building’s structural framework. This makes them a practical choice for ensuring the stability and safety of large-scale structures.
###### Aesthetic Flexibility
- **Versatility in Design**: Despite their simplicity, planar panels can be arranged in various configurations to create visually interesting and dynamic facades. They can be used to form patterns, rhythms, and textures that enhance the building’s visual appeal.
- **Surface Treatment Options**: Planar panels offer flexibility in terms of surface treatments and finishes. Materials can vary widely from metals to composites, each capable of receiving a range of finishes that can complement the overall architectural design.
###### Sustainability Considerations
- **Material Usage**: Using flat panels often results in less waste during production compared to custom-shaped pieces. The efficiency in material use is a crucial factor in sustainable building practices.
- **Recyclability and Reusability**: The more standardized the component, the easier it is to recycle or reuse. Planar panels often meet these criteria better than more complex forms.
### [[Meshes#Defining Meshes by Triangulation|Triangulation]] of a Surface
Triangulation is a specific type of surface discretization (i.e. [[#Planar Panels|planar panels]]). It involves breaking down a surface into triangles. 
	This is particularly common in computer graphics and computational design because triangles are the simplest polygon, and any surface in 3D space can be represented as a collection of triangles. 
		This makes rendering and analyzing the geometry computationally efficient. Triangulation allows for the approximation of curved surfaces using flat, two-dimensional facets that are easier to work with both in software and physical fabrication processes.
###### Ease of Assembly and Load Transfer: 
Triangulation, is particularly valuable because triangular elements are inherently very stable. 
	When a surface is broken down into triangles, each triangular panel can be designed to effectively transfer and distribute structural loads. 
		This is crucial for the stability and integrity of large-scale structures.
###### Cost and Material Efficiency:
The uniformity that can be achieved through techniques like triangulation **allows for the reuse of molds** and standardization of parts, which significantly reduces manufacturing costs. 
*For example*:
	Using planar panels of the same dimensions simplifies the construction process and can make the assembly more systematic and less prone to error.
###### Structural Integrity:
Each fabricated part, whether triangular or another shape derived from discretization, can be optimized to handle specific loads. 
	When assembled, these parts work together to distribute the structural load across the object, enhancing the overall strength and stability of the structure.
		These methods are essential in computational design to handle complex geometries efficiently, especially when aiming to simplify the construction and reduce costs while maintaining the structural and aesthetic integrity of the original design.
### Challenges Introduced by [[#Planar Panels|Planar Panels]]
The main challenge of building a freeform facade has traditionally been to approximate a surface using **planar panels** of the same dimensions. 
	Essentially, freeform designs often include complex, non-linear, and curved surfaces that don't naturally align with flat, straight-edged panels.
##### Geometric Approximation
- **Complexity of Curvature**: Freeform facades often involve complex curvatures that are difficult to accurately represent with flat panels. 
	- Planar panels can only approximate these curves by segmenting them into flat facets, which may not capture the smoothness and continuity of the original design.
- **Visual Aesthetics**: The approximation of curved surfaces with flat panels can lead to a faceted appearance, where the smooth flow of the surface is interrupted by the edges of the panels. 
	- This can detract from the intended aesthetic effect of the design.
##### Structural Integrity
- **Load Distribution**: Curved surfaces naturally distribute loads differently compared to flat surfaces. 
	- When these curves are approximated with flat panels, it can alter the way loads are transferred through the structure, potentially requiring additional supports or reinforcement.
- **Joint Stress**: The points where flat panels meet to approximate a curve can experience higher stresses, as the flat nature of the panels can concentrate forces at the joints rather than distributing them smoothly across a curve.
##### Construction and Assembly
- **Alignment and Tolerance**: Fabricating and assembling a large number of flat panels to form a complex shape requires high precision. 
	- Misalignment can lead to gaps or uneven surfaces, and even small errors in measurement or fabrication can be magnified across the facade.
- **Increased Complexity in Installation**: The installation process can become more complex and time-consuming due to the need to precisely align and attach multiple flat panels to create the illusion of a continuous curved surface.
##### Cost Implications
- **Increased Material Usage**: To approximate curves, more panels may be required than if the surface were to be constructed with inherently curved materials. 
	- This can lead to increased material costs.
- **Specialized Fabrication**: Although using standardized planar panels can reduce individual unit costs, the overall cost might increase due to the complexity of the design and the need for precise engineering and assembly.
##### Aesthetic Limitations
- **Segmentation of the Surface**: The aesthetic appeal of a smooth, continuous surface is often segmented by the linear boundaries of flat panels, which may not be desirable in all design contexts.
- **Reflection and Light Dynamics**: The way light and shadows play on a curved surface differs significantly from how they interact with a faceted surface composed of flat panels. 
	- This can affect the visual perception of the facade at different times of the day and under different lighting conditions.
### Disadvantages to Triangulation of a Surface
Increased weight of the support structure and the complexity of each structural node.
## Two Strategies for Fabrication
There are two important strategies for the fabrication of large scale objects, that are currently being researched and developed both by academia and industry. 
### 1. Computational Approach
This approach is used to address the issues of [[#Meshes Defining Meshes by Triangulation Triangulation of a Surface|triangulation]] to achieve [[#Surface Discretization|surface discretization]].
	This approach bypasses the utilization of triangular, planar, panels.

Computational techniques enable the development of [[Meshes#Planar Quadrangular Panels (i.e. PQ Meshes)|planar quad panels (i.e. PQ Meshes)]] from an arbitrary freeform surface.

Computational approaches operate within the traditional fabrication environment.
#### Planar Quad Panels (i.e. PQ Meshes)
Refer to meshes composed of **Planar Quadrilateral** panels, each panel in a PQ Mesh is a quadrilateral, meaning it has four sides and four vertices, which can be all equal or of varying lengths.
##### Key Characteristics of PQ Meshes
1. **Geometry**: The quadrilateral shape of each panel provides versatility in filling out and approximating complex freeform surfaces. Unlike triangles, quadrilaterals can be more flexible in aligning with the natural flow of certain architectural forms.
2. **Structural Connectivity**: Quadrilateral panels share edges with adjacent panels, and the typical connections at each vertex involve four panels. This arrangement can provide a robust mesh structure, supporting the stability and integrity of the overall architectural form.
3. **Panel Uniformity**: In many cases, the use of quadrilaterals allows for a more uniform mesh configuration, which can simplify the design and computation processes. It also aids in achieving a more cohesive aesthetic look, particularly where the flow of the surface needs to be smooth without sharp breaks.
4. **Ease of Fabrication**: While quadrilaterals provide a bit more complexity than triangles, they still lend themselves to efficient manufacturing processes, especially when the panels can be standardized or when only a few different shapes are needed.
5. **Surface Approximation**: Quadrilaterals, especially when arranged in a mesh (grid), are effective at approximating curved surfaces by slightly adjusting the angles and lengths of the sides to conform to desired curvatures. This flexibility makes them highly useful in architectural designs where large, smooth surfaces are needed.
##### Benefits in Construction
- **Aesthetic Versatility**: PQ Meshes allow for a range of aesthetic expressions, from rigid, geometric facades to more fluid, dynamic surfaces, depending on how the quadrilateral panels are sized, shaped, and arranged.
- **Structural Benefits**: The ability to create large, connected meshes with quadrilaterals aids in distributing loads across the structure. This distribution can be finely tuned by adjusting the mesh configuration to better handle specific structural demands.
- **Economic Efficiency**: Utilizing PQ Meshes can optimize the use of materials and reduce the need for bespoke molds in fabrication, as quadrilaterals can often be cut from standard sheets of material with minimal waste.
- **Design Flexibility**: Designers can manipulate the individual panels in a PQ Mesh to follow complex architectural forms more closely than is possible with more rigid panel shapes. This flexibility allows for the creation of innovative designs that are both visually appealing and structurally sound.
- **Simplification of Installation**: Although each panel connects at four points, the overall design of a PQ Mesh can be engineered to simplify installation. By planning the mesh to align with structural supports and to minimize the variability in panel shapes, the assembly of the facade or architectural element can be streamlined.

And Computational techniques are also able to develop, under certain conditions, **hexagonal panels** (i.e. P-Hex Meshes).
#### Hexagonal Panels (i.e. P-Hex Meshes)
Refer to planar panels arranged in a hexagonal grid that are used to approximate the surfaces of freeform geometries in architectural designs.

These panels are shaped as hexagons—six-sided polygons—and are used in constructing facades, roofs, or other architectural elements where a curved or complex surface needs to be covered.

Simplify the fabrication of the underlying structure as each node of a hexagon connects just three rods. 
![[Pasted image 20240428173829.png|400]]
##### Key Characteristics of P-Hex Meshes:
- **Geometry**: Each panel is a hexagon, which provides unique geometric properties. Hexagons have six vertices and six sides of equal length, forming a regular polygon that tessellates perfectly, meaning they can fill a plane with no gaps, which is ideal for covering surfaces efficiently.
- **Structural Connectivity**: A significant advantage of hexagonal panels in architectural applications is their connectivity. Each hexagon shares edges with six neighboring hexagons, creating a high degree of interconnection that enhances structural stability. This connectivity distributes loads more evenly across the structure.
- **Node Simplification**: Each intersection point (node) where corners of the hexagons meet typically connects only three panels. This simplification at nodes can make the structural framework easier to design and construct compared to more complex junctions that might occur with other shapes.
- **Aesthetic Appeal**: Hexagonal patterns are visually appealing and are often used for their aesthetic value as much as their structural qualities. The uniformity and symmetry of the hexagonal arrangement can enhance the architectural design, offering a distinctive appearance.
- **Surface Approximation**: Like other planar panels used in computational approaches, hexagonal panels can approximate curved surfaces. Although each panel is flat, the overall effect can suggest curvature through the geometric layout of the panels.
##### Benefits in Construction:
- **Efficient Coverage**: Due to their ability to tessellate without gaps, hexagonal panels can cover surfaces efficiently, minimizing waste and potentially reducing material costs.
- **Uniform Load Distribution**: The hexagonal structure can handle loads effectively due to the even spread of force through the interconnected mesh.
- **Ease of Fabrication**: While individual hexagonal panels are more complex than square or rectangular panels, their uniformity allows for repeatability in manufacturing processes, which can be cost-effective at scale.
- **Flexibility in Design**: Hexagonal meshes can adapt to various architectural forms, allowing designers to work with complex shapes and surfaces while maintaining an orderly and coherent panel system.
#### [[Surface Strategies#To **identify** developable surfaces|Developable]] Strategies
Developable strategies play an important role in the construction of freeform objects. 

Several algorithms have been developed in order to find developable surfaces or sets of surfaces to approximate a freeform geometry. 

Since every developable surface is a [[Notion of Surface Curvature#**Ruled Surfaces**|ruled surface]], **a set of straight lines can always be found**.
	**These lines** can **become the axis of linear beams**, ultimately simplifying the support structure.
### 2. Innovative Fabrication Approach
Focus on developing new fabrication strategies.

*For example*: Inventor and engineer Enrico Dini is successfully testing additive techniques to print large scale objects.
	His procedures are encouraging designers to rethink the conception and optimization of structures. 