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
PSS iterative calculations approach an [[Static Equilibrium|equilibrium state]] where the sum of all the forces is zero. 
	The iterative calculations are performed by mathematical solvers. 
###### Mathematical Solvers
Operate iteratively within a main *engine*, meaning every subsequent iteration narrows the position and velocity (magnitude and direction) of particles from the previous step towards an equilibrium solution. 