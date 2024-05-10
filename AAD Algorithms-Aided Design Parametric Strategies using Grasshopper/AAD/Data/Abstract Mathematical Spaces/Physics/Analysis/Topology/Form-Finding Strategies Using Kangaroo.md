---
up:
  - "[[Topology Optimization]]"
related:
  - "[[Digital Form-Finding]]"
  - "[[Topology]]"
  - "[[Surfaces]]"
date created: 2024-05-10
---
# Form-Finding Strategies Using Kangaroo
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
## Strategies/Patterns (as [[Digital Simulation|Digital Simulations]])
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
3. **Particle-spring system:** 
	![[Pasted image 20240505084542.png|600]]
	- The **Shatter** component outputs a series of unique lines that are converted into springs using the **Springs From Line** component, which generates the system's springs.
	- The **(S) output** of the **Shatter** component stored in the container component **Line**, is connected to the **(Connection) input** and the **(Rest Length) input** of the **Springs From Line** component. 
	- The **(P) output** of **Divide Curve** component is connected to the (P) input of the **Unary Force** component -- which applies a force vector to every input point or particle according to a direction (F) input. which takes a vector with specified magnitude. 
	- Anchor points are defined as the end points of the initial curve.
	- The **Kangaroo Engine** component (i.e. **KanagrooPhysics** component) collects the outputs of the **Springs from Line** component and the **Unary Force** component in the "Force Objects" input - ==which must be set to flatten==.
		- The end points of the initial curve are fed into the (AnchorPoints) input.
		- By default the simulation influences only the particles, which can velocity while the simulation is attempting to reach equilibrium. 
		- To visualize the simulation of the cable seeking equilibrium, the output of the **Shatter** component is fed into the (Geometry) input of the **KangarooPhysics** component.  
4. To start or stop the simulation, a **Boolean Toggle** component (in the (SimulationReset) input where start = *true*, stop = *false*) and a **Timer** component are connected to the **KangarooPhysics** component.  
	- Alternatively, if the component is double clicked a contextual panel will appear with a set of buttons: stop, play, pause.
	- Once the simulation is started the particles move in the direction of the force vectors which are restrained by the elastic-linear springs properties. 
		- The cable's geometry changes several times until it reaches an equilibrium state.
			![[Pasted image 20240510164437.png]]
		- If changes are made to the initial geometry or to the discretization process the simulation is required to be reset and then started again, to visualize the influence of the changes.
			- Other parameters, such as the Unary Force direction and magnitude, and the location of the anchor points can be changed during the simulation. 
		- The position of the constraints can be changed manually by setting the anchor points from Rhino instead of relying on the End Points component. 
			![[Pasted image 20240510164753.png|300]] 
			![[Pasted image 20240510164808.png|400]]
			- Once the simulation has started the position of the anchor points can be changed "manually": 
				- The simulation will react to the change and, once again, seek equilibrium.
					- *Manual interaction with the model can lead to errors if the points are not returned to their original position before stopping and starting a new simulation.*
						- *If the simulation is run without returning the anchor points to their original position the physics engine will not recognize how to restrain the model.*
			- To add additional or new anchor points, points can be set from Rhino or calculated within Grasshopper. 
				- **Anchor points must be always positioned at particles**.
					- *For instance*, an anchor point drawn in the middle of a spring will have no influence.
#### Strategy: Continuity 
![[Pasted image 20240510164730.png|400]]
Kangaroo's inputs are defined as points, lines or meshes. Kangaroo's output is similarly defined as the same kind of geometries.

An elastic cable can be simulated by connecting the (ParticlesOut) output to the (V) input of the **NURBS Curve** component, defining an interpolated curve through the points. 
	This strategy can be useful to achieve continuity; 
		However, it can lead to physically incorrect results since the Nurbs-curve acts rigidly around point B, which is impossible since particles act as spherical hinges, without [[Non-Concurrent Systems#Moment Capacity|moment capacity]].
### Elastic Behavior: [[Digital Simulation#Hooke's Law|Hooke's Law]]
