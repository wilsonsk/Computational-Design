# Chain Rule
## [[Mapping#A Composite Function as a Subset of Functions|Composite Functions]]
$$\LARGE f \circ g \circ h: \mathbb{R} \xrightarrow{h}\mathbb{R} \xrightarrow{g}  \mathbb{R} \xrightarrow{f} \mathbb{R}$$
$$\LARGE \frac{d}{dx}f(g(h(x))) = \frac{d}{dg(h(x))}f(g(h(x))) \cdot \frac{d}{dh(x)}g(h(x)) \cdot \frac{d}{dx}h(x)$$
$$\LARGE ==  f'(g(h(x)) \cdot g'(h(x)) \cdot h'(x)$$
## Chain Rule
The chain rule is a formula for computing the derivative of the composition (i.e. composite functions) of two or more functions.
	I.e. is a rule for computations of the [[Derivatives|derivatives]] of [[Mapping#A Composite Function as a Subset of Functions|composite functions]].
		Where the $\textcolor{yellow}{\text{derivative of a composite function}}$ is the product of the derivatives of each of the subsequent component functions. 
$$ \LARGE \textcolor{magenta}{x} \to \textcolor{orange}{x^2} \to \textcolor{green}{\sin x^2} \to \textcolor{red}{\ln(\sin x^2)} $$
$$\LARGE \textcolor{green}{\frac{d}{dx}\sin x^2 = \cos x^2}$$
$$\LARGE \textcolor{orange}{\frac{d}{dx} x^2 = 2x}$$
$$\LARGE \textcolor{magenta}{\frac{d}{dx} x = 1}$$
$$ \LARGE = \textcolor{yellow}{\frac{d}{dx}(\ln (\sin x^2))} = \textcolor{red}{\frac{1}{\sin x^2}} \cdot \textcolor{green}{\cos x^2} \cdot \textcolor{orange}{2x} \cdot \textcolor{magenta}{1}$$
In this case there are three functions which are composed with each other.
	And the chain rule gives a product of three derivatives, the most outer one, the most inner one, and all the functions in between. 
## Notation of the Four Variants of the Chain Rule
$\LARGE s$: A [[Mapping#Scalar Functions as a Subset of Functions|Real-Valued]] function (i.e. a Scalar Function) of one real variable.

$\LARGE f$: A [[Mapping#Scalar Functions as a Subset of Functions|Real-Valued]] function (i.e. a Scalar Function) of several real variables.

$\LARGE \vec{v}$: A [[Mapping#Higher-Level Functions (i.e. Composite Functions) Higher-Level Functions|Vector-Valued]] function (i.e. a Vector Function) of one real variable.

$\LARGE \phi$: A change of variables in $\LARGE \mathbb{R}^2$ or in $\LARGE \mathbb{R}^3$.
## Variant 0
The one-dimensional Chain Rule for 
$$\LARGE f \circ g : \mathbb{R} \xrightarrow{g}\mathbb{R} \xrightarrow{f}  \mathbb{R}$$
$$\LARGE \frac{d}{dx}f(g(x)) =  f'(g(x)) \cdot g'(x)$$
$$\LARGE \text{With the notation } u = f(v),\space v = g(x)$$
$$\LARGE \text{We can write } \frac{du}{dx} = \frac{du}{dv} \cdot \frac{dv}{dx}, \quad u:\mathbb{R} \to \mathbb{R}$$