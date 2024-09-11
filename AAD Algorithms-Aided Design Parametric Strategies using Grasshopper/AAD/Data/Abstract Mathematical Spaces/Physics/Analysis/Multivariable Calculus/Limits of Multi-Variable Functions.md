# Limits of Multi-Variable Functions
![[Pasted image 20240909160627.png]]
##### For a limit of a function with a parameter $\LARGE t \to t_0$ 
The $\LARGE \textcolor{yellow}{\text{Domain}}$ is the interval $\LARGE \textcolor{yellow}{[t_0 - \delta, t_0 + \epsilon]}$ 

###### $\LARGE \epsilon \delta$
For each $\LARGE \epsilon$ that is greater than $0$ ($\LARGE \forall \epsilon >0$) there exists some $\LARGE \delta$ that is greater than $0$ ($\LARGE \exists \delta$) with the following property: 
	For each $t$ as an element of the domain (i.e. the interval $[a,b]$ ), if only the $t$ belongs to the $\LARGE \delta$ [[Neighborhoods|neighborhood]] of $\LARGE t_0$, but is different than $\LARGE t_0$.
		Then the distance between the value of the function in the point $\LARGE t$ and the point of the limit, is less than $\LARGE \epsilon$.
## Limits of Multi-Variable Functions (i.e. vector valued functions) are Calculated Component-wise.
$$\LARGE \lim\limits_{t\to t_0}\vec{r}(t) = (x_0, y_0)$$
$$\large \lim\limits_{t\to t_0}\vec{r}(t) = (x_0, y_0) \quad\text{If and Only If}\quad x(t) - x_0 \to 0 \quad (\text{where} \space x_0 = t, \quad0 = t_0)$$
$$\large \text{And }\quad y(t) - y_0 \to 0 \quad (\text{where} \space y_0 = t, \quad 0 = t_0)$$
$$\large \text{And }\quad z(t) - z_0 \to 0 \quad (\text{where} \space z_0 = t, \quad 0 = t_0)$$

$$\large \equiv \lim\limits_{t\to t_0}x(t) = x_0 \quad \text{and} \quad \lim\limits_{y \to y_o}y(t) = y_0 =  \quad \text{and} \quad \lim\limits_{z \to z_o}z(t) = z_0$$
## If All the Component Functions have a Limit at $t_0$
Then:
$$\LARGE \lim\limits_{t \to t_0} \vec{r} = ( \lim\limits_{t \to t_0}x(t), \space \lim\limits_{t \to t_0}y(t), \space \lim\limits_{t \to t_0}z(t))$$
**Again**, Limits of multi-variable functions (i.e. vector valued functions) are calculated component-wise.
