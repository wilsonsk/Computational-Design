---
up:
  - "[[Statics Analysis]]"
related: 
date created: 2024-05-03
---
# Free Body Diagram
A tool used to solve engineering mechanics problems.
The purpose of the diagram is to "free" the body from all other objects and surfaces around it so that it can be studied in isolation.
	The diagram includes any forces or moments acting on the body, including those forces and moments exerted by the surrounding bodies and surfaces that are removed. 

When vectors are drawn to form free body diagrams, the magnitude and direction are usually given in one of two formats (i.e. [[Static Equilibrium#Vector Form Analysis (i.e. Cartesian Vectors)|vector form]] or [[Static Equilibrium#Scalar Form Analysis|scalar form]]).

This diagram makes it easier to write out equilibrium equations for statics or strengths of materials problems, or the equations of motion for dynamics. 

![[Pasted image 20240503152008.png]]
## Constructing the Free Body Diagram
1. First draw the body being analyzed, separated from all other surrounding bodies and surfaces.
	Pay close attention to the boundary, identifying what is part of the body and what is part of the surroundings. 
2. Draw all **external** forces and moments acting directly on the body.
	**Do not include** any **forces or moments** that **do not directly act on the body being analyzed**. 
		**Do not include** any **forces** that are **internal** to the body being analyzed.
3. Label any key dimensions and angles on the diagram. 
## Examples using Common Types of Forces
### Gravitational Forces
![[Pasted image 20240503152715.png]]
Gravitational forces always act downward on the center of mass. 
### Normal Forces (i.e. Reaction Forces)
![[Pasted image 20240503152953.png]]
Every object in direct contact with the body will exert a normal force (a force that is perpendicular to the surfaces in contact) on that body which prevents the two objects from occupying the same space at the same time. 
	Note that only objects in direct contact can exert normal forces on the body.

An object in contact with another object or surface will experience a normal force that is perpendicular (normal) to the surfaces in contact.
	I.e. Normal forces always act perpendicular to the surfaces in contact. The barrel in the hand truck shown on the left has a normal force at each contact point.
		 The roller on the left allows for rotation and movement along the surface, but a normal force in the y direction prevents motion vertically. 
			 The pin joint in the center allows for rotation, but normal forces in the x and y directions prevent motion in all directions. 
				 The fixed connection on the right has a normal forces preventing motion in all directions and a reaction moment preventing rotation.
![[Pasted image 20240503153034.png|400]]

Joints or connections between bodies can also cause reaction forces or moments, and we will have one force or moment for each type of motion or rotation the connection prevents.
### Friction Forces
Objects in direct contact with the body can also exert friction forces.
	Friction forces will resist the two bodies sliding against one another, on the body. 

Friction forces will always be perpendicular to the surfaces in contact.
	For smooth surfaces we assume that there is no friction force.
	For rough surfaces we assume the bodies will not slide relative to one another no matter what. 
		In this case, the friction force is always just large enough to prevent this sliding. 
![[Pasted image 20240503153508.png]]
*For a smooth surface we assume only a normal force perpendicular to the surface. For a rough surface we assume normal and friction forces are present.*
### Tension Forces
![[Pasted image 20240503153617.png]]
Exert a pulling force on the body in the direction of the source of tension. 
	These forces will always pull on the body and cannot be used for pushing.