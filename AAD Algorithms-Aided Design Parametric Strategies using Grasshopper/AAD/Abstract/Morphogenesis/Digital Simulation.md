# Digital Simulation (and Particle Spring Systems)
*"Science is a tool for ideas [...] and it is not only a means to verify structural strength. Science must lead us to discover the optimized geometry for that particular static (or dynamic) condition".* - Sergio Musmeci

Structures that transmit forces through axial compression or tension have an increased capacity to withstand loads with smaller cross sectional areas.
	Traditional form-finding strategies for axially loaded structures include: complex physical models, hanging chain networks, stretched fabrics, soap films etc..
These techniques are difficult and time consuming. 
	As a result, few designers investigated these form-finding potentials. 
		 Traditional form-finding techniques can now be digitally found using particle-spring systems that simulated the physical behavior of deformable bodies.
			 Whereas traditional techniques were difficult to apply, digital simulations allow designers to investigate form, in real time, by updating forces, supports and physical properties.
## Particle-Spring Systems
![[Pasted image 20240502012955.png|400]]
Are a discretization of a continuous model into a finite number of masses, called particles, connected by elastic springs. 
#### Main Components
###### Particles
Each particle in the system is a lumped mass, that changes position and velocity as the simulation evolves.
###### Springs
An elastic linear connection between two particles that behaves according to the **Hooke's Law**.
	"A spring has an initial resting length and a stiffness value, $k$".
###### Forces
Weights and external loads are simulated by [[Structural Analysis#Vector Addition|vectors]] that are applied exclusively to particles.
###### Anchor Points
Particles that do not change position during the simulation.