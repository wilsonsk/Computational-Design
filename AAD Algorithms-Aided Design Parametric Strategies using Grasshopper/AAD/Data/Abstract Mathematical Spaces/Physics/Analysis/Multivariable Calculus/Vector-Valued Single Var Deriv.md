# Vector-Valued Single Variable Derivatives
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
Where the "longer" the velocity vector, the higher the speed of the movement.
	The [[Dot Product|Dot Product]] of the the position vector and the velocity vector is $\LARGE 0$.
		Therefore, they are orthogonal.
![[Pasted image 20240907144456.png]]
## Continuity and Smoothness 
The trajectory of a particle (i.e. the curve $\LARGE \vec{r}(t)$) is **smooth** if the velocity vector $\LARGE \vec{v}(t) = \vec{r}(t)$ in each point:
	1. exists (i.e. is differentiable)
	2. is non-zero
	3. is continuous

