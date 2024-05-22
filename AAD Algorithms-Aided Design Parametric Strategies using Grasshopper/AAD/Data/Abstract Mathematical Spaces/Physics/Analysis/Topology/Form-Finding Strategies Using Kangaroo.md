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

Structures that transmit forces through axial [[Curvature's Role in Stress Distribution#Compression (i.e. squeezing stress)|compression]] or [[Curvature's Role in Stress Distribution#Tension (i.e. stretching stress)|tension]] have an increased capacity to withstand loads with smaller cross sectional areas.
	Traditional form-finding strategies for axially loaded structures include: complex physical models, hanging chain networks, stretched fabrics, soap films etc..
These techniques are difficult and time consuming. 
	As a result, few designers investigated these form-finding potentials. 
		 Traditional form-finding techniques can now be digitally found using particle-spring systems that simulated the physical behavior of deformable bodies.
			 Whereas traditional techniques were difficult to apply, digital simulations allow designers to investigate form, in real time, by updating forces, supports and physical properties.
### [[Concurrent Systems#Particle Spring Systems|Particle-Spring Systems]] (i.e. PSS)
![[Pasted image 20240502012955.png|400]]
*Above image is a particle spring system that simulates a square membrane anchored at its corners, force vectors are applied to the particles.*

Are a discretization of a continuous model into a finite number of masses, called particles, connected by elastic springs. 

PSS iterative calculations approach an [[Static Equilibrium|equilibrium state]] where the sum of all the forces is zero. 
	The iterative calculations are performed by mathematical solvers. 
###### Mathematical Solvers
Operate iteratively within a main *engine*, meaning every subsequent iteration narrows the position and velocity (magnitude and direction) of particles from the previous step towards an equilibrium solution. 
	This process creates the **illusion** of movement when frames are calculated in a continuous sequence.
#### Main Components
##### [[Points#Idealization in Physics|Particles]]
Each [[Bodies#Particles in Static Equilibrium Translational Equilibrium Translational Equilibrium in Concurrent Systems|particle in the PSS system]] is a lumped mass, that changes position and velocity as the simulation evolves.
	Where all forces meet at a single point on the particle.
##### Springs
An elastic linear connection between two particles that behaves according to the **Hooke's Law**.
	"A spring has an initial resting length and a [[#Stiffness|stiffness]] value, $k$".
##### Oscillating System
An oscillating system in this context means that the springs, due to their elasticity, can undergo oscillations (back-and-forth movements) when displaced from their equilibrium position. 
	This is a common behavior in mechanical systems with mass and elasticity, where:
		- **[[Newton's First Law#Mass|Mass]]**: The particles have mass, which means they have [[Newton's First Law#Inertia|inertia]] and can [[Newton's Second Law#Acceleration|accelerate]] or decelerate.
		- **Elasticity**: The springs can stretch and compress, generating restoring forces that can cause the particles to move back and forth.
###### Elasticity
Refers to the ability of a material to return to its original shape and length after the force causing the deformation is removed.
	It describes how a material behaves when deformed. 
		An elastic material can stretch or compress and then return to its original form once the force is removed.
			 The degree to which a material can stretch and then return to its original shape without permanent deformation is its elasticity.
###### Extensibility
Refers to the property of a material or system that allows it to increase in length when a force (tension) is applied.
- **Extensible Springs in Simulation**: When using particle-spring systems to simulate a catenary curve, the springs connecting the particles are typically extensible. 
	- This means they can stretch and compress, altering their length in response to forces.
		- This behavior can lead to oscillations and deviations from the ideal catenary shape.
###### Implications for [[#Catenary Curves and Particle-Spring Systems (i.e. PSS) Particle Spring Systems|Catenary Curves]]
When trying to simulate an inextensible catenary curve using a particle-spring system, the springs’ ability to stretch and compress introduces oscillations. 
###### Inextensibility
Refers to the behavior of maintaining a constant length; the shape is purely due to gravity and endpoint constraints.
- **Springs are not perfectly inextensible**: They have some elasticity, which means they can stretch and thus allow the particles to oscillate.
- **Inextensible Cable**: An inextensible cable is one that cannot be stretched. Its length remains constant regardless of the forces applied to it.
	- This is a key characteristic of a true catenary curve, where the shape is determined by gravity and the constraints at the endpoints, without any stretching of the material.
- **Extensible Springs**: Can stretch or compress, meaning the length of the spring changes when forces are applied.
- **Simulation Deviations**: The ability of the springs to stretch means that the simulated curve might not perfectly match the theoretical catenary curve, especially under dynamic conditions or when high stiffness is not achieved.
- **Deviations from the ideal catenary shape**: These oscillations can cause the simulated curve to differ slightly from the true shape of an inextensible catenary curve, especially if the springs oscillate before settling into a final shape.
##### Hooke's Law
![[Pasted image 20240502201008.png|500]]
States that the force needed to stretch or compress a spring by a distance is linearly proportional to that distance. 
	Displacements or size of the deformation of a body (treated as a spring) is directly proportional to the deforming force or load.
		*See* [[Concurrent Systems#Springs|springs in concurrent systems]] *for more info on springs in static systems.*

![[Pasted image 20240511000634.png]]
$|\vec{F}| = k \times X$ and $X = {|\vec{F}| \over k}$

Where $\vec{F}$ is an [[Static Equilibrium#Force Representation|applied force]] expressed in Newtons ($N$).

$k$ is a positive constant called, **Stiffness**, usually expressed in $N/cm$.
	The value of $k$ depends on material and cross sectional geometric properties of the elastic body.

$X$ is the change in length or deformation of the body (spring in this case).
	I.e. $\LARGE x$ is actually $\LARGE \triangle x$ the displacement of the spring relative to [[Curvature's Role in Stress Distribution#Compression (i.e. squeezing stress)|compression]] or [[Curvature's Role in Stress Distribution#Tension (i.e. stretching stress)|tension]].
	Commonly expressed in $cm$
##### [[Statics Analysis#Forces|Forces]]
Weights and external loads are simulated by [[Statics Analysis#Vector Addition|vectors]] that are applied exclusively to particles.
##### Unary Force
A unary force (in the context of Grasshopper's Kangaroo physics engine) is essentially a [[Concurrent Systems|concurrent force]] applied uniformly to all [[Bodies#Particles in Concurrent Systems Concurrent Systems|particles]] in a system.
	It ensures that each particle experiences the same magnitude and direction of force.
		 This type of force is useful for simulating effects like gravity, where every particle needs to be influenced equally, regardless of its position or other properties​​​​​​.

A unary force is a type of force in Grasshopper's Kangaroo physics engine that applies a uniform force vector to each particle in a system. 
	This force acts on individual particles rather than on pairs of particles or elements.
		 *For example*, when simulating gravity, a unary force can be used to apply a downward force on each particle, ensuring that gravity affects the entire system uniformly.
  
  The magnitude of this force can be set according to the specific requirements of the simulation, such as the weight of the particles or other external forces​​​​​​.
##### Anchor Points
Particles that do not change position during the simulation.
#### Simulation
Once the simulation has started, the particles move from their initial positions until they reach an equilibrium state which is dependent on the initial geometry, the force vectors, and the springs' defined properties.
	Following Hooke's Law, the lower the "stiffness" or $k$ value, the greater the spring elongation. 
		Since particles in this system behave like spherical hinges without the capacity to resist moment forces, equilibrium solutions carry defined loads exclusively through [[Curvature's Role in Stress Distribution#Axial Compression and Axial Tension|axial forces]].
			This is the ideal condition for form-finding strategies.
###### Frame
A "frame" typically refers to an individual iteration or time step in a dynamic simulation.
	Each frame represents a single step in the calculation of the positions and interactions of particles or other elements in the system. 

The simulation progresses frame by frame, updating the positions and states of all elements based on the forces applied and the constraints set in the model.

For instance, in a particle-spring system simulation using Kangaroo, the positions of particles are updated at each frame based on the forces acting on them, such as springs and unary forces. 
	This process continues until the system reaches a state of equilibrium or the simulation is stopped. 
		The "timer" component in Grasshopper can control the rate at which these frames are processed, effectively setting the speed of the simulation​​​​ .
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
A deformable [[Bodies|body]] (i.e. a fabric membrane or flexible cable) is created by discretizing NURBS-geometries and subsequently processing the resulting geometry with a particle-spring system.
###### [[Bodies#Deformable Bodies|Deformable Body]]
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
## [[#Digital Simulation (and Particle Spring Systems)|Digital Simulations]] Strategies/Patterns for [[Concurrent Systems#Particle Spring Systems|PSS]]
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
#### Elastic Behavior: [[#Hooke's Law|Hooke's Law]]
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
#### [[Digital Form-Finding#Catenary Curve|Catenary]] Simulation
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
#### Catenary Curves and [[#Particle-Spring Systems (i.e. PSS)|Particle Spring Systems]] 
A Catenary Curve is defined as **a curve formed by a perfect flexible, uniformly dense and inextensible cable, suspended from two ends**. 
	Therefore, the curve must comply with four conditions:
###### Four Conditions of Catenary Curves
1. To be suspended by its end points.
	The cable is hanging freely from two fixed points.
2. To be perfectly flexible.
	The cable can bend without any resistance or stiffness, meaning it can freely assume the shape dictated by the forces acting upon it.
3. To be uniformly dense.
	The cable has a consistent mass per unit length, ensuring that its weight distribution is uniform.
4. To be inextensible.
	"Inextensible" means that the cable or curve cannot be stretched. 
		An inextensible cable maintains a constant length regardless of the forces applied to it.
			Ensuring that its shape is solely determined by its weight and the forces acting on it (like gravity), rather than by any elasticity or stretching.

These [[#Oscillating System|conditions are not entirely met]] by the deformable linear-curve.
	When simulating catenary curves using particle-spring systems, these conditions need to be approximated. 
		Particle-spring systems consist of particles connected by springs that can stretch and compress. 
			While this method can approximate a catenary curve, the springs typically have some elasticity (they can stretch), meaning they are not truly inextensible.
				 This means that the simulated curve may differ slightly from an ideal catenary curve because it does not perfectly satisfy the inextensibility condition.
	In fact, even if a high [[#Stiffness|stiffness value]] is set, the springs will not be [[#Implications for Catenary Curves and Particle-Spring Systems (i.e. PSS) Particle Spring Systems Catenary Curves|inextensible]]. 
		As a result, the simulation will generate a curve that is slightly different from a catenary curve. 
![[Pasted image 20240519161820.png]]

To more closely approximate a Catenary curve, an arc can be used as a starting geometry, described using the component **Arc 3Pt**, through a set of three points. 
	Then the measured arc-length is set equal to the length of the desired catenary curve.
![[Pasted image 20240519170217.png]]
##### Steps
![[Pasted image 20240519170610.png]]
1. Initial Geometry
	Is an arc with a length of 20 units drawn through three points: A, B, C.
2. Discretization
	The arc is then divided using the **Divide Curve** component with the (N)-input set to 50.
		Which yields 51 equidistant points.
	A polyline is created through the resulting points and exploded into segments by the **Explode** component, in order to return 50 lines. 
		The lines are then converted into springs, each initially measuring 20 (i.e. arc length) /50 (i.e. 50 steps) = 0.4 units. 
			![[Pasted image 20240519171114.png]]
3. Particle-Spring System
	The output of the **Explode** component is connected to the (Connection)-input of the **Springs From Line** component, after passing through a **Line** container component. 
		==To achieve [[#Inextensibility|inextensibility]] of the cable, the rest length is set such that the rest length < start length using a multiplier factor of 0.995, and a (Stiffness)-input set to 7000 units.== 
	Gravity loads are applied to each particle using the component **Unary Force** in the Z-direction with a magnitude of -1.
		The resulting vectors are connected to the (Force objects)-input of the component **Kangaroo**.
			Set points A and B, are combined into a single list via **Merge** component and connected to the (AnchorPoints)-input of the **Kangaroo** component.
				![[Pasted image 20240519171841.png]]
	When the simulation is initiated, the segmented arc moves in the negative Z direction, taking the form of a Catenary Cable. 
		The calculated polyline complies with the [[#Four Conditions of Catenary Curves|four conditions]] of the Catenary definition. 
			The segments change minimally in length from their start length (0.4 units) after the simulation.
				![[Pasted image 20240521150914.png]]
	So far the **Unary Force component (Force)-input value** (which represents self [[Newton's First Law#weight|weight]] ([[Newton's First Law#mass|mass]] * [[Newton's First Law#Gravity|gravity]])), has been set arbitrarily.
		More accurately, the **[[#Unary Force|Unary Force]] component (Force)-input value** should be set by:
			Dividing the cable's total weight by the numbers of particles. 
				![[Pasted image 20240521182217.png]]
					The above image is of two Catenary Curves, each with starting points on respective initial freeform [[Notion of Surface Curvature#Frame|frames]].
### Membrane Simulation
The behavior of a regular flat membrane anchored at four corner points and subjected to gravity loads can be simulated using [[Concurrent Systems#Particle Spring Systems|particle-spring systems]].
##### Membrane
In the context of structural engineering and computational design, refers to a thin and flexible [[Surfaces|surface]] that can carry loads primarily through [[Curvature's Role in Stress Distribution#Tensile Structures|tensile forces]].
	Membranes are often used in simulations to represent materials like fabric, rubber and any other flexible materials that can undergo large deformations without significant bending stiffness. 
###### Characteristics of Membranes
1. **Thin and Flexible**: Membranes are characterized by their minimal thickness compared to their other dimensions, allowing them to bend and flex easily.
2. **Tensile Structures**: They carry loads primarily through tension, not compression or bending. This makes them ideal for structures like tents, sails, and certain types of roofs.
3. **Anchoring**: Membranes are typically anchored at their edges or at specific points to define their shape and maintain tension.
4. **Simulation in Grasshopper**: In Grasshopper's Kangaroo plugin, membranes are often simulated using a mesh representation where vertices are treated as particles and edges as springs. This setup allows the simulation of the flexible behavior of membranes under various forces, such as gravity​​.
###### Simulation Process
- **Discretization**: A continuous surface (e.g., a NURBS surface) is converted into a mesh of points and edges to simulate its behavior.
- **Spring System**: The edges of the mesh act as springs that can stretch and compress, representing the flexible nature of the membrane.
- **Anchor Points**: Specific points on the membrane are fixed or anchored to simulate how the membrane is held in place in a real-world scenario​​.
###### Form-Finding Techniques
- **Hanging Models**: A traditional form-finding technique where a physical membrane model is hung and allowed to settle under gravity, forming a shape purely in tension. This shape can then be used as the basis for designing compression structures like arches and domes by inverting the geometry​​.
- **Pneumatic Methods**: Inflating a membrane to achieve a specific form, which can then be used to design various structural forms like shells and domes​​.

Membranes are crucial in both practical engineering applications and computational simulations, providing a versatile tool for exploring and realizing complex, flexible structures.
###### To simulate membranes or other sheet materials such as fabrics, a [[Grids|grid]] of springs is defined. 

Grids can be [[Grids#Grid Generation|established]] using numerous strategies.
![[Pasted image 20240521184625.png]]
	The most common technique is:
		1. To convert a NURBS surface to a mesh.
		2. [[Computational Methodology#Decomposition|Decompose]]/[[Large Scale Projects#Surface Discretization|Discretization]] 
			Extract the edges, and vertices.
				These become the springs and particles of the system.
###### Discretization 
