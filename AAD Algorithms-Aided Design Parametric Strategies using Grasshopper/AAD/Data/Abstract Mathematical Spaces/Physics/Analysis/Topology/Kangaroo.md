---
up:
  - "[[Topology Optimization]]"
related:
  - "[[Topology]]"
  - "[[Digital Form-Finding]]"
  - "[[Form-Finding Strategies Using Kangaroo]]"
date created: 2024-05-22
---
# Kangaroo
A Form-finding, optimized, and constraint-solving engine.
  
Kangaroo is a [live physics engine](http://kangaroo3d.com/) that helps form-finding, interactive simulation, optimization, and constraint solving. It is a 3D plugin for Grasshopper and Rhino.
	It enables recording of the designing steps where one can go back and make changes to the previous actions, which changes the final output accordingly.

Daniel Piker created it in 2014, one of the many popular plugins for Rhino 3D.

Structural engineers use Kangaroo to produce accurate structural solutions for parametric design projects. 
	The software optimizes structural elements like columns, beams, steel frames, steel rebars, etc., in terms of their performance and workability in the design. 
		It also analyses the structural components, reveals errors, and resolves constraints. 
			When changes are made to the structure, the optimization and analysis tool adjusts the model on a real-time basis. 

Kangaroo is like a physical laboratory where one can simulate the elastic behavior of cables, chains, members, etc., to predict a shape coming from form-finding software. 
	But, It does not allow one to calculate the formations or calculate stresses inside the geometries.
## Workflow of Kangaroo
![[Pasted image 20240522125203.png]]

1. The **Kangaroo** component must be first placed in the Grasshopper Canvas to create a simulation.

**_Kangaroo Physics_:** It will give the user the forces and show them the animation of how the forces react to each other.

**_Zombie Kangaroo:_** There is no animation and will only show the results of what is acting on the surface.

Kangaroo uses the [[Form-Finding Strategies Using Kangaroo#Particle-Spring System|particle-spring system]] where a chain is fixed to two points, and more minor issues divide the chain into different segments. 
	Each segment is made of “[[Form-Finding Strategies Using Kangaroo#Springs|Spring]],” which are essentially elastic elements that move according to the points on either side.
		 Since the peripheral points cannot be transferred, forces can be applied to the intermediary points and change their positions. 

Similarly, an entire mesh can created from springs arranged in a  square grid of desired columns and rows.
#### Inputs
###### Force Objects
 It is an input where the generated forces that affect the 3D Model particles are fed.
	  The forces could be material deformation, user input, or geometric constraints.
		   Kangaroo creates interactions between the force and 3D model through force vectors.
###### Anchor Points
These are certain point on the mesh that maintains a fixed location. 
	Whatever forces applied on the points, Kangaroo cannot move them. 
		Rhino can transfer the points to interact with the simulation as it is running.
#### Joining Objects Together
If two or more points in the initial input (Force Objects and Anchors) are in the same position (within the tolerance setting), they will get joined together and treated as a single particle by Kangaroo.
### Settings
![[Pasted image 20240522125502.png]]- 
###### Tolerance
Minimum distance between two separate points. If points are closer than the tolerance, they will be merged into one.
###### TimeStep
How fast the system moves through different versions. Smaller values produce stable but slow simulations. Stronger forces require smaller time steps.
###### Sublterations
Number of iterations computed between each solution being drawn.
###### Floor
A physical constraint that can turned on and off restricting particles from moving to the lowest level. (Z=0)
###### Drag
Resisting force on particles against their motion. This feature helps the system settle down to a static equilibrium position. The system will oscillate if the drag is too slow, and the particles will move too fast if the drag is less.
###### Restitution
This shows the elastic collisions between the floor and particles. 1= Particles bounce back to their initial height from which they were dropped, 0= they do not bounce.
###### Tumble
How much horizontal velocity is conserved in collisions between particles and floor?
###### Solver
A calculator that uses the integration method to compute new positions of particles.
#### Simulation Output
Disturbances in the simulation can become unstable when dealing with particles because Kangaroo is trying to represent functions that are continuous in time steps that are non-continuous.
	This can improve by using softer springs or by increasing the spring dampening and drag so that the actions happen in smaller time intervals, allowing for more calculations for the same amount of movement.

Disturbances can also reduce by increasing the number of calculations between the seen particle interactions.

## Applications of the Software
- Creates meshes that can use as 2D planes which join together to create a 3D model.
- Meshes can treated as plane surfaces to apply materials and for fabrication.
- Creates equal sizes of meshes, making them modular instead of having different sizes of meshes across the project.
- To enable the creation of membrane roofs, it minimizes the surface area of the mesh.
- Kangaroo helps create canary arches, an otherwise extremely difficult element to create structurally.
- Has the ability to create arches and domes that are structurally accurate.
- Simulates origami-like folding elements with flat surfaces that can expand and contract.
- It can check gravity loading on framed systems to visualize deflections in individual elements.
- Analyze imposed loads on the structure or building like wind, snow, and other lateral loads.
- The gears of a machine to check the workings of an engine.
- Simulates loads on panels to see how they’d bend under pressure.
- Simulates how objects would configure themselves if packed within a certain area.
### Advantages of Kangaroo
- It helps create advanced curves like catenary
- Analyses the behavior of the forces acting on it
- Free software
- Parametric – editing in real-time
- Compatible with 3D modeling software -Rhino
- Provides accurate simulations for the physics of the structure
- Creation of tensile structures

One of the demerits of the Kangaroo is that it is a complex learning curve where the outputs might have errors. There are also chances of system crashes if the inputs are wrong.