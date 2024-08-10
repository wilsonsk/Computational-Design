# Cross Product
Given two vectors in $\mathbf{R^3}$, their cross product is a **new vector** in the $\mathbf{R^3}$.
$$\LARGE \text{If } \mathbf{u}= (u_1, u_2, u_3) \text{ and } \mathbf{v} = (v_1, v_2, v_3) \text{ are vectors in the } \mathbf{R^3}$$
$$\LARGE \text{Then their Cross Product is defined as }$$
$$\LARGE \mathbf{u} \times \mathbf{v} = (u_2v_3 - u_3v_2,\space u_3v_1 - u_1v_3,\space u_1v_2 - u_2v_1)$$
- - -
## Fake Determinant Method
Expand upon each element of the first row. 
	Easier to remember equation of Cross Product.
$$\LARGE \text{Can use a "fake" Determinant, } \mathbf{u} \times \mathbf{v} = \begin{vmatrix} \mathbf{e_1} & \mathbf{e_2} & \mathbf{e_3} \\ u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3 \end{vmatrix}$$
$$\LARGE \text{"Fake" because it does contain real numbers in each place. }$$
$$\LARGE \text{I.e. It will not produce a scalar. }$$
### Expanding
$$\LARGE \vec{e_1} \cdot \begin{vmatrix} u_2 & u_3 \\ v_2 & v_3\end{vmatrix} - \vec{e_2} \cdot \begin{vmatrix} u_1 & u_3 \\ v_1 & v_3\end{vmatrix} + \vec{e_3} \cdot \begin{vmatrix} u_1 & u_2 \\ v_1 & v_2\end{vmatrix} $$
$$\LARGE = (1, 0, 0) \cdot (u_2v_3 - u_3v_2)$$
$$\LARGE = (0, 1, 0) \cdot (u_1v_3 - u_3v_1)$$
$$\LARGE = (0, 0, 1) \cdot (u_1v_2 - u_2v_1)$$
$$\LARGE  = (u_2v_3 - u_3v_2,\space u_3v_1 - u_1v_3,\space u_1v_2 - u_2v_1) = \mathbf{u} \times \mathbf{v}$$
- - -
## Direction of New Vector
The direction is relative to "what line it is parallel to".

The direction of the new vector is **perpendicular** to both vectors.
###### If the Two Vectors are Parallel
Then the Cross Product is Zero Vector.
## Orientation of New Vector
The orientation of the new vector is based on the [[Data/Abstract Mathematical Spaces/Physics/Classical Mechanics/Newtonian Physics/Statics Analysis/Statics Analysis#Orientation and Right-Hand Rule|Right Hand Rule]].
	I.e. The two vectors and their Cross Product are oriented as the standard unit vectors $\LARGE \mathbf{i}, \mathbf{j}, \mathbf{k}$.
$$\LARGE \vec{i} = \mathbf{i} = \hat{i} = \vec{e_1} = \mathbf{e_1} = (1, 0, 0)$$
$$\LARGE \vec{j} = \mathbf{j} = \hat{j} = \vec{e_2} = \mathbf{e_2} = (0, 1, 0)$$
$$\LARGE \vec{k} = \mathbf{k} = \hat{k} = \vec{e_3} = \mathbf{e_1} = (0, 0, 1)$$
![[Pasted image 20240809061348.png]]
![[Pasted image 20240809061435.png]]
![[Pasted image 20240809061447.png]]
## Length of New Vector
The length of the new vector is equal to the **area** of the parallelogram spanned on $\mathbf{u}$ and $\mathbf{v}$.
![[Pasted image 20240809061516.png]]
![[Pasted image 20240809061208.png|300]]
## Examples
![[Pasted image 20240809063504.png]]
![[Pasted image 20240809063452.png]]
## Three Properties of Cross Product
$$\LARGE \text{If } \mathbf{u}, \mathbf{v} \in \mathbb{R}^3 \text{, then}$$
$$\LARGE \text{1. Anti=Commutativity: }\mathbf{u} \times v = - \mathbf{v} \times \mathbf{u}$$
$$\LARGE \text{2. } \mathbf{u} \cdot (\mathbf{u} \times v) = 0$$
$$\LARGE \text{3. } |\mathbf{u} \times \mathbf{v}|^2 = |\mathbf{u}|^2|\mathbf{v}|^2 - (\mathbf{u} \cdot \mathbf{v})^2$$
