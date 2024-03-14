**Date: 2/1/2024**
<hr>

### Matrix Determinants

#### Examples of standard sides
Given $A = \begin{bmatrix}a_{11}&a_{12}\\a_{21}&a_{22}\end{bmatrix}$, $\det A = |A| = a_{11}a_{22} - a_{12}a_{21}$.
Given $A = \begin{bmatrix}a_{11}&a_{12}&a_{13}\\a_{21}&a_{22}&a_{23}\\a_{31}&a_{32}&a_{33}\end{bmatrix}$, $\det A = |A| = a_{11}\left|\begin{array}{cc}a_{22}&a_{23}\\a_{32}&a_{33}\end{array}\right| - a_{12}\left|\begin{array}{cc}a_{21}&a_{23}\\a_{31}&a_{33}\end{array}\right| + a_{13}\left|\begin{array}{cc}a_{21}&a_{22}\\a_{31}&a_{32}\end{array}\right|$.
The choice of coefficients are arbitrary, and can be any column or row.


DEF: Given $A_{n\times n}$, we define the determinant as:
$$\det A = \sum_{i=1}^n\sum_{j=1}^n a_{ij}C_{ij} = \sum_{i=1}^n\sum_{j=1}^n (-1)^{i+j} a_{ij}\det A_{ij}$$

Theorem: The determinant of any triangular matrix is the product of the diagonal matrices.

#### Properties of Determinants
1) If $A$ has a zero row or column, $\det A = 0$.
2) If $B$ is obtained by interchanging rows or columns of $A$, then $\det B = -\det A$.
3) If $A$ has 2 identical rows or columns, $\det A = 0$.
4) If $B$ is obtained by multiplying a row or column of $A$ by $k$, then $\det B = k\det{A}$
5) If $A, B, C$ are identical except that the i-th row or column of $C$ is the sum of i-th row or column of $A$ and $B$, then $\det C = \det A + \det B$.
6) If $B$ is obtained by adding a multiple of 1 row or column of $A$, $\det B = \det A$.
#### Facts of Determinants
1) $|A| = 0$ iff $A$ is not invertible.
2) $|A| \ne 0$ iff $A$ is invertible.
3) Given $A, B$, then $\det(A\times B) = \det(A)\times \det(B)$.
4) Given $A_{n\times n}$, $\det(kA) = k^n\det(A)$.
5) If $A$ is invertible, $\det\left(A^{-1}\right) = \dfrac{1}{\det(A)}$.
6) Given $A$, $\det\left(A^T\right) = \det(A)$.

### Cramer's Rule
Given $A_{n\times n}$ and $\vec{b} \in \mathbb{R}^n$, the unique solutions of the system $A\vec{x}=\vec{b}$ is given by:
$$x_i = \dfrac{|A_i(\vec{b})|}{|A|}$$
Where $A_i(\vec{b})$ is replacing column $i$ with the vector $\vec{b}$.
### Inverse Matrices using Determinants
Def: Given $A_{n\times n}$, the *adjoint* of $A$ is defined as:
$$\mathrm{adj}(A)_{ij} = C_{ji}$$
$$\mathrm{adj}(A) = A^{-1}\det(A)$$




