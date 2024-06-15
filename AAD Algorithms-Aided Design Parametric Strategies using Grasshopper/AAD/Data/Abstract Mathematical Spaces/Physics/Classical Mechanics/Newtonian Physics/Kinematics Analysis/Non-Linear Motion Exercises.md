---
up:
  - "[[Non-Linear Motion]]"
related: 
date created: 2024-06-14
---
# Non-Linear Motion Exercises
## 1. Roller Coaster
![[Pasted image 20240614125005.png]]
###### Consider the following velocity versus time dependence of the roller coaster between $t=[0s, 16s].
$$\LARGE v(t) = -{1m \over 15s^{4}} \cdot t^{3} + {8m\over 5s^{3}} \cdot t^{2}$$
##### Did the acceleration surpass $1g = 9.81{m\over s^{2}}$ at some point of time?

##### Notes
Note the time dependent terms.

The $t^{2}$, (i.e. the quadratic - power of two dependence) is much larger than the $t^{3}$ (i.e. the cubic - power of three dependence) term, and thus **dominates** the initial output values for the smaller $t$ input values.
###### At smaller values of $t$:
- The **quadratic term** $\LARGE \frac{8 , \text{m}}{5 , \text{s}^{3}} \cdot t^{2}$ grows faster initially because for small $t$, $t^2$ will be larger relative to $t^3$ when considering their coefficients.
- Therefore, the quadratic term dominates, leading to an increase in $v(t)$.

I.e. When $t$ is small, the quadratic term ($\frac{8 , \text{m}}{5 , \text{s}^{3}} \cdot t^{2}$) will have a relatively larger effect on the velocity compared to the cubic term because $t^2$ grows slower than $t^3$.
	As a result, for small $t$, the positive quadratic term will dominate, leading to an increase in $v(t)$.
###### At larger values of $t$:
- As $T$ continues to increase, the **cubic term** $\LARGE -\frac{1 , \text{m}}{15 , \text{s}^{4}} \cdot t^{3}$ grows faster than the quadratic term because $t^3$ grows faster than $t^2$.
- Eventually, the negative cubic term will dominate over the positive quadratic term.
		But after the initial 16 values, the $t^{3}$ dominates.
			I.e. The velocity increases initially, then eventually decreases as $t$ increases. 

To see this dominance mathematically, consider the limits:
- For small $t$, $t^3$ is negligible compared to $t^2$, so the positive term dominates.
- For large $t$, the $t^3$ term, despite its smaller coefficient, will eventually outweigh the $t^2$ term because the rate of growth of $t^3$ is faster than that of $t^2$.
### Calculate the Acceleration
###### To calculate the acceleration we have to calculate the time derivative of the velocity.
Therefore, the quadratic and cubic terms must be differentiated.  
##### To Calculate the Derivative of a Polynomial
Use the [[Derivatives#Power Rule|Power Rule]].
$$\LARGE 3 \cdot -{1m\over 15s^4} \cdot t^2 + 2 \cdot {8\over 5s^3} \cdot t$$
$$\LARGE = a(t) = {dv\over dt} = v(t) = {1m \over 5s^{4}} \cdot t^{2} + {16m\over 5s^{3}} \cdot t$$
![[Pasted image 20240614220028.png|400]]

##### Answer: Did the acceleration surpass $1g = 9.81{m\over s^{2}}$ at some point of time?
###### Calculated Answer
Via examining the graph:
	Where velocity is increasing the fastest, we get a local maximum of the acceleration.
		And the corresponding value of the acceleration is above 10$m\over s^2$.
			Therefore, yes.
###### Analyzed Answer (i.e. analyzing the parabola)
Via finding **position** of the local maximum, and then what is the corresponding value of the acceleration. 
###### Find the Maximum
1. Find the **first derivative** of the acceleration.
2. Set $t = 0$.
$$\LARGE 0 = a'(t_{m}) = 2 \cdot {1\over 5s^4} \cdot t+ {16m\over 5s^3} = -{2m\over 5s^{4}} \cdot t_{m} + {16m \over 5s^3}$$ 