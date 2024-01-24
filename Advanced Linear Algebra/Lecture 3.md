**Date: 1/23/2024**

**DEF :** A set of vectors is linearly dependent **iff** there are scalars at least one of which is not zero, such that $\vec{c}\cdot\vec{v} = 0$. If this is not the case, then the set of vectors is linearly independent.

**Theorem:** A set of vectors in $\mathbb{R}$ is linearly dependent **iff** at least one of them can be expressed as linear combination of the others in the set.

**Theorem:** Let vectors in $\mathbb{R}^n$ and let $A$ be the $n\times m$ matrix $\left[v_1, v_2,\dots, v_m\right]$. Then the set of vectors are linear dependent **iff** $[A|0]$ has non-trivial solutions. If all the result is 0s, then it is linear independent.

### Example Pg. 98, #24
$$\begin{bmatrix}2\\2\\1\end{bmatrix}, \begin{bmatrix}3\\1\\2\end{bmatrix}, \begin{bmatrix}1\\-5\\2\end{bmatrix}
$$
$$\left[\begin{array}{ccc|c}2&3&1&0\\2&1&-5&0\\1&2&2&0\end{array}\right] \rightarrow \left[\begin{array}{ccc|c}1&2&2&0\\0&1&3&0\\0&0&0&0\end{array}\right]$$
The matrix has non-trivial solutions, they are linearly dependent.

**Theorem**: Any set of $m$ vectors in $\mathbb{R}^n$ is linearly dependent if $m>n$.

DEF : A matrix is a rectangular array of numbers.
$$A = \begin{bmatrix}a_{11}&a_{12}&a_{13}&\dots&a_{1n}\\a_{21}&a_{22}&a_{23}&\dots&a_{2n}\\a_{31}&a_{32}&a_{33}&\dots&a_{3n}\end{bmatrix}_{m\times n}$$
$A = [a_{ij}]$, where $i$ is the row and $j$ is the column.

### Matrix Multiplication
$$C = A\times B, \ \ c_{ij} = \sum_{k=1}^{n}a_{ik}b_{kj}$$
$$A_{a\times b} \times B_{b\times c} = C_{a\times c}$$
### Matrix Exponentiation
$A^1 = A$ only if $A_{n\times n}$.
$A^2 = A\times A$
$A^k = A\times A\times\dots\times A$, $k$ times.

**DEF** : The transpose of $A_{m\times n}$ is the $n\times m$ matrix $A^T$.
$$[A^T]_{ij} = [A]_{ji}$$
**DEF** : $A_{n\times n}$ is symmetric **iff** $A=A^T$.


**DEF** : Matrices $A_1, A_2,\dots, A_k$ of same size, are said to be linearly independent if the only solution of the equation $\sum_i c_iA_i = 0$.

***Insert Properties of Matrices***

### Example P. 161, #14
$$\begin{bmatrix}1&2\\3&4\end{bmatrix}, \begin{bmatrix}2&1\\-1&0\end{bmatrix}, \begin{bmatrix}1&1\\1&1\end{bmatrix}$$
$$\left[\begin{array}{ccc|c}1&2&1&0\\2&1&1&0\\4&-1&1&0\\3&0&1&0\end{array}\right] \rightarrow \left[\begin{array}{ccc|c}3&0&1&0\\0&3&1&0\\0&0&0&0\\0&0&0&0\end{array}\right]$$
**Theorem:** 
i) If $A_{n\times n}$, then $A+A^T$ is symmetric.
Proof: $\left(A+A^T\right)^T = \left(A^T+A\right) = \left(A+A^T\right) \ \ \blacksquare$
ii) For any matrix $A$, $AA^T$ and $A^TA$ are symmetric.
Proof: $(AA^T)^T=(A^T)^TA^T = AA^T \ \ \blacksquare$
Proof: $(A^TA)^T=A^T(A^T)^T = A^TA \ \ \blacksquare$

**DEF** : The inverse of $A_{n\times n}$, $A^{-1}$ is a $n\times n$ matrix where:
$$A \ A^{-1} = A^{-1}A = \mathbb{I}$$
If $A^{-1}$ exists, then $A$ is called _invertible_.
If $A$ is invertible, then $A^{-1}$ is unique.
If $A$ is invertible, then the system of linear equations $A\vec{x}=\vec{b}$ has a unique solution.
$$\vec{x} = A^{-1}\vec{b}$$

**Theorem:** If $A = \begin{bmatrix}a&b\\c&d\end{bmatrix}$, then $A^{-1}=\dfrac{1}{ad-bc}\begin{bmatrix}d&-b\\-c&a\end{bmatrix}$.
If $\det A = 0$, then $A^{-1}$ doesn't exist ($A$ is non-invertible).
