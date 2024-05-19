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
## Digital Simulation (and Particle Spring Systems)
*"Science is a tool for ideas [...] and it is not only a means to verify structural strength. Science must lead us to discover the optimized geometry for that particular static (or dynamic) condition".* - Sergio Musmeci

Structures that transmit forces through axial compression or tension have an increased capacity to withstand loads with smaller cross sectional areas.
	Traditional form-finding strategies for axially loaded structures include: complex physical models, hanging chain networks, stretched fabrics, soap films etc..
These techniques are difficult and time consuming. 
	As a result, few designers investigated these form-finding potentials. 
		 Traditional form-finding techniques can now be digitally found using particle-spring systems that simulated the physical behavior of deformable bodies.
			 Whereas traditional techniques were difficult to apply, digital simulations allow designers to investigate form, in real time, by updating forces, supports and physical properties.
### Particle-Spring Systems (i.e. PSS)
![[Pasted image 20240502012955.png|400]]
*Above image is a particle spring system that simulates a square membrane anchored at its corners, force vectors are applied to the particles.*

Are a discretization of a continuous model into a finite number of masses, called particles, connected by elastic springs. 

PSS iterative calculations approach an [[Static Equilibrium|equilibrium state]] where the sum of all the forces is zero. 
	The iterative calculations are performed by mathematical solvers. 
###### Mathematical Solvers
Operate iteratively within a main *engine*, meaning every subsequent iteration narrows the position and velocity (magnitude and direction) of particles from the previous step towards an equilibrium solution. 
	This process creates the **illusion** of movement when frames are calculated in a continuous sequence.
#### Main Components
###### [[Points#Idealization in Physics|Particles]]
Each particle in the system is a lumped mass, that changes position and velocity as the simulation evolves.
###### Springs
An elastic linear connection between two particles that behaves according to the **Hooke's Law**.
	"A spring has an initial resting length and a stiffness value, $k$".
###### Hooke's Law
![[Pasted image 20240502201008.png|500]]
States that the force needed to stretch or compress a spring by a distance is linearly proportional to that distance. 
	Displacements or size of the deformation of a body (treated as a spring) is directly proportional to the deforming force or load.

![[Pasted image 20240511000634.png]]
$|\vec{F}| = k \times X$ and $X = {|\vec{F}| \over k}$

