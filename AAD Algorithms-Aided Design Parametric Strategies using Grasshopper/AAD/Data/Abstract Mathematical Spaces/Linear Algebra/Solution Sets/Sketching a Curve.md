# Sketching a Parametric Curve
## Three Prerequisite Tasks
$$\LARGE \text{For all, } \quad \vec{r} = (x(t), y(t)) \implies \vec{r}(t) = (x'(t), y'(t))$$
The following three Tasks need to be handled in order to sketch the curve of this vector, $\LARGE \vec{r}$. 
1. Localize some points on the curve (i.e. The Table of Values)
	The table would have rows for $\LARGE t, x, y$ and $\LARGE z$ if a 3D vector
		And $\LARGE n$ columns for $\LARGE n$ points.
1. Does the curve intersect itself? 
	In order to know this, you must solve Where $\LARGE \vec{r}(t_1) = \vec{r}(t_2)$?
3. Where do we find the [[Derivatives#Inflection Points Inflection Points (*also see* Curves Inflection Point Inflection Points in Curves)|inflection points]]?
	I.e. Where the curve "turns".
		These inflection points can be vertical or horizontal.
	Identification of Inflection Points is done by localizing the point where the tangent vectors (i.e. the velocity vectors) are vertical or horizontal.
	- Tangent vector vertical $\LARGE x'(t) = 0$ 
	- Tangent vector horizontal $\LARGE y'(t) = 0$
### 1. Localizing Some Points on the Curve (i.e. Table of Values)
$$\LARGE \text{Example Vector-Valued Function:}$$
$$\LARGE \vec{r}(t) = (t^2-4, t^3 -4t), \quad -2.5 \le t \le 2.5$$
$$\LARGE \vec{r'}(t) = (2t, 3t^2 -4), \quad -2.5 \le t \le 2.5$$
###### Start and End Points $\LARGE t_1, t_n$
![[Pasted image 20240909072247.png|400]]
###### $\LARGE t = -2, 2$
![[Pasted image 20240909072328.png|400]]
###### $\LARGE t = -1,1$
![[Pasted image 20240909072357.png|400]]
###### $\LARGE t = 0$
![[Pasted image 20240909072419.png|400]]
### 2. Curve Intersections
###### 1. Identify if there are two different parameters corresponding to the same point.
To identify, solve the following equation:
$$\LARGE \vec{r}(t_1) = \vec{r}(t_2)$$
This equation implies that the coordinates of both vectors (of differing parameters) are equal to each other.
###### 2. Translate the Equation to a System of Equations
$$\LARGE \text{The equation to translate:} \quad \vec{r}(t_1) = \vec{r}(t_2)$$
$$\LARGE \text{For vector function, } \quad \vec{r}(t) = (\textcolor{violet}{t^2-4}, \textcolor{green}{t^3 -4t}), \quad -2.5 \le t \le 2.5$$
$$\LARGE \text{Where }\quad \textcolor{violet}{x-coordinate = t^2- 4}, \quad \textcolor{green}{y-coordinate = t^3-4t}$$
$$\LARGE \begin{cases} \textcolor{violet}{t_{1}^2 - 4} = \textcolor{violet}{t_{2}^2 - 4} \\ \textcolor{green}{t_1(t_{1}^2 -4)} = \textcolor{green}{t_2(t_{2}^2 -4)} \\ t_1 < t_2 \end{cases}$$
Where $\LARGE t_1 < t_2$ is our previously stated restriction that the parameters are different, and in this case we want $t_1$ specifically less than $t2$.
###### 3. Solve the System of Equations
$$\large \begin{cases}
\textcolor{violet}{t_{1}^2 - \cancel{4}} \cancel{+4} = \textcolor{violet}{t_{2}^2 - \cancel{4}} + \cancel{4} \equiv \textcolor{violet}{t_{1}^2} - t_{2}^2= \cancel{\textcolor{violet}{t_{2}^2} - t_{2}^2} =0 \equiv (t_1-t_2)(t_1+t_2) = 0
\\ \textcolor{green}{t_1(t_{1}^2 -4)} = \textcolor{green}{t_2(t_{2}^2 -4)} \equiv \frac{\textcolor{green}{\cancel{t_1}(t_{1}^2 -4)}}{\cancel{t}} = \frac{\textcolor{green}{\cancel{t_2}(t_{2}^2 -4)}}{\cancel{t}}  \equiv (t^2 -4) = -(t^2-4) \\ \text{The only number that equals its own opposite is $0$} \implies t^2 = 4 
\\ t_1 < t_2 \\ \quad \text{ 0 product prop of the first eq and this restriction}  \implies t\neq 0 \implies t_1 = -t_2 = t
\end{cases}$$
$$\LARGE \text{Because } t^2 = 4\implies \quad \sqrt{t^\cancel{2}} = \sqrt{4}$$
$$\LARGE t_1 = -2 \quad t_2 = 2$$

In the context of our example vector function, we see that, in fact, the curve does intersect itself.
	Because we have the two values of $\LARGE t =2,-2$ where the same points are produced $\LARGE (0,0)$.
## 3. Identify the [[Derivatives#Inflection Points Inflection Points (*also see* Curves Inflection Point Inflection Points in Curves)|Inflection Points]]
##### Vertical Tangent Velocity Vector 
$$\LARGE \vec{r'}(t) = (\textcolor{violet}{2t}, \textcolor{green}{3t^2 -4}), \quad -2.5 \le t \le 2.5$$
![[Pasted image 20240909115744.png]]
$$\LARGE \text{Vertical Tangent Vector (i.e. Velocity Vector) } \quad x'(t) = 0$$
###### 1. Solve for $\LARGE x'(t) =0$ for the Vertical Tangent (Velocity) Vector
$$\LARGE x'(t) = \textcolor{violet}{2t} = 0 \Longleftrightarrow t =0$$
###### 2. Check the Table of Values where $\LARGE t=0$ to find the coordinates of $\LARGE \vec{r}(t)$ at $t=0$. 
These coordinates represent where the position vector, $\LARGE \vec{r}$ is located.
###### 3. Plugin the Identified $t$ value to $\LARGE y'(t)$ to Find Length of Vertical Velocity Vector
$$\LARGE t= 0, \quad y'(0) = 3(0)^2-4 = -4$$
![[Pasted image 20240909121233.png]]
##### Horizontal Tangent Velocity Vector 
$$\LARGE \vec{r'}(t) = (\textcolor{violet}{2t}, \textcolor{green}{3t^2 -4}), \quad -2.5 \le t \le 2.5$$
![[Pasted image 20240909115744.png]]
$$\LARGE \text{Horizontal Tangent Vector (i.e. Velocity Vector) } \quad y'(t) = 0$$
###### 1. Solve for $\LARGE y'(t) =0$ for the Horizontal Tangent (Velocity) Vector
$$\large y'(t) = \textcolor{green}{3t^2-4} = 0 \equiv \sqrt{t^\cancel{2}} =\sqrt{\frac{-4}{3}} \quad \Longleftrightarrow \quad t =\frac{2}{\sqrt{3}} \text{ or } t = -\frac{2}{\sqrt{3}}$$
###### 2. Check the Table of Values (Or In This Case, Compute the Coordinates) where $\LARGE t = \frac{2}{\sqrt{3}}, t = -\frac{2}{\sqrt{3}}$ to find the coordinates of $\LARGE \vec{r}(t) = (x(t), y(t))$
$$\LARGE x(t)=t^2-4, \quad t = -\frac{2}{\sqrt{3}}: \quad -(\frac{2}{\sqrt{3}})^2 -4 = -2.66$$
$$\LARGE y(t)=t^3-4t, \quad t = -\frac{2}{\sqrt{3}}: \quad -(\frac{2}{\sqrt{3}})^3 -4(\frac{-2}{\sqrt3}) = 3.1$$
$$\LARGE x(t)=t^2-4, \quad t = -\frac{2}{\sqrt{3}}: \quad -(\frac{2}{\sqrt{3}})^2 -4 = -2.66$$
$$\LARGE y(t)=t^3-4t, \quad t = \frac{2}{\sqrt{3}}: \quad -(\frac{2}{\sqrt{3}})^3 -4(\frac{2}{\sqrt3}) = -3.1$$
These coordinates represent where the position vector, $\LARGE \vec{r}$ is located.
###### 3. Plugin the Identified $t$ value to $\LARGE x'(t)$ to Find Length of Horizontal Velocity Vector
$$\LARGE t= 0, \quad x'(-\frac{2}{\sqrt3}) = 2(-\frac{2}{\sqrt3}) = -2.3$$
$$\LARGE t= 0, \quad x'(\frac{2}{\sqrt3}) = 2(\frac{2}{\sqrt3}) = 2.3$$
![[Pasted image 20240909160054.png]]