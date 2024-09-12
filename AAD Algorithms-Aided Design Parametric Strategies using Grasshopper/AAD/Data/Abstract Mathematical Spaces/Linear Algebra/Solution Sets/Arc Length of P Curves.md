# Arc Length $\large l$ of Parametric Curves
$$\LARGE \vec{r}: [a,b] \to \mathbb{R}^3$$
$$\LARGE \vec{r}(t) = [x(t), y(t)], \quad \vec{r'}(t) = \vec{v}(t) = [x'(t), y'(t)]$$
$$\LARGE x,y,z: [a,b] \to \mathbb{R}$$
![[Pasted image 20240906071943.png]]
## Calculating the Length of the Arc Path
### 1. Successive Approximation of the Arc Length $\LARGE l$
By piecewise linear curves (i.e. straight line segments) aka a polygonal path.
	Where the approximation of the arc length $\LARGE l$ improves its accuracy with each successive approximation, i.e. division and summation.
##### 1. $\LARGE a \to b = l \approx l_1$ 
Measure the distance of the Secant Line (i.e. the linear function) between the starting point $\LARGE a = t_0$ and the end point $\LARGE b = t_n$.
![[Pasted image 20240912053721.png]]
##### 2. $\LARGE \frac{[a, b]}{2} = t_1, \quad a\to t_1 = l_1, \quad t_1 \to b= l_2, \quad l \approx l_1 +l_2$
Divide the interval $\LARGE [a.b]$ by $\LARGE 2$, which produces $\LARGE 2$ equal line segments within the interval
	Which also produces $\LARGE 1$ division point, $\LARGE t_1$, and thus $\LARGE 1$ additional position within the interval and along the curve, $\LARGE \vec{r}(t_1)$.
		The arc length $\LARGE l$ is now approximated by the sum of these $\LARGE 2$ line segments. 
![[Pasted image 20240912054521.png]]
$$\large 3. \quad \frac{[a, b]}{3} = t_1, t_2, \quad a\to t_1 = l_1, \quad t_1 \to t_2= l_2, \quad t_2 \to b = l_3 \quad l \approx l_1 +l_2 +l_3$$
Divide the interval $\LARGE [a.b]$ by $\LARGE 3$, which produces $\LARGE 3$ equal line segments within the interval.
	Which also produces $\LARGE 2$ division points, $\LARGE t_1, t_2$, and thus $\LARGE 2$ additional positions within the interval and along the curve, $\LARGE \vec{r}(t_1), \vec{r}(t_2)$.
		The arc length $\LARGE l$ is now approximated by the sum of these $\LARGE 3$ line segments. 
![[Pasted image 20240912055343.png]]
$$4. \quad \frac{[a, b]}{4} = t_1,t_2,t_3 \quad a\to t_1 = l_1, \quad t_1 \to t_2= l_2, \quad t_2\to t_3 = l_3 \quad t_3 \to b = l_4 \quad l \approx l_1 +l_2 +l_3 +l_4$$
Divide the interval $\LARGE [a.b]$ by $\LARGE 3$, which produces $\LARGE 4$ equal line segments within the interval.
	Which also produces $\LARGE 3$ division points, $\LARGE t_1, t_2, t_3$ and thus $\LARGE 3$ additional positions within the interval and along the curve, $\LARGE \vec{r}(t_1), \vec{r}(t_2), \vec{r}(t_3)$. 
		The arc length $\LARGE l$ is now approximated by the sum of these $\LARGE 3$ line segments. 
![[Pasted image 20240912055803.png]]
##### "Infinite" Division Points
Divide the interval $\LARGE [a.b]$ by $\LARGE n \to \infty$, which produces $\LARGE n$ equal line segments within the interval.
	Which also produces $\LARGE n-1$ division points, $\LARGE t_1, t_2, \dots , t_n$ and thus $\LARGE n-1$ additional positions within the interval and along the curve, $\LARGE \vec{r}(t_1), \vec{r}(t_2), \dots, \vec{r}(t_n)$. 
		The arc length $\LARGE l$ is now approximated by the sum of these $\LARGE n$ line segments. 
$$\LARGE l \approx \sum_{i=0}^{n}l_i$$
![[Pasted image 20240912060353.png]]
##### Expressing in terms of the Derivative (and Integral) of the Position Vectors, $\LARGE \vec{r}$
One "piece" of line segment $\LARGE l_i$, corresponds to the vector which is equal to the difference of the start and end position vectors of that specific segment.  
	Where when $\LARGE n \to \infty$ then $\LARGE \Delta t_i$ becomes a differential of infinitesimally small change, $\LARGE dt$.
		Therefore, each line segment $\LARGE l_i$ corresponds to the derivative of its associated start point $\LARGE \vec{r}(t_i)$.
			And $\LARGE |\vec{r}(t)|$ is a scalar (not a vector value) and so implies that $\LARGE |\vec{r}(t)|$ is a scalar value function, representing the length of the velocity vector. 
![[Pasted image 20240912062802.png]]