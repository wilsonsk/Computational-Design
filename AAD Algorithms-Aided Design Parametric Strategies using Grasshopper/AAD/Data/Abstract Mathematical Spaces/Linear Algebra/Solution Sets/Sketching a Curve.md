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
### Localizing Some Points on the Curve (i.e. Table of Values)
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
### Curve Intersections
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
\\ \textcolor{green}{t_1(t_{1}^2 -4)} = \textcolor{green}{t_2(t_{2}^2 -4)} \equiv \frac{\textcolor{green}{\cancel{t_1}(t_{1}^2 -4)}}{\cancel{t}} = \frac{\textcolor{green}{\cancel{t_2}(t_{2}^2 -4)}}{\cancel{t}}  \equiv (t^2 -4) = -(t^2-4)
\\ t_1 < t_2  \text{ 0 product prop of the first eq and this restriction}  \implies t\neq 0 \implies t_1 = -t_2 = t
\end{cases}$$


In the context of our example vector function, we see that, in fact, the curve does intersect itself.
	Because we have the 