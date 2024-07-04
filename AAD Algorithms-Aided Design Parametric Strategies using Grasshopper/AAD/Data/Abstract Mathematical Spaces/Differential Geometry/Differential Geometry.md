# Differential Geometry
Differential geometry is a branch of mathematics that uses techniques of calculus and linear algebra to study geometric problems. 
	It focuses on the properties of curves, surfaces, and more general geometric structures that are smooth (i.e., [[Derivatives#Differentiable Function|differentiable]]).

The term "**[[Derivatives#Differential|differential]]**" refers to a [[Linear Mapping|linear map]] that approximates how [[Mapping|functions]] or maps change in a smooth and consistent manner at an infinitesimal level.
	This concept is central to understanding how [[Curves|curves]] and [[Surfaces|surfaces]] behave and interact locally.
## Curve
Curve defined as a differentiable map $\LARGE \alpha$ of an open interval $\LARGE I = (a,b)$ of the real line $\LARGE R$ into $\LARGE R^3$.
$$\LARGE \alpha: I \to \mathbb{R}^3$$

#### Map $\LARGE \alpha : I \to R^3$
Is a function that assigns to each real number $t \in I$ a point $\alpha(t)$ in three-dimensional space.
	The notation $\alpha: I \to \mathbb{R}^3$ specifies that $\alpha$ is a map (function) from the set $I$ to the set $\mathbb{R}^3$.
#### The Domain $R$, Open Interval $\LARGE I = (a,b)$
$I$ is an open interval on the real line $\mathbb{R}$. 
	This means it includes all real numbers between $a$ and $b$, but not the endpoints $a$ and $b$ themselves.
	
This interval $I$ serves as the domain of the function $\alpha$.
	This means that $\alpha$ takes values from within this interval.
	
The domain of $\alpha$ is an interval on the real line, meaning $\alpha$ takes values from a continuous set of real numbers between $a$ and $b$, not including $a$ and $b$.
#### Superset of the Domain , $\LARGE\mathbb{R}$ (i.e. Real Line)
The real line $\mathbb{R}$ is the set of all real numbers.
	In this context, it emphasizes that $I$ is a subset of the real numbers.
	
It extends infinitely in both positive and negative directions.
	It can be visualized as a continuous, one-dimensional line where every point on the line corresponds to a real number.
###### Into the Codomain, $\LARGE \mathbb{R}^3$
This part indicates that the function $\alpha$ maps points from the interval $I$ to points in three-dimensional space $\mathbb{R}^3$.

The codomain is three-dimensional space, meaning $\alpha$ produces points with three coordinates $(x(t), y(t), z(t))$.
##### "Parametrized" means the curve is described using a parameter (typically $t$).
##### "Differentiable" means that the function describing the curve is smooth and has derivatives.

## Key Components of Differential Geometry
#### Parametrization
Parametrization is the process of defining a curve by expressing its coordinates as functions of one or more parameters.
	***Example***: For a circle of radius $R$, a common parametrization is 
	$$(x(t), y(t)) = (R \cos(t), R \sin(t))$$
	where $t$ is the parameter.
#### Curves and Surfaces
###### Curves
One-dimensional objects in space, like the path of a moving point.
###### Surfaces
Two-dimensional objects, like the skin of a 3D shape.
#### Smoothness and Differentiability
###### Smoothness
A smooth curve or surface has no sharp edges or breaks; it's continuously differentiable.
###### Differentiability
A function is differentiable if it has a derivative at each point, which means it can be approximated by a tangent line or plane at very small scales.
#### Tangent Spaces
###### Tangent Space
At any point on a smooth curve or surface, the tangent space is a linear approximation of the geometry at that point. It's essentially the best flat surface that approximates the curve or surface locally.
#### Curvature
###### Curvature
Measures how much a curve deviates from being a straight line, or a surface deviates from being a plane.
###### Types of Curvature
Includes Gaussian curvature (intrinsic curvature) and mean curvature (extrinsic curvature).
#### Metrics
###### Metric
Defines the distance between points on a curve or surface. In differential geometry, metrics help quantify how shapes change and deform.