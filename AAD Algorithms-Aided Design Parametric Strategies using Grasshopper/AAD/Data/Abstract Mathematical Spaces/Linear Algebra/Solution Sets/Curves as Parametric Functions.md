# Curves as Parametric Functions (i.e. [[Mapping#General Vector-Valued Function Notation|Vector-Valued Functions]])
*[[Curves Theory|Curves can describe many things.]]*
![[Pasted image 20240906071943.png]]
$$\LARGE \vec{r}(t) : [0,1] \to \mathbb{R}^3, \quad \vec{r}(t) = [x(t)\textcolor{red}{,}\space y(t)\textcolor{red}{,}\space z(t)], \quad x,y,z : [0,1] \to \mathbb{R} $$
$$\LARGE \equiv \mathbf{r}(t) = (x(t)\textcolor{red}{,}\space y(t)\textcolor{red}{,}\space z(t))$$
$$\LARGE \equiv \text{A linear Combo of Std. Unit Vectors: }\quad \vec{r}(t) = x(t)\vec{i} \textcolor{red}{+} y(t)\vec{j} \textcolor{red}{+} z(t)\vec{k} $$
$$\LARGE \equiv \text{A linear Combo of Std. Unit Vectors: }\quad\mathbf{r}(t) = x(t)\mathbf{i} \textcolor{red}{+} y(t)\mathbf{j} \textcolor{red}{+} z(t)\mathbf{k}$$
$$\text{Where } \quad \vec{i} = \mathbf{i} = (1,0,0), \quad \vec{j} = \mathbf{j} = (0,1,0), \quad \vec{k} = \mathbf{k} = (0,0,1)$$
$$\text{And where each component function scaled by a std. unit vector is another vector}$$
$$\quad x(t)\mathbf{i} = ( x(t), 0, 0), \quad y(t)\mathbf{j} = (0, y(t), 0), \quad z(t)\mathbf{k} = (0,0,z(t)) $$
$$\LARGE \implies \textcolor{red}{\neq} \cancel{\mathbf{r}(t) = \textcolor{red}{(}x(t)\mathbf{i}, y(t)\mathbf{j},z(t)\mathbf{k}\textcolor{red}{)}}$$
$$\LARGE \text{Where $\vec{r}$ is a Vector-Valued Function, and $t$ is a parameter.}$$
$$\LARGE \text{And $x(t), \space y(t), \space z(t)$ are Component Scalar Functions, $\mathbb{R}\to \mathbb{R}$} $$
The Scalars returned by these component scalar functions compose the "points" of the returned vector. 
## $\LARGE t$ as a Parameter
In the context of the parametric function $\vec{r}(t)$, where $\vec{r}(t)$ is typically a vector-valued function describing a curve or path in space, the variable $t$ is identified as a parameter due to the following characteristics:
##### 1. [[Parameters vs. Variables#Step 2 Analyze the Role of the Variable|Role as a Controlled Variable]]

- **Description**: The variable $t$ does not represent a spatial coordinate (such as $x$, $y$, or $z$), but rather it controls the position along the curve or path described by $\vec{r}(t)$.
- In the parametric vector function $\LARGE \vec{r}(t)$, the variable $t$ controls the values of the component vectors $\LARGE \vec{x}(t)$, $\LARGE \vec{y}(t)$, and $\LARGE \vec{z}(t)$.

- **Example in $\vec{r}(t)$**:: Each component vector, $\LARGE \vec{x}(t)$, $\LARGE \vec{y}(t)$, and $\LARGE \vec{z}(t)$, is a function of $t$. As $t$ varies, it influences these component functions, determining their values at each point along the curve or path described by $\LARGE \vec{r}(t)$. Essentially, $t$ dictates how the entire vector $\LARGE \vec{r}(t)$ changes, which in turn defines the trajectory of the curve in space.

	- **For a given $\LARGE t$**: The specific values of $\LARGE \vec{x}(t)$, $\LARGE \vec{y}(t)$, and $\LARGE \vec{z}(t)$ are determined by the corresponding functions of $t$. Together, these values give the position of a point on the curve at that particular $t$.
	- **For a range of $t$ values**: As $t$ changes within its domain, it "controls" the movement along the path or curve in space by altering the values of $\LARGE \vec{x}(t)$, $\LARGE \vec{y}(t)$, and $\LARGE \vec{z}(t)$, thereby defining the entire curve traced by $\LARGE \vec{r}(t)$.
	- **Independent of the Spatial Dimensions**: Unlike $\LARGE \vec{x}(t)$, $\LARGE \vec{y}(t)$, and $\LARGE \vec{z}(t)$, which represent spatial coordinates, $t$ is not directly tied to a physical dimension in the space. Instead, it serves as an abstract quantity that determines the progression along the curve.
