---
up:
  - "[[Abstract Concept]]"
related: 
date created: 2024-05-01
---
# Digital Simulation (and Particle Spring Systems)
*"Science is a tool for ideas [...] and it is not only a means to verify structural strength. Science must lead us to discover the optimized geometry for that particular static (or dynamic) condition".* - Sergio Musmeci

Structures that transmit forces through axial compression or tension have an increased capacity to withstand loads with smaller cross sectional areas.
	Traditional form-finding strategies for axially loaded structures include: complex physical models, hanging chain networks, stretched fabrics, soap films etc..
These techniques are difficult and time consuming. 
	As a result, few designers investigated these form-finding potentials. 
		 Traditional form-finding techniques can now be digitally found using particle-spring systems that simulated the physical behavior of deformable bodies.
			 Whereas traditional techniques were difficult to apply, digital simulations allow designers to investigate form, in real time, by updating forces, supports and physical properties.
## Particle-Spring Systems (i.e. PSS)
![[Pasted image 20240502012955.png|400]]
*Above image is a particle spring system that simulates a square membrane anchored at its corners, force vectors are applied to the particles.*

Are a discretization of a continuous model into a finite number of masses, called particles, connected by elastic springs. 

PSS iterative calculations approach an [[Static Equilibrium|equilibrium state]] where the sum of all the forces is zero. 
	The iterative calculations are performed by mathematical solvers. 
###### Mathematical Solvers
Operate iteratively within a main *engine*, meaning every subsequent iteration narrows the position and velocity (magnitude and direction) of particles from the previous step towards an equilibrium solution. 
	This process creates the **illusion** of movement when frames are calculated in a continuous sequence.
#### Main Components
###### [[Points#Idealization in Physics]]
Each particle in the system is a lumped mass, that changes position and velocity as the simulation evolves.
###### Springs
An elastic linear connection between two particles that behaves according to the **Hooke's Law**.
	"A spring has an initial resting length and a stiffness value, $k$".
###### Hooke's Law
![[Pasted image 20240502201008.png|500]]
States that the force needed to stretch or compress a spring by a distance is linearly proportional to that distance. 
###### Forces
Weights and external loads are simulated by [[Structural Analysis#Vector Addition|vectors]] that are applied exclusively to particles.
###### Anchor Points
Particles that do not change position during the simulation.
#### Simulation
Once the simulation has started, the particles move from their initial positions until they reach an equilibrium state which is dependent on the initial geometry, the force vectors, and the springs' defined properties.
	Following Hooke's Law, the lower the "stiffness" or $k$ value, the greater the spring elongation. 
		Since particles in this system behave like spherical hinges without the capacity to resist moment forces, equilibrium solutions carry defined loads exclusively through [[Curvature's Role in Stress Distribution#Axial Compression and Axial Tension|axial forces]].
			This is the ideal condition for form-finding strategies.
## Kangaroo (plugin)
A physics based particle-spring system engine developed by Daniel Piker.

Enables designers to interact with form through particle-spring simulations in real time. 
There are two interactive methods:
###### 1. Direct Interaction
Includes the manipulation of anchor points, forces and spring properties.
###### 2. Parametric/Associative Interaction
Anchor points, forces, and spring properties can be parametrically linked to other parts of the 3D model.
	*For example*, the anchor points can be defined as the end points of a set of lines whose position is defined by another part of the algorithm. 
### Kangaroo Workflow
![[Pasted image 20240504141138.png]]
Relies on the same set of rules and operations for [[Meshes#Low Nodal Models (e.g., Single Digital Chains)|low nodal models]], such as single digital chains, as [[Meshes#High Nodal Models (e.g., Multi-Supported Membranes)|high nodal models]] such multi-supported membranes.
##### [[Large Scale Projects#Surface Discretization|Discretization]]
A deformable body (i.e. a fabric membrane or flexible cable) is created by discretizing NURBS-geometries and subsequently processing the resulting geometry with a particle-spring system.
###### Deformable Body
A deformable body is **a physical body that deforms, meaning it changes its shape or volume while being acted upon by an external force**. 
	The relative position of any points on a deformable body can change. 
		They are the opposite of rigid bodies and are defined by their elements.

Kangaroo requires that NURBS-curves are converted to lines and NURBS-surfaces are converted to meshes (i.e. points and lines). 
	Kangaroo cannot process NURBS-surfaces and NURBS-curves. 
		The main components used for discretization are hosted within the Extract panel of Weaverbird. 
			We can also find useful components within Grasshopper standard tabs or Kangaroo tab.
##### Particle-Spring System
After a geometry has been discretized, lines are converted into springs and points are converted into particles, using specific components hosted within the Kangaroo toolbar.
	[[Structural Analysis#Force Vector Representation|Vectors representing forces]] are applied to particles, and the anchor points are assigned. 
##### Kangaroo Engine
Particles, springs, forces and anchor points are connected to the Kangaroo Engine in their respective slots. 
	Toggling between *True* and *False* statements using the component, **Boolean Toggle**, to start and stop the simulation.
		While the simulation is running, particles move until an equilibrium state is reached. 
			For this reason the engine's output can be considered as **dynamic**.
## Example Simulations
### Cable Simulation
![[Pasted image 20240505005158.png]]
Simulates the behavior of a flexible elastic cable, that is suspended between two end points and subjected to loads imposed by self weights. 

#### Procedure

1. Set a horizontal line referenced in Rhino using the **Curve** container component. 
2. **Discretization**: 
	![[Pasted image 20240505005633.png|600]]
	-  The initial geometry is then discretized by splitting (**Shatter** component) the set line at division points, via **Divide Curve** component. 
	- The **N-input** of the **Divide Curve** component sets the number of divisions. 
		- The greater the number of division points the greater the final deformation. 
			- These division points are the particles in the system where force is applied or restraints are set. 
2. **Particle-spring system:** 
	![[Pasted image 20240505084542.png|600]]
	- The **Shatter** component outputs a series of unique lines that are converted into springs using the **Springs From Line** component, which generates the system's springs.
	- The **(S) output** of the **Shatter** component stored in the container component **Line**, is connected to the **(Connection) input** and the **(Rest Length) input** of the **Springs From Line** component. 
	- The **(P) output** of **Divide Curve** component is connected to the (P) input of the **Unary Force** component -- which applies a force vector to every input point or particle according to a direction (F) input. which takes a vector with specified magnitude. 
	- Ancho points are defined as the end points of the initial curve.
	- The **Kangaroo Engine** component collects the outputs of the **Springs from Line** component and the **Unary Force** component in the "Force Objects" input - ==which must be set to flatten==.
