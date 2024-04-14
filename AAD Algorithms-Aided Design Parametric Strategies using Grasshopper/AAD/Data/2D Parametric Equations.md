---
up:
  - "[[Parametric Equations]]"
related:
  - "[[3D Parametric Equations]]"
  - "[[Parameters]]"
  - "[[Parametric Space]]"
  - "[[Data Relationships]]"
  - "[[Curves]]"
date created: 2024-03-20
---
# 2D Parametric Equations

## Normal Point Equation:
The normal-point equation of a line is defined by a point *q* and a non-zero vector *n* that is normal to this line
	Since *q* is on the line, any vector between it and another point of the line must be **perpendicular** to *n* and therefore, have a zeros scalar product with *vector n*.
		*vector n* * (*p*-*q*) = 0
	This equation represents a simple test using vectors and points to determine if *p* is on the line. 
		It is thus useful in parametric modelers that provide basic vector operations- no conversion to other equation forms or unpacking of vector and point components is needed.

## Parametric Equations:
Works in **both** 2D and 3D and is **constructive**- it can be used to **generate** points on the line. 
	A line is uniquely defined by a point and a vector.
		Given a point *p* and vector *v* any point *p(t)* on the line has the functional equation:
			*p(t)* = *p + t * vector v*
			Where *t* is a **parameter**, that is a real value that **scales** the vector *v*. 
			Each value of *t* represents a distinct point on the line.
			*t* is essentially a number, a scalar. 
		**Changing** the parameter t, **moves** the point p(*t*), and it specifically moves point *p(t)* **in proportion** to *t*.
			For example:
				 if *t = 0.4* then *p(t)* is 4/10ths of the **distance** along the **line** from *p0* to *p1*.
				This **linear** relationship between *t* and *p(t)* holds **only for lines**. **It does not hold for curves**.
		This is **Linear Interpolation** [[Curves#^linear-interpolation|Linear Interpolation]]
			**Systolic Array**:
				Represent a parametric line equation, that is, the **relationship** between *p(t), p0, p1, and t*.
				Comprises of three points, where the lower point is determined by the upper points and the systolic array parameter, *t*.
				The **coordinate values** from *p0* and *p1* *flow* into *p(t)*
				