##### 2. [[Parameters vs. Variables#Step 3 Look at the Variable's Flexibility|Fixed in Context, Varies Across Scenarios]]

- **Description**: For a specific instance of the function, $t$ takes on particular values, but it can vary across different instances to describe different points on the curve.
- **Example in $\vec{r}(t)$**: While analyzing the path traced by $\vec{r}(t)$, $t$ is treated as a variable that varies continuously over an interval (e.g., $[0, 2\pi]$ for a full circle). Within this context, $t$ is not a fixed constant but varies to describe the curve.
	- It parameterizes the curve, meaning it describes how to move along the curve from one point to another.
##### 3. [[Parameters vs. Variables#2. Does the Variable Define a Family of Solutions?|Describes a Family of Points]]

- **Description**: The parameter $t$ allows the function to describe a family of points along a curve rather than just a single point.
- **Example in $\vec{r}(t)$**: As $t$ changes, $\vec{r}(t)$ describes all the points on a circle or another curve. Each distinct value of $t$ corresponds to a unique point on the curve, making $t$ the parameter that generates the curve by varying over its domain.

##### 4. Defines a Continuous Path

- **Description**: $t$ defines a continuous and smooth path in space as it varies, which is a characteristic of parameters in parametric functions.
- **Example in $\vec{r}(t)$**: In the function $\vec{r}(t) = \langle \cos(t), \sin(t) \rangle$, $t$ moves the point smoothly along the circumference of a circle, indicating that it is the parameter driving this movement.

##### 5. [[Parameters vs. Variables#3. Is the Variable Controlling the Equation’s Behavior?|Influences the Behavior of the Function]]

- **Description**: $t$ directly influences the behavior of the function $\vec{r}(t)$ by determining which point on the curve is being described at any given moment.
- **Example in $\vec{r}(t)$**: The behavior of $\vec{r}(t)$ as a function of $t$ shows how the curve is generated in the plane or space, with $t$ controlling the specific output of $\vec{r}(t)$ at each instance.
## The Domain of Parametric Curves
#### In General
$$\LARGE f: X \to Y$$
$$\LARGE \text{Domain of $f$, }\quad D_f \subset X$$
$$\LARGE \text{Codomain of $f$, }\quad Y $$
$$\LARGE \text{Range of $f$, }\quad V_f \subset Y$$

The **domain** of a function is a subset of $\LARGE X$, that is, the set of the all the possible arguments.
	For example, $\LARGE f: \mathbb{R} \to \mathbb{R}, \quad f(x) = \frac{1}{x}$ the domain is, $\LARGE D_f  = \mathbb{R} \backslash {0} == V_f$
		*Where '\' is notation for "except".*

The **range** of a function is a subset of $\LARGE Y$ where $\LARGE V_f = \{y;\space y = f(x) \text{ for some } x \in D_f\}$
### The Domain of Parametric Curves (i.e. Vector-Valued Functions) is an Interval (i.e. an intersection of the Domains of its Component Scalar Functions)
The Domain consists of **all** the values of the parameter $t$, for which **all** the component functions are possible to compute. 
	Each scalar function $\vec{x}(t)$, $\vec{y}(t)$, and $\vec{z}(t)$ may have different domains, but for the vector-valued function $\vec{r}(t)$ to be defined, $t$ must be in the domain of **all** of the component functions.
		This ensures that $\vec{r}(t)$ is defined only where all of its components are defined.
		
Therefore, the Domain of the Vector-Valued Functions is the intersection (i.e. $\LARGE \cap$) of the two or three component scalar functions.
	The Domain of $\LARGE \vec{r}$ being an intersection of the Domains its corresponding component scalar functions, implies that the Domain of $\LARGE \vec{r}$ is in fact an interval. 
