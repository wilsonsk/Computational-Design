---
up:
  - "[[Analysis]]"
related: 
date created: 2024-05-15
---
# Bodies
Refers to physical objects that can be analyzed in terms of their [[Newton's Second Law#Motion|motion]], forces acting upon them, and the resulting responses. 
### Particles
A [[Points|particle]] is an idealized object with mass but no dimensions.
	It is considered a point mass, meaning it has a size so small compared to other length scales in the problem that its shape, size, and structure do not affect the analysis.
#### Application
Particles are used in physics to simplify the analysis of motion and forces. They allow focusing purely on translational motion (movement from one place to another) without worrying about rotational effects or the internal structure of the object.
##### In Static Analysis Systems
###### [[Concurrent Systems|Concurrent Systems]]
Particles in concurrent force systems are subjected to multiple forces that all pass through a single common point. Here, only translational equilibrium is considered (i.e., ∑𝐹⃗=0∑F=0).
###### [[Non-Concurrent Systems|Non-concurrent Systems]]
Even in non-concurrent systems, where forces do not meet at a single point, particles are analyzed purely for translational equilibrium because they cannot exhibit rotational motion.
##### In Dynamic Analysis Systems
Similar to statics, a particle in dynamics is an idealized point mass. 
	It is significant in dynamics because it simplifies the study of motion without needing to consider dimensions or rotational effects.
###### Dynamics Analysis
I.e. Motion Analysis.
	The fundamental equations of motion for particles ($F=ma$) describe how linear forces affect the translational motion (acceleration) of particles.
		 In dynamics, the trajectories, velocities, and accelerations of particles under various forces are extensively analyzed.
### Rigid Bodies
A rigid body is an idealized solid object in which the distance between any two given points remains constant, no matter how the body is deformed by forces.
	It does not deform under normal conditions and can be subjected to translational as well as rotational motion.
#### Application
Rigid bodies are extensively used in mechanics to study objects that do not significantly flex, stretch, or compress. Analyzing the motion and forces on rigid bodies involves considering both the forces and moments (torques) that might cause the body to translate and rotate.
##### In Static Analysis Systems
###### [[Concurrent Systems|Concurrent Systems]]
For rigid bodies in concurrent systems, the main concern is ensuring translational equilibrium. Although all external forces act through one point, rotational equilibrium typically does not need separate analysis unless the point of concurrency is not at the center of mass.
###### [[Non-Concurrent Systems|Non-concurrent Systems]]
Rigid bodies in non-concurrent systems require careful analysis for both translational and rotational equilibrium. Forces acting at various points on the body create moments that must be balanced to maintain rotational equilibrium (∑𝜏⃗=0∑τ=0) around any point or, more conveniently, about the center of mass.
##### In Dynamic Analysis Systems
Rigid bodies in dynamics are bodies assumed not to deform under forces or torques. 
	They can undergo translational as well as rotational motions, making their analysis more complex than particles.
###### Equations of Motion
Dynamics of rigid bodies often involves both Newton’s laws for translation (𝐹=𝑚𝑎F=ma) and rotation (𝜏=𝐼𝛼τ=Iα, where 𝐼I is moment of inertia and 𝛼α is angular acceleration). These bodies are analyzed to determine responses to forces and torques, including the effects of inertia and damping.
###### Kinematics and Kinetics
Analysis includes kinematics (describing motion without regard to forces) and kinetics (forces causing the motion), providing a comprehensive understanding of motion in systems like vehicles, machinery, and aerospace structures.
### Deformable Bodies
Deformable bodies, unlike rigid bodies, can change shape in response to forces. 
	The analysis of deformable bodies takes into account the object’s elasticity, plasticity, and other material properties that influence how it deforms.
#### Application
Commonly used in materials science, civil engineering, and mechanical engineering, deformable body mechanics are crucial for understanding how structures bend, stretch, compress, or otherwise deform under various loads.
##### In Static Analysis Systems
Deformable bodies are analyzed less frequently in basic statics due to their complex behavior under load, but they are crucial in more advanced studies like strength of materials and structural analysis.

The study often focuses on how deformations are distributed within the body and ensuring that the net forces and moments remain balanced to maintain overall static equilibrium.
##### In Dynamic Analysis Systems
Deformable bodies can significantly change shape and size under forces. 
	The dynamics of deformable bodies is more complex due to the need to consider internal stresses and strains alongside external forces.
###### Complex Responses
Studying the dynamic behavior of deformable bodies often involves sophisticated models like finite element analysis, which can simulate how these bodies respond dynamically to impacts, oscillating loads, and other time-dependent forces.
### Continua (Continuous Media)
Continua, or continuous media, are bodies that can be modeled as continuously distributed material without discrete particles.
	This model is used to study fluids (liquids and gases) and elastic solids in a unified framework, focusing on properties like density, pressure, and velocity fields.
###### Application
The continuum model is fundamental in fluid dynamics and elasticity theory. It helps analyze flow patterns, stress distributions, and dynamic responses of materials under external influences.
