---
up:
  - "[[Algorithms Aided Design MOC]]"
related:
  - "[[Printable Objects]]"
date created: 2024-04-18
---
# Digital Fabrication
Fabrication has always been in a crucial relationship with design (industrial, architecture).
The manufacturing techniques, assembly processes, and materials often prompt shifts in design. 

*For example*: 
The introduction of structural steel fabrication, influenced the design of structures, facilitated new formal ideas.
But also required new understanding and consideration in detailing and pre fabrication.
- I.e. The introduction of a new component within the design process, influenced a new the production, marginalizing handcraft and pushing the designer into an essential role within the build process. 

## Assemblies
Refers to the construction or arrangement of various parts or components that come together to form a complete object or system. 

Assemblies involve the consideration (i.e. design decisions) of fit and functional relationships between different components. 
	The manufacturing techniques, assembly procedures, and materials can prompt significant shifts in a design.
		I.e. The interrelationships between components dictates the overall design and functionality of an outcome.  
## Before the Digital Revolution
The management of complexity within building projects, involved the designer:
	Decomposing components into their fundamental components.
	Studying part to whole assembly strategies, via scale models and drawings. 
		The scale models and subsequent construction drawings were then transferred to suppliers and contractors to interpret and fabricate the assembly components. 

This process was constrained to working with orthogonal structures, lacking the ability to handle complex shapes.
	With few notable exceptions:
		Jorn Utzon, Heinz Isler, Antoni Gaudi, etc.

The digital revolution removed this constraint, by integrating design output directly with fabrication. 
## Digital Revolution
### The first stage:
Controls the project by generating digital, tri-dimensional model (3D model) as a primary source.
	From which all necessary bi-dimensional (2D) components (plans, sections, elevations, details) can be generated from via computer interpretation. 
		I.e. The building processes are directly interpreted from this 3D primary source. 
#### Informed Digital Fabrication
This digital controlling source is called **Informed digital fabrication**:
	Which itself is a framework or workflow where digital data directly drives manufacturing equipment to form various parts such as (component geometries, shapes, fabrication and assembly).
		I.e. CAD (Computer-aided design) to CAM (Computer-aided manufacturing).

#### CNC
Computer Numerical Control:
	Refers to the use of computer in driving and controlling a machine's movements.
		For example: a milling cutter, a lathe, a laser or waterjet cutter, etc.

CNC processes are an informed digital fabrication, and directly link 3D geometry to the final components.
	Removing the need for and thus production of drawings.
		The use of traditional drawings is now limited to merely aiding in the assembly of components. 
			Drawings can be all together bypassed by printing assembly instructions directly on components.
				Future implications are instructions that are provided in the form of coded instruction sets. 

Informed digital fabrication (i.e. the automated production of components) improves accuracy and makes complexity and thus managing it, not complicated. 
	Where a complex operation will have the same level of machining difficulty as a simple operation. 
##### Future Implications
###### Rapid Prototyping
An additive fabrication technique in which material is deposited in layers to print a component. 
	Facilitating the generation of a physical object from a 3D model. 
## Fabrication Techniques
Can be sorted according to processes and materials.
### (2D) Bi-dimensional Cutting 
2D fabrications transform planar sheets of: aluminum, steel, plywood acrylic, etc. of varying thickness into tri-dimensional assemblies. 