$$\LARGE D_{\vec{r}} = D_x \space \cap \space D_y \space\cap \space D_z$$
###### For Example
$$\LARGE \vec{r} = \left( 2t+1, \frac{\sin t}{t}, \frac{1}{\sqrt{1-t^2}} \right)$$
$$\LARGE \text{Where }\quad  x(t) = 2t+1, \quad D_x = \mathbb{R}$$
$$\LARGE y(t) = \frac{\sin t}{t}, \quad D_y = \mathbb{R} \backslash \{0\}$$
$$\LARGE z(t) = \frac{1}{\sqrt{1-t^2}}, \quad D_z = [-1,1]$$
$$\LARGE \text{(I.e. $t$ is any value between the interval $-1$ and 1)}$$
$$\LARGE \text{Therefore, } D_\vec{r} = [-1,0] \space \cup \space [0,1]$$
### The Domain of $\vec{r}(t)$ as an Intersection of its Component Functions Implies an Interval which is itself a Subset of $\mathbb{R}^1$
Each component function $x(t)$, $y(t)$, and $z(t)$ has its own domain, denoted by $D_x$, $D_y$, and $D_z$, respectively.
	The **domain** $D_{\vec{r}}$ of the entire vector-valued function is the set of all values of $t$ where all three component functions are defined. In other words, it is the intersection of $D_x$, $D_y$, and $D_z$.
		If this intersection is a connected set of real numbers, it is typically represented as an **interval**. 
			Since an interval is a **subset of $\mathbb{R}^1$**, this indeed implies that the domain $D_{\vec{r}}$ is a subset of $\mathbb{R}$ (the real number line).

The parameter $t$ is a real number, and the domain of $\vec{r}(t)$ is a set of values that $t$ can take where all component functions ($\vec{x}(t), \vec{y}(t), \vec{z}(t)$) are defined.
	Therefore, the domain of $\vec{r}(t)$ is a subset of $\mathbb{R}^1$, typically an interval like $[a, b]$ or a larger set like $(-\infty, \infty)$, depending on the context.
#### Implication Breakdown
##### Intersection of Domains
$\LARGE D_x \cap D_y \cap D_z$ refers to the set of $t$ values where all component functions $x(t)$, $y(t)$, and $z(t)$ are simultaneously defined.
##### Interval
If this set is continuous, it forms an interval, which could be closed, open, or half-open (e.g., $[a, b]$, $(a, b]$, etc.).
##### Subset
Any interval is a subset of $\mathbb{R}$, meaning $D_{\vec{r}} \subseteq \mathbb{R}$.
#### Why an Interval of $\mathbb{R}^1$ rather than all of $\mathbb{R}^1$?
The domain of a parametric curve is usually an **interval** of $\mathbb{R}^1$ rather than the entire real line $\mathbb{R}^1$, because parametric curves typically describe a **finite path** or trajectory through space. 
	I.e. **The domain of a parametric curve is an interval of $\mathbb{R}^1$** because the curve is typically only defined or of interest over a specific range of $t$ values, and this range is represented by an interval.
##### Finite Definition of the Curve
The parameter $t$ represents a single degree of freedom that controls movement along the curve. 
	Often, we are only interested in tracing the curve over a specific range of $t$ values, which corresponds to an interval. 
		For example, in a circle parameterized by $t$:
$$\LARGE \vec{r}(t) = [\cos(t), \sin(t)] $$
		  You might restrict $t$ to the interval $[0, 2\pi]$ to describe one full rotation around the circle.
##### Specific Intervals
Parametric curves often represent segments or bounded portions of curves. 
	For example, if you wanted to describe a segment of a line or a part of a curve, you would restrict $t$ to a particular interval, say $[a, b]$. 
		For instance, if $t \in [0, 1]$, it might represent a specific portion of the curve between two points.
#### Why not all of $\mathbb{R}^1$?
##### Infinite Domain
In some cases, we can extend the domain to be all of $\mathbb{R}^1$ (e.g., $t \in (-\infty, \infty)$), but in many practical cases, we're interested in specific portions of the curve, like a finite arc of a circle, a segment of a line, or a finite motion trajectory.
	This makes an interval more suitable for describing such cases.
##### Natural Boundaries
Some curves or motions inherently have a beginning and an end.
	For example, if you’re describing a finite-length curve, it makes sense to define the domain of $t$ as an interval, rather than the entire real line.

## How to [[Data/Abstract Mathematical Spaces/Linear Algebra/Solution Sets/Parametrization|Parametrize]] a Curve