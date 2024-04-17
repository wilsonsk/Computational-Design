---
up:
  - "[[Numbers]]"
related:
  - "[[Parameters]]"
  - "[[Grids]]"
  - "[[Data Relationships]]"
  - "[[Elemental Building Blocks]]"
  - "[[Surface Creation]]"
date created: 2024-03-25
---
# Points

##### Points are the **first level of abstraction** constructed from a **relationship between numbers** (fundamental units).

**Numbers** enable a system of relationships between any aspects that the numbers represent.
Points **represent a relative position in space**. 
Therefore, these **positions can relate to other positions**, forming either simple or increasingly complex relationships. 

The positions themselves, can compose next higher level structures like lines and curves.

Positions of a curve could be the **start** and **end** **points** of that curve. 
That is, the **vertices**. 

## A Geometry is Just Points
### A point just represents a position.
And a geometry is composed of defined - "occupied" positions.

[[Elemental Building Blocks#Points Point as the Fundamental Building Block of Form|Points are the fundamental component of the entire geometry.]]

A **line** is the **set** of **all points** in 2D space that are within two bounding points.

A **rotational cylinder** is the **set** of **all points** in 3D space that are equidistant from an axis. 

A **sphere** (surface) is the **set** of **all points** in 3D space that at distance, *r*, from the center, *c*. 

Therefore, lines, planes, surfaces, etc. are just **sets of points**.

## Mathematical Context
### Continuity within Bounds
In calculus, particularly when discussing the concept of continuity and the behavior of functions within specific bounds, you encounter the term **"interval"** to describe the range within which the function behaves or is analyzed. 

Points within these intervals where specific properties of the function are assumed or investigated are typically called **"points of continuity"** if the function does not break, jump, or have an undefined value.
#### Intervals:
##### Closed Interval: 
Denoted as $[a,b]$, this includes both endpoints $a$ and $b$. 
A function defined on a closed interval is assumed to be continuous on that interval if it meets continuity criteria at every point between $a$ and $b$, including the endpoints.
##### Open Interval: 
Denoted as $(a,b)$, this excludes the endpoints. 
A function is considered continuous on an open interval if it is continuous at every point within $a$ and $b$ but not necessarily at $a$ and $b$ themselves.
##### Points of [[Discontinuity|Discontinuity]]:
When discussing continuity within a bounded interval, it’s also crucial to identify points where continuity may be broken. These are called **"points of discontinuity"**. Discontinuities can be **removable (a hole in the graph)**, **jump (sudden jumps in the function values)**, or **infinite (vertical asymptotes)**, among others.
##### Cluster Points:
In some contexts, especially in more advanced calculus or real analysis, **cluster points** (or [[Limits|limit]] points) are considered within bounds. A cluster point of a set within an interval is a point where every neighborhood around it contains other points from the set. This concept is crucial when discussing limits and continuity.
##### Interior Points:
Interior points of an interval are points that can be surrounded by a small interval fully contained within the larger interval. These points are always away from the boundaries of the interval, ensuring that small perturbations around these points stay within the interval.
#### Interpolation
A mathematical and computational technique used to estimate or construct new data points within the range of a discrete set of known data points. 
### Continuity on Closed Intervals:
#### Intermediate Value Theorem (IVT)
The concept in calculus that deals with the assumption of [[Limits#Curves Continuity (i.e. when curves join) Continuity|continuity]] of points within certain bounds.

States that if you have a function $f$ that is continuous on a closed interval [a,b], and $d$ is any number between $f(a)$ and $f(b)$, then there is at least one $c$ in the interval [a,b] such that $f(c)=d$. This theorem fundamentally relies on the concept of continuity.
#### Extreme Value Theorem
A foundational theorem related to continuity within bounds, particularly on closed intervals, is the **Extreme Value Theorem**. This theorem states that if a function $f$ is continuous on a closed interval $[a,b]$, then $f$ must attain its maximum and minimum values at least once each within the interval. This implies that not only is the function continuous, but it also behaves well enough at the boundaries to include all intermediate values (by the Intermediate Value Theorem).
## Vertices:
^vertices
Represent specific positions in space, and subsequently **compose edges**, which **compose faces**.
	Where a set of numbers compose a point
	A set of points compose a vertex.
	A set of vertices compose an edge.
	A set of edges compose a face.  ^96eec9

### Valence:
The of **degree** of a vertex (from **graph theory**).
	I.e. The number of edges that a vertex connects to.
		Including **loops** which are counted twice.
	




