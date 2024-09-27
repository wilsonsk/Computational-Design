# Straight Lines
The functions that produce lines, are themselves solution sets, and each solution of the set is contained within the produced line.
## Straight Lines in the Plane (I.e. Straight Lines in $\mathbb{R}^2$) 
Lines in $\mathbb{R}^2$ (i.e. lines that exist in the plane) can be represented in 4 ways.
### 1. Standard Form of a Line
![[Pasted image 20240814060236.png|500]]
The general equation of a straight line in two dimensions can be written as:
$$\LARGE y = mx + b$$
   where:
   - $y$ is the dependent variable,
   - $x$ is the independent variable,
   - $m$ is the slope of the line (the rate at which $y$ changes with respect to $x$),
   - $b$ is the y-intercept (the value of $y$ when $x = 0$).
#### Think About It...
$\LARGE y$ and $\LARGE x$ are Directly Proportional if $\LARGE b = 0$.
	Where $\LARGE m$ is then the [[Division#Constant of Direct Proportionality is a Constant Ratio ($ LARGE k$)|Constant of Proportionality]] of $\LARGE y$ and $\LARGE x$. 
#### The Standard Equation of a Line with Slope $m$ Passing Through a Point $(x_1, y_1)$
The equation $\LARGE y - y_1 = m(x - x_1)$ is known as the **point-slope form of a line**. 
	It is derived by starting from the general form of a line and using the condition that the line passes through a specific point $(x_1, y_1)$. 
		This form is particularly useful because it directly relates the slope of the line $m$ and the coordinates of a point on the line.
##### Finding the Equation with a Specific Point
Suppose we know the slope $m$ of the line and we want the line to pass through a specific point $(x_1, y_1)$.
	We can start with the general form of the line and use the point $(x_1, y_1)$ to find $b$, the y-intercept.

1. **Using the Point to Find the Y-Intercept**:
   Substitute $x_1$ for $x$ and $y_1$ for $y$ in the general equation $y = mx + b$:
$$\LARGE y_1 = mx_1 + b$$
   To solve for $b$, rearrange this equation:
$$\LARGE b = y_1 - mx_1$$
4. **Substitute Back to Get the Point-Slope Form**:
   Now, substitute $b = y_1 - mx_1$ back into the general equation $y = mx + b$:
$$\LARGE y = mx + (y_1 - mx_1)$$
   This can be rearranged as:
$$\LARGE y - y_1 = m(x - x_1)$$
###### *How to calculate the [[Data/Abstract Mathematical Spaces/Physics/Analysis/Tangent Line#The Tangent Line Through a Point|tangent line through a point]]*
### 2. Normal Equation of a Line
![[Pasted image 20240814060636.png]]
Is an equation for a line $\LARGE l$ through $\LARGE \mathbf{x_0} = (x_0, y_0)$ and orthogonal to the vector $\LARGE \vec{n} = (A,B)$.
$$\LARGE Ax + By + C = 0$$
Where $\LARGE \textcolor{red}{C = -Ax_0 - By_0}$

This equation represents the linear combination of the normal vector scaled by the coordinates of the terminating point $\LARGE x=(x,y,z)$, where $\LARGE C$ is some constant that allows the equation to equal $0$. 
	$\LARGE Ax+By+C=0$ is the [[Data/Abstract Mathematical Spaces/Linear Algebra/Dot Product|dot product]] of $(A,B)$ and $(x-x_0, y-y_0)$.
#### The Reasoning of the Normal Equation
If a point $\LARGE x_0=(x_0,y_0)$ belongs to the plane $\LARGE \pi$ then the vectors $\LARGE \vec{n}=(a,b)$ and $\LARGE \mathbf{x}-\mathbf{x_0} = (x-x_0, y-y_0)$ must be orthogonal.
	This means the [[Data/Abstract Mathematical Spaces/Linear Algebra/Dot Product|dot product]] between the two vectors must be produce $\LARGE 0$.
		Where $\LARGE \textcolor{red}{c}$ contains the remaining terms that equate the equation to the dot product between the two vectors.
$$\LARGE (a,b) \cdot (x-x_0, y-y_0) = 0$$
$$\LARGE  \iff$$
$$\LARGE  ax\textcolor{red}{-ax_0} + by\textcolor{red}{-by_0} = 0$$
$$\LARGE  \iff$$
$$\LARGE ax+by+\textcolor{red}{c}= 0$$
### 3. Intercept Form of a Line
![[Pasted image 20240814061157.png|500]]
$$\LARGE \frac{x}{b_1} + \frac{y}{b_2} = 1$$
Where $\LARGE b_1$ is the $\LARGE x$-intercept.
	That is where the line intersects the $\LARGE x$-axis (i.e. where $\LARGE y =0$)
		I.e. $\LARGE (b_1, 0)$

Where $\LARGE b_2$ is the $\LARGE y$-intercept.
	That is where the line intersects the $\LARGE y$-axis (i.e. where $\LARGE x =0$)
		I.e. $\LARGE (0, b_2)$
### 4. Point Vector Form of a Line (i.e. a Parametric Equation)
![[Pasted image 20240814062213.png|500]]
A Parametric equation that utilizes a single parameter $\LARGE t$ that is $\LARGE \in \mathbb{R}$.
	Where any point on the line $\LARGE \mathbf{x}$ can be described as a Linear Combination of the initial point $\LARGE x_0$ and where the parameter $\LARGE t$ [[Scaling|scales]] the [[Partial Derivatives#Direction Vector in the Plane $y = b$|Direction Vector]] $\LARGE \vec{v} = (v_1, v_2)$ of the line.
$$\LARGE \mathbf{x} = x_0 + t\vec{v}, \quad t \in \mathbb{R}$$

- - - 
## Straight Lines in the Space (I.e. in $\mathbb{R}^3$)
Lines in $\LARGE \mathbb{R}^3$ (i.e. lines that exist in space) can be represented in 2 ways.
	This is because there is **no** concept of slope in Space ($\LARGE \mathbb{R}^3$).
		Slope is the [[Division#Constant of Direct Proportionality is a Constant Ratio ($ LARGE k$)|Constant of Proportionality]] between **two** values. 
### Point Vector Form of a Line in Space (i.e. Parametric Equation)
![[Pasted image 20240811062503.png]]
A point $(x,y,z)$ and the origin point $\LARGE \mathbf{x} = (x_0,y_0,z_0)$, in linear combination with a scaling of the parameter ($\LARGE t$) of the [[Partial Derivatives#Direction Vector in the Plane $y = b$|direction vector]] ($\LARGE \vec{v} = (v_1, v_2, v_3)$) of the line.
$$\LARGE \mathbf{x} = x_0 + t\vec{v}, \quad t \in \mathbb{R}$$
#### Point Vector Form "Coordinate-Wise"
This form describes the same Point Vector Form equation, but substitutes the coordinates of a point and vector with the corresponding variables.
$$\LARGE (x,y,z) = (x_0,y_0,z_0) + t(v_1,v_2,v_3), \quad t \in \mathbb{R}$$
##### Coordinate-Wise in Three Rows
A Linear System of Equations that gives the coordinates of any point on the line, $\LARGE l$.
	One **row** for each coordinate. 
$$\LARGE l:\begin{Bmatrix} x = x_0 + v_1t \\ y = y_0 + v_2t \\ z = z_0 + v_3t\end{Bmatrix}, \quad t \in \mathbb{R}$$
### Standard Equation for a Line Through a Point
A Parameter-free (i.e. Non Parametric) equation, and instead is an equality of (i.e. [[Division#Proportionality|Proportion]]) of some quotients.
	But is **derived** from the [[#Point Vector Form "Coordinate-Wise"|Point Vector Form]] (i.e. the Parametric equation).
		This is done by solving all the "rows" for parameter $\LARGE t$ of the Point Vector Form equation.

Describes a line $\LARGE l$ through the point $\LARGE x_0 = (x_0, y_0, z_0)$ and with a [[Data/Abstract Mathematical Spaces/Physics/Analysis/Multivariable Calculus/Partial Derivatives#Direction Vector in the Plane $y = b$|direction vector]] $\LARGE \vec{v} = (v_1, v_2, v_3)$ with all non-zero coordinates.
	Eliminate the $t$ parameter:
$$\LARGE l: \begin{Bmatrix} x = x_0 + v_1t \\ y = y_0 + v_2t \\ z = z_0 + v_3t\end{Bmatrix} =  \frac{x - x_0}{v_1} = \frac{y - y_0}{v_2} = \frac{z - z_0}{v_3}$$

If *for example* $\LARGE v_2 = 0$ (and $v_1, v_3 \neq 0$), produces the following equation:
$$\LARGE \frac{x-x_0}{v_1} = \frac{z-z_0}{v_3}, y = y_0$$
Here, the $y$-coordinate is **constant** for all the points on the line, which means that the line lies in the **plane** $\LARGE y = y_0$ which is **parallel** to the $\LARGE xz$-plane.
	But this form with a zero coordinate doesn't "look" right because it has a $\LARGE \frac{y-y_0}{0}$ a division by $0$.
		In which case using the Point Vector Form is optimal. 

- - -
## The Tangent Line Through a Point (on a Curve)
The equation of the tangent line through a point $(a, f(a))$ is derived from the limit of the slope of the secant line as it approaches the point $(a, f(a))$. 
	The equation $y = f(a) + f'(a)(x - a)$ is derived by finding the slope of the tangent line as the limit of the slopes of secant lines and then using the point-slope form of the equation of a line. 
		This process ensures that the tangent line touches the curve $y = f(x)$ at exactly one point $(a, f(a))$ and has a slope equal to the derivative $f'(a)$ at that point.

The **tangent line** through a point on a curve is derived using the derivative to find [[Straight Lines#The Standard Equation of a Line with Slope $m$ Passing Through a Point $(x_1, y_1)$|the slope at that point]].

1. **Secant Line Slope**:
   The slope of the secant line between the points $(a, f(a))$ and $(x, f(x))$ on the curve $y = f(x)$ is given by:
   $$\LARGE
   m_{\text{sec}} = \frac{f(x) - f(a)}{x - a}
   $$

2. **Tangent Line Slope**:
   The slope of the tangent line at the point $(a, f(a))$ is the limit of the secant slope as $x$ approaches $a$:
   $$\LARGE
   m_{\text{tan}} = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}
   $$

   This limit, if it exists, is the derivative of $f(x)$ at $x = a$, which we denote as $f'(a)$:
   $$\LARGE
   m_{\text{tan}} = f'(a)
   $$

3. **Equation of the Tangent Line**:
   The equation of a line with slope $m$ passing through a point $(x_1, y_1)$ is:
   $$\LARGE
   y - y_1 = m(x - x_1)
   $$

   In our case, the slope $m$ is $f'(a)$ and the point $(x_1, y_1)$ is $(a, f(a))$. 
	   Plugging in these values:
   $$\LARGE
   y - f(a) = f'(a)(x - a)
   $$

4. **Rearranging to the Standard Form**:
   We can rearrange this equation to the more familiar form of the tangent line:

   $$\LARGE
   y = f(a) + f'(a)(x - a)
   $$
### The Relationship Between the Tangent Line (Through a Point) and [[#1. Standard Form of a Line|The Standard Form of a Line]]
##### The Tangent Line Through a Point
$$\LARGE y = f(a) + f'(a)(x - a)$$
##### The Standard Form of a Line
$$\LARGE y = mx + b$$
#### The Derivative as the [[Derivatives#Is the Tangent Line The Slope of a Tangent Line Slope (i.e. a proportion/rate/ratio between $ Delta y / Delta x$) of the Tangent Line Tangent Line|Slope]] of a Tangent Line
The [[Derivatives|derivative]] of that single point along the curve of a function is the slope of the tangent line through a point.
$$\LARGE m_{tan} = f'(a) = \frac{\Delta y}{\Delta x} = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}$$ - - -
### Computing the Normal Line Through a Point with a Directional Vector
There are two ways to calculate a **line** through a **point**, $\LARGE (a,b,f(a,b))$ , on the [[Planes|plane]] ($\LARGE \pi$), with the directional vector (being the [[#Normal Vector as a Cross Product Cross Product (Between the two Tangent Vectors of Partial Derivatives)|normal vector]]), $\LARGE \vec{v} = (f'_x(a,b), f'_y(a,b), -1)$.
##### [[Straight Lines#Parametric Equation|Parametric Form of a Line Through a Point with a Vector]]
$$ \begin{Bmatrix} x = x_0 + v_1t \\ y = y_0 + v_2t \\ z = z_0 + v_3t\end{Bmatrix} =(x,y,z) = (a,b,f(a,b)) + t(f'_1(a,b), f'_2(a,b), -1), t \in \mathbb{R}$$
##### [[Straight Lines#Standard Equation for a Line Through a Point|Standard Form of a Line Through a Point with a Vector]]
$$\LARGE \frac{x - x_0}{v_1} = \frac{y - y_0}{v_2} = \frac{z - z_0}{v_3} = \frac{x - a}{x'_x(a,b)} = \frac{y - b}{f'_y(a,b)} = \frac{z - f(a,b)}{-1}$$