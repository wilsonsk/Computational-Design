# Curves as Parametric Functions (i.e. [[Mapping#General Vector-Valued Function Notation|Vector-Valued Functions]])
*[[Curves Theory|Curves can describe many things.]]*
![[Pasted image 20240903055710.png]]
$$\LARGE \vec{r}(t), \quad \text{Where $t$ is a parameter.}$$
$$\LARGE \vec{r}(t) = [\vec{x}(t), \vec{y}(t), \vec{z}(t)]$$
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

#### For Parametric Curves