Where $\vec{F}$ is an [[Static Equilibrium#Force Representation|applied force]] expressed in Newtons ($N$).

$k$ is a positive constant called, **Stiffness**, usually expressed in $N/cm$.
	The value of $k$ depends on material and cross sectional geometric properties of the elastic body.

$X$ is the change in length or deformation of the body (spring in this case).
	Commonly expressed in $cm$
###### [[Statics Analysis#Forces|Forces]]
Weights and external loads are simulated by [[Statics Analysis#Vector Addition|vectors]] that are applied exclusively to particles.
###### Unary Force
###### Anchor Points
Particles that do not change position during the simulation.
#### Simulation
Once the simulation has started, the particles move from their initial positions until they reach an equilibrium state which is dependent on the initial geometry, the force vectors, and the springs' defined properties.
	Following Hooke's Law, the lower the "stiffness" or $k$ value, the greater the spring elongation. 
		Since particles in this system behave like spherical hinges without the capacity to resist moment forces, equilibrium solutions carry defined loads exclusively through [[Curvature's Role in Stress Distribution#Axial Compression and Axial Tension|axial forces]].
			This is the ideal condition for form-finding strategies.
## Kangaroo (plugin)
A physics based [[#Particle-Spring System|particle-spring system]] engine developed by Daniel Piker.

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
	[[Statics Analysis#Force Vector Representation|Vectors representing forces]] are applied to particles, and the anchor points are assigned. 
##### Kangaroo Engine
[[#Points Idealization in Physics Particles|Particles]], [[#Springs|springs]], [[#Forces|forces]] and [[#Anchor Points|anchor points]] are connected to the Kangaroo Engine in their respective slots. 
	Toggling between *True* and *False* statements using the component, **Boolean Toggle**, to start and stop the simulation.
		While the simulation is running, particles move until an [[Static Equilibrium|equilibrium state]] is reached. 
			For this reason the engine's output can be considered as **[[Dynamics Analysis#Dynamics "Explains" the Causality of a State Change|dynamic]]**.
## Strategies/Patterns (as [[#Digital Simulation (and Particle Spring Systems)]])
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
### Elastic Behavior: [[#Hooke's Law|Hooke's Law]]
Kangaroo's **elastic behavior** follows [[#Hooke's Law|Hooke's Law]] in that "displacements or size of the deformation of a body (in this case, each spring) is directly proportional to the deforming force or load."
###### Springs from Line component
Embeds Hooke's Law.

When the cable reaches an equilibrium state (which is induced by the influences of [[Static Equilibrium#Forms of Forces - Methods of Analyzing Physical Quantities|external forces]]) and resisted by the elasticity of the springs, then the length of each segment increases.  
![[Pasted image 20240510191348.png]]
*For example*
	The demonstrated curve above is discretized into 5 parts, each 2 units in length.
		Six identical unary forces with a magnitude of -20 units in the $z$ direction, are applied to the particles.
			This produces a final curve with an overall length of 10.46 units.
				Therefore, a [[#Deformable Body|deformation]] of $0.46$ units. 
	This deformation is not evenly split among the segments.
		Instead, the springs "closer to the reactions" elongate further. 
			The reason is that these more elongated springs, bear the weight of the other springs.
![[Pasted image 20240510235746.png]]

If a force of $100 N$ is applied to an anchored cable with initial length of $80 cm$ and **stiffness** of $2N/cm$:
	$X = {|\vec{F}| \over k} == X = {100\over2} = 50cm$
![[Pasted image 20240511001303.png]]
If the load is removed, the cable will return to its start length ($80cm$).
###### Rest Length
Refers to the length a cable reaches when loads are removed.
	Which does not always equate to the start length.
###### Damping Constant $c$ 
Aka the Damping Coefficient.
Represents the amount of resistance or friction acting on an oscillating systems.
	I.e. Signifies the contribution of velocity to force. 
		The greater the Damping Constant, the lower the deformation velocity. 

Does not affect the change in length but only the deformation velocity. 

The **time it takes the cable to reach an equilibrium state** depends on the **stiffness $k$** and the **Damping Constant $c$**.
	The higher the $k$ value, the lower the deformation.
![[Pasted image 20240511004427.png]]
The relative algorithm considers the cable to be a single spring. 
	Where the calculated results of the spring's deformation match Hooke's Law.
The **Springs from Line** component embeds the physical characteristics that were discussed in the previous example and the following other important parameters:
###### Connection
Springs are linear, elastic connections.
The connection-input requires lines.
	Any other geometry will yield null results.
Every line's initial length is called the "start length".
###### Stiffness
According to Hooke's Law, the (Stiffness)-input sets the springs' stiffness (i.e. $k$ value).
	The higher the $k$ value, the lower the deformation.
Stiffness is determined by material properties as well as the area of spring's cross-section.
###### Damping
The (Damping)-input influences the deformation velocity, with no influence on the change in length.
	By default the (Damping)-input is set to $10$.
###### Rest Length
The length that a spring endeavors to reach once the loads are removed. 
	The (Rest Length)-input is essential to simulate the behaviors of different materials. 

Three cases can be discerned:
1. **Rest Length = Start Length**:
	- This condition mimics perfectly the elastic behavior and is achieved by connecting the springs (i.e. Lines) to the (Rest Length)-input.
		![[Pasted image 20240512151256.png]]
2. **Rest Length < Start Length**:
	- This condition imitates the effect of pre-tensioning the springs, which **shortens** their length.
	- This simulates the tensile materials that attempt to minimize their length or area.
	- This condition is accomplished in Kangaroo by using the component **Length** to measure the initial springs' length then scaling it by a **Rest Length Factor** that ranges from 0 to 1. 
		![[Pasted image 20240512151507.png]]
3. **Rest Length > Start Length**:
	- This condition replicates the relaxation or lengthening of springs. 
	- This condition is accomplished in Kangaroo by using the component **Length** to measure the initial springs' length then scaling it by a **Rest Length Factor** that ranges between 1 and $N$. 
		![[Pasted image 20240512151631.png]]
- **Upper/Lower Cutoff**:
	- Sets limits for the springs to operate, below or above respectfully. 
		- By default the Upper/Lower cutoffs are set to $0$.
- **Plasticity**:
	- The maximum elastic deformation, as compared to rest length.
### [[Digital Form-Finding#Catenary Curve|Catenary]] Simulation
![[Pasted image 20240518160622.png|300]]
	$\large y=a \times cos h({x \over a}$)
		where:
			- $cosh$ is the [hyperbolic cosine function](https://en.wikipedia.org/wiki/Hyperbolic_functions).
			- $a$ is a constant that dictates the curve's steepness and the distance between its lowest point and the horizontal asymptotes.
			- $x$ and $y$ are the coordinates of points on the curve.

The curve can be calculated by the **Evaluate (Fx)** component.
![[Pasted image 20240518162045.png]]
A Catenary curve can also be drawn by the **Catenary** component, which embeds the equation of a Catenary curve.
	The **Catenary** component requires as inputs:
		- (A)-input: The start point of Catenary curve.
		- (B)-input: The end point of Catenary curve.
		- (L)-input: The length of the Catenary curve.
		- (G)-input: The gravity direction.
![[Pasted image 20240518163941.png]]
##### Catenary Curves and [[#Particle-Spring Systems (i.e. PSS)|Particle Spring Systems]] 
A Catenary Curve is defined as **a curve formed by a perfect flexible, uniformly dense and inextensible cable, suspended from two ends**. 
