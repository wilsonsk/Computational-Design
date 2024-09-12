# Vector-Valued Single Variable Derivatives, $\LARGE \vec{r}: [0,1] \to \mathbb{R}^3$
![[Pasted image 20240910063322.png]]
For Vector-Valued Functions composed of Scalar-Valued Functions, derivatives are computed **component-wise**.
	I.e. [[Mapping#A Composite Function as a Subset of Functions|Compositional Functions]], where Vector-Valued Functions are composed of Scalar-Valued Functions. 
		Normal Single Variable Derivative Rules apply for these individual component (i.e. scalar) functions.
$$\LARGE \vec{r}: [0,1] \to \mathbb{R}^3, \quad x,y,z : [0,1] \to \mathbb{R}$$
$$\LARGE \text{If all the component functions are differentiable then:}$$
$$\LARGE \vec{r}(t) = \frac{d}{dt}\vec{r} = \lim\limits_{h \to 0}\frac{\vec{r}(t+ h)-\vec{r}(t)}{h} = (x'(t), y'(t), z'(t))$$
###### *Compare to Vector-Valued [[Partial Derivatives|Multi-Variable Derivative]] (i.e. Partial Derivatives)*
$$\frac{\partial f}{\partial x} = \partial_x f(a,b) = {\partial \over \partial x}f(a,b) = f'_{x}(a,b) = f'_{1}(a,b) = \lim_{h \rightarrow 0} {f(a+h,b) - f(a,b) \over h} = g'(a)$$
![[Pasted image 20240907143354.png]]
#### Example of Vector-Valued Single Variable Derivative
$$\LARGE \vec{r}(t) = (2t+1, \sin^2t, e^t \cos t)$$
$$\LARGE = \frac{d}{dt}\vec{r}(t) = \vec{r}'(t) = (2, 2 \sin t \cos t, e^t \cos t - e^t \sin t)$$
## Tangent Vectors (i.e. Velocity Vectors)
$$\LARGE \vec{r}(t) = [x(t), y(t)], \quad \vec{r'}(t) = \vec{v}(t) = [x'(t), y'(t)]$$
The proof of the Tangent Vector Computed component wise.
![[Pasted image 20240910070247.png]]
##### The Secant Line
Recall that a $\textcolor{red}{\text{Line}}$ connecting two points is called the [[Secant Line|Secant Line]] and it is a linear function.
	I.e. Is a **straight line** (i.e. linear equation) that **intersects (i.e. cuts) a curve at two points**.
###### [[Straight Lines#The Standard Equation of a Line with Slope $m$ Passing Through a Point $(x_1, y_1)$|Point Slope Form]] Derived
1. Substitute $x_0$ for $x$ and $y_0$ for $y$ in the general equation $y = mx + b$:
$$\LARGE 1) \quad y_1 = mx_1 + b$$
2. To solve for $b$, rearrange this equation:
$$\LARGE 2) \quad  b = y_0 - mx_0$$
3. Now, substitute $b = y_0 - mx_0$ back into the general equation $y = mx + b$:
$$\LARGE 3) \quad  y = mx + (y_0 - mx_0)$$
4. Rearrange
$$\LARGE 4a) \quad  y \textcolor{yellow}{- y_0}= mx + (\cancel{y_0} - mx_0) \cancel{\textcolor{yellow}{- y_0}}$$
$$\LARGE 4b) \quad  y \textcolor{yellow}{- y_0}= \frac{\cancel{m}x - \cancel{m}x_0}{\cancel{\textcolor{yellow}{m}}} = y \textcolor{yellow}{- y_0}= m(x-x_0)$$
$$\LARGE y - y_0 = m(x - x_0)$$
$$\LARGE \frac{y - y_0}{x - x_0} = m$$
##### The Slope of the Secant Line, $m$
$$\large \text{For Vector-Valued Functions } \frac{\Delta y}{\Delta x} = \frac{y(t)-y(t_0)}{x(t)-x(t_0)} = \frac{y(t)-y(t_0)}{t-t_0} \cdot \frac{t-t_0}{x(t)-x(t_0)} $$
$$\large \text{Compared to Scalar-Valued Functions } \frac{\Delta y}{\Delta x} = \frac{f(x)-f(x_0)}{x-x_0} = {f(x+h)−f(x)​ \over h}$$

The **slope of a secant line** is the the **average rate of change** over an **interval of distance** between the chosen **points on the curve of the function**.
###### As the Difference Quotient
$$\LARGE \frac{y(t)-y(t_0)}{x(t)-x(t_0)}$$
The ratio of the change in output values to the change in the input values.
	This ratio is the slope of a linear function.
		Aka the Slope of the Secant Line.
##### The Secant Line and the Tangent Line
The Tangent of the Secant Line is the Slope of the Secant Line.
$$\LARGE \tan \alpha = \frac{\Delta y}{\Delta x}$$
![[Pasted image 20240911061758.png]]
The **Limit** of the slope of this Secant Line is the is the Slope of the $\textcolor{green}{\text{Tangent Line}}$.
	I.e. The Secant Line **becomes** the Tangent Line as $\LARGE t - t_0\to 0$, that is $\LARGE t \to t_0$
		And the Slope of that Tangent Line is the Difference Quotient of the Derivatives of each component functions.
$$\LARGE \frac{\Delta y}{\Delta x} =\frac{y(t)-y(t_0)}{t-t_0} \cdot \frac{t-t_0}{x(t)-x(t_0)} \xrightarrow{t \to t_0} \frac{y'(t_0)}{x'(t_0)}$$
$$ \text{Compared to Scalar-Valued Functions } \frac{\Delta y}{\Delta x} = \frac{f(x)-f(x_0)}{x-x_0} = {f(x+h)−f(x)​ \over h} \xrightarrow{h \to 0} f'(x)$$
![[Pasted image 20240422233019.png]]

Where the "longer" the velocity vector, the higher the speed of the movement.
	The [[Dot Product|Dot Product]] of the the position vector and the velocity vector is $\LARGE 0$.
		Therefore, they are orthogonal.
![[Pasted image 20240907144456.png]]
## Continuity and Smoothness 
The trajectory of a particle (i.e. the curve $\LARGE \vec{r}(t)$) is **smooth** if the velocity vector $\LARGE \vec{v}(t) = \vec{r}(t)$ in each point:
	1. exists (i.e. is differentiable)
	2. is non-zero
	3. is continuous