**Planar sheets** can be used to form geometries using techniques such as: stacking, faceting, etc. 
**Flat sheets** can be *bent* to form complex [[Gaussian Curvature#Developable Surfaces|developable geometries]], or geometries with [[Gaussian Curvature#Null Gaussian Curvature|null Gaussian Curvature]]. 
#### Bi-dimensional Cutting-Based Processes
##### CNC Laser cutters
A focused laser at a specified power and cutting speed, are used to burn or melt material. 
	The cutting speeds and power are set according to a material's dimensional and physical properties. 
		Laser cutting is not able to be used for every material; aluminum sheets will reflect the laser. 
###### Laser:
**L**ight **A**mplification by **S**timulated **E**mission of **R**adiation.
##### CNC Plasma cutters
Use focused stream of super heated gas or plasma to cut materials.
	Widely used for cutting of steel and aluminum. 

##### CNC Waterjet cutter
Use a focused jet of water combined with an abrasive substance. 
	The major advantage of the Waterjet is that is does not **create *heat-affected zones* where the molecular structure is modified**. 
		Can be used on a wide range of materials from steel to wood. 

### Subtractive Techniques
Create objects by **removing** material.
Subtractive methods can achieve the same output of cutting machines with the **added ability** to **specify the Z depth of a cut**.

Solid blocks of materials from wood to polystyrene can be milled to cave described geometry.
	Not all geometry can achieved using 3 axis milling.
		And in many cases objects must be decomposed into several parts to prevent **undercutting**. 
###### Undercutting
Refers to a scenario where part of a material or object is cut from underneath or inside, creating an overhand or a recess that is difficult to reach with traditional machining tools like drills or mills. 
	I.e. Creating features that are not accessible or cannot be machined directly from the tools' approach angle. 
		*Examples*: Internal cavities, deep recesses, or complex geometries that recede under other surfaces. 

![[Pasted image 20240418220410.png|400]]
#### CNC Milling machines
A tooling process that uses a cutter head to remove material from a sheet or block of material. 
	Mills vary in their size and depth capacity as well as the number of axis that the cutter head can be manipulated. 
These machines are informed by digital geometry which is used to describe the tooling paths. 

The most commons machines are:
	2D:
		Mills cut at a specified Z depth similar to cutting machines. 
	2.5D:
		Mills that operate in 3 axes but only perform operations in 2 axes simultaneously.
	3D:
		Mills that perform operations in all 3 axes simultaneously.
![[Pasted image 20240418222929.png]]
Less common:
	5 axis mills:
		Move in 4 or more axes to create custom parts with limited tooling restrictions.
![[Pasted image 20240418223029.png]]
*Aura, by Zaha Hadid Architects (design team F. Wirz and M. Lanza).*
	Created using a 6 axis CNC machine using polyurethane foam as material to mill.

##### Hot-wire foam cutters
Use an electronically heated wire to cut polystyrene foam or similar materials. 
	Several different types of hot-wire cutters exist.
		From wires able to cut on a single plane to cutters able to cut on multiple planes. 
This method is used to quickly generate tri-dimensional (3D) shapes. 
##### Robotic arms
Used to facilitate other fabrication techniques:
	Holding a milling cutter head or heated wires.
	Grasping and folding, forming, etc.
The implications are new design possibilities only enabled by the high degree of flexibility provided by the robotic arm.

### Additive Techniques
Additive Manufacturing (AM) creates tri-dimensional (3D) objects though an accumulation of successive layers. 
Enables designers to fabricate objects that are impossible to make using subtractive techniques at a small scale.
	Such as branching shapes, complex twisting, moving parts with intricate details.
#### Optimization
Additive techniques revolutionize the area of optimization.
Where traditionally, optimization has been linked to simplifying fabrication techniques such as: 
	Cutting operations, complexity through similarity, describing developable surfaces or planar panels, etc. 
Optimization of additive techniques involves finding the optimal shape which meets a prescribed set of performance targets.
	Such as minimally using material.

Additionally, advanced form-finding strategies such as **[[Topology Optimization|topology optimization]]**, are becoming increasingly important in design (architecture, industrial design). 

![[Pasted image 20240418232947.png]]
*Example of Topology Optimization; driving the material distribution within the volume of the truss.*
#### Deposition Paths
AM is defined by describing **deposition paths**. 

Created by slicing a digital model (developed using 3D software- like Rhino) into layers with a defined slice thickness or resolution. 
	The contours describe how material is deposited, layer by layer. 
#### AM Process
1. Creation of a digital 3D model.
	- A printable model is required to meet the criteria of a printable object.
2. Conversion of the digital model into a code based machine-readable format.
3. 3D printing the object. 
##### 3D Printing Format
The most commonly used 3D printing format is Standard Tessellation Language (STL).
	An interface developed by 3D Systems
##### STL Conversion
An STL conversion triangulates an initial tri-dimensional model and outputs the coordinates of each vertex according to the right-hand rule. 
	The number of triangulation iterations can be equated to the smoothness of the final model.
		Meaning the more triangles the smoother the model. 
The output can be described in ASCII and Binary. 
	Binary is the more common language because of the smaller file dimensions. 
#### Most Common 3D Printing Techniques
##### Stereolithgraphy (SLA)
Developed in 1983 by Charles Hull.
An SLA printer consists of four main elements:
	1. A vat containing a photosensitive liquid form resin.
	2. A mobile perforated-platform.
	3. A UV beam.
	4. A computer that controls booth the beam and the platform.
![[Pasted image 20240418231725.png|300]]
The platform is initially positioned on the top of the vat, just below a thin layer of resin.
As the UV beam strikes the resin, the resin selectively solidifies and a layer if formed.
	Which is as defined by one layer of the **[[#Deposition Paths|sliced]]** digital model.
The platform is then lowered the distance of one layer to print the next slice.
This process continues until all the sections are created.
After the object is completed, it is rinsed with a liquid solvent and baked in a UV oven to cure the plastic. 
Resin that is not solidified remains in the initial liquid form.
Un-solidified liquid resin is unable to support overlying parts.
	For this reason, it is often necessary to create support structures.
SLA printers can produce very=high-resolution objects, but are slow and expensive.
##### Selective Laser Sintering (SLS)
Developed in 1986 by Carl Deckard. 
Use a high powered laser to selectively fuse powdered particles of plastic, metals, ceramic, glass, etc. 
Consists of four main elements:
	1. A laser.
	2. A powder cartridge.
	3. A roller.
	4. A fabrication platform where the laser traces a bi-dimensional section of the object.
		- Where the material is sintered together. 
![[Pasted image 20240418232159.png|400]]
The platform is then lowered the distance of one layer thickness and subsequently the roller deposits new material from the powder cartridge to be sintered forming the next layer. 
The process continues until the part is completed. 
SLS does not require support structures since the sintering parts are surrounded and thus supported by the non-fused powder.
##### Fuse Deposited Modeling (FDM)
Developed in 1998 by Scott Crump.
Form geometry by melting plastic filament and depositing thin layers additively on a platform. 
The FDM printers require support structures for overhanging parts.
Some FDM printers can print multiple materials, in this way supports can be printed in a material that is easy to remove; such as water soluble filament.
FDM printers use two types of plastic:
	1. ABS.
	2. PLA, an organic version of ABS.
