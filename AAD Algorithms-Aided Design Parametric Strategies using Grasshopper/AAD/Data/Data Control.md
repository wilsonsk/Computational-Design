---
up:
  - "[[Data]]"
related:
  - "[[Data Relationships]]"
  - "[[Data Operations]]"
  - "[[Elemental Building Blocks]]"
  - "[[Data Trees]]"
  - "[[Numbers]]"
  - "[[Parameters]]"
  - "[[Points]]"
date created:
  - 2024-03-23
---
# Data Control

## Data Control is about how designers or algorithms interact with the data itself to influence the design outcome. 

Data control involves the active **manipulation** of those parameters within the framework set by those relationships.

Data control represents the **process** or **actions** taken within that structure to achieve desired design outcomes.

Data control is implemented by **Boolean operations** and **algorithms**, the latter is the sequence of data control operations and data relationship equations.

## Definition and Role: 
Data control refers to the mechanisms and strategies employed to manipulate, guide, or constrain data within a design system. 

It involves the tools and methods used to input, adjust, and manage data, ensuring that the design adheres to specific constraints, meets certain criteria, or explores a desired range of possibilities. 

Data control mechanisms might include user interfaces for inputting parameters, algorithms that automate certain design decisions, or optimization routines that search for the best design solutions within a defined space.

## Examples:
An example of data control is a slider in a graphical user interface that allows the designer to adjust the radius of a cylindrical column within a specific range. 

The slider controls the input data (radius) within predetermined bounds. 

Another example is an optimization algorithm that adjusts various design parameters to minimize material usage while maintaining structural integrity.
## Purpose:
The purpose of data control is to enable designers to interact with and influence the design process actively. 

It provides the means to implement design intentions, explore design spaces, and achieve design objectives through direct manipulation of parameters and automated adjustments based on performance feedback.

## Algorithms can define every type of geometry:
The method to construct geometries procedurally is based on writing a rough draft and translate it into a programming language. 

For example, the image below can be sketched by writing the following list of instructions: 

0. Draw four circles; 
1. Subdivide the four circles into N parts; we get N points for each circle; 
2. Connect the corresponding points. 

The same element could be defined by different parameters, **but it is natural to write an algorithm in a way that establishes relations between the variable parts of an object**. In the example the number of lines is affected by the number of subdivisions (N), which is the main parameter. Nevertheless, the algorithm is still ambiguous since it does not specify unique origins with respect to the z coordinate: {x,y,z'}, {x,y,z^} and {x,y,z^}, a radius for each circle (r'), (r^) and (r^), and the method of connecting the lines. These refinements are made when transitioning from the rough draft to the final algorithm.

[[Curves]] and [[Surfaces]]

**Algorithmic Modeling**:
	1. Requires an strong understanding of the principles of form generation.
		1. Specifically a knowledge of **NURBS geometries** ([[Nurbs Curves]])
		2. 