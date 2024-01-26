**Date: 1/25/2024**
<hr>
### Inverse Matrix Properties
If $A$ and $B$ are $n\times n$ invertible matrices and $c$ is a scalar, then:
$$\begin{align}
\left(A^{-1}\right)^{-1} &= A \\
\left(cA\right)^{-1} &= \dfrac{1}{c}A^{-1} \\
\left(A\times B\right)^{-1} &= B^{-1}A^{-1} \\
\left(A^{T}\right)^{-1} &= \left(A^{-1}\right)^{T} \\
\left(A^{n}\right)^{-1} &= \left(A^{-1}\right)^{n} \\
\end{align}$$
<hr>
### Elementary Matrices
An *elementary matrix* is a matrix that can be obtained by performing an elementary row operation on an identity matrix.
To achieve an elementary row operation on $A$, we multiply by an elementary matrix on the left.
All elementary matrices have inverses that are equivalent to their inverse row operation.
#### Example
Express $\begin{bmatrix}2&3\\1&3\end{bmatrix}$ as a product of elementary matrices.
$$\begin{bmatrix}1&0\\0&-1/3\end{bmatrix}\begin{bmatrix}1&1\\0&1\end{bmatrix}\begin{bmatrix}1&0\\-2&1\end{bmatrix}\begin{bmatrix}0&1\\1&0\end{bmatrix}\begin{bmatrix}2&3\\1&3\end{bmatrix} = \mathbb{I}$$
$$\begin{bmatrix}1&0\\0&-1/3\end{bmatrix}\begin{bmatrix}1&1\\0&1\end{bmatrix}\begin{bmatrix}1&0\\-2&1\end{bmatrix}\begin{bmatrix}0&1\\1&0\end{bmatrix} = \begin{bmatrix}2&3\\1&3\end{bmatrix}^{-1}$$
#### Connection to Matrix Inverses
If a sequence of elementary row operations reduces a matrix $A$ to the identity $\mathbb{I}$, then the same sequence of elementary row operations transforms $I$ into $A^{-1}$.
 - This is the Gauss-Jordan method for computing $A^{-1}$.

<hr>
### Gauss-Jordan Method for $A^{-1}$
$$\left[A_{n\times n}|\mathbb{I}_{n\times n}\right] \rightarrow \left[\mathbb{I}_{n\times n}|A_{n\times n}^{-1}\right]$$
#### Gauss-Jordan Example
Given $A = \begin{bmatrix}1&2&-1\\2&2&4\\1&3&-3\end{bmatrix}$, find $A^{-1}$.
$$\left[\begin{array}{ccc|ccc}1&2&-1&1&0&0\\2&2&4&0&1&0\\1&3&-3&0&0&1\end{array}\right] \rightarrow
\left[\begin{array}{ccc|ccc}1&0&0&9&-3/2&-5\\0&1&0&-5&1&3\\0&0&1&-2&1/2&1\end{array}\right]$$
$$A^{-1}=\dfrac{1}{2}\left[\begin{array}{ccc}18&-3&-10\\-10&2&6\\-4&1&2\end{array}\right]$$
<hr>
### Fundamental Theorem of Invertible Matrices
Let $A_{n\times n}$ be given, then the following is equivalent.
  i) $A$ is invertible.
 ii) $A\vec{x}=\vec{b}$ has a unique solution in $\mathbb{R}^n$.
iii) $A\vec{x}=\vec{0}$ has a only the trivial solution.
iv) The RREF of $A$ is $I_{n\times n}$.
 v) $A$ is a product of elementary matrices.
**THIS IS 10% OF THE FINAL RIGHT HERE**

<hr>
### LU Factorization
It is helpful to factor a matrix and write it as the a product of other matrices.
There are 2 kinds of matrices: Upper Triangular ($U$) and Lower Triangular ($L$).
#### Definition
Given $A_{n\times n}$, a factorization $A = LU$, where $L$ is unit lower triangular and $U$ is upper triangular, is called an LU Factorization.
#### Example
$$\begin{bmatrix}3&-1\\9&5\end{bmatrix} = \begin{bmatrix}1&0\\3&1\end{bmatrix}\begin{bmatrix}3&-1\\0&2\end{bmatrix}$$
$$\begin{bmatrix}1&2\\-3&-1\end{bmatrix} = \begin{bmatrix}1&0\\-3&1\end{bmatrix}\begin{bmatrix}1&2\\0&5\end{bmatrix}$$
Using Elementary Row Operations, you can solve for $A$. Solve for $U$ first, and the elementary matrices outside will be $L$.

#### Example Pg. 189 #3
$$A = \begin{bmatrix}2&1&-2\\-2&3&-4\\4&-3&0\end{bmatrix}, \ \ L = \begin{bmatrix}1&0&0\\-1&1&0\\2&-5/4&1\end{bmatrix}, \ \  U = \begin{bmatrix}2&1&-2\\0&4&-6\\0&0&-7/2\end{bmatrix}, \ \ \vec{b} = \begin{bmatrix}-3\\1\\0\end{bmatrix}$$
Use $L$ to solve for $A\vec{x}=\vec{b}$, and the solutions use as the input vector for $U$.
Effectively, doing 1 matrix at a time with diagonals so it's much faster.

<hr>
### Homework
Sec 3.3: 6,26,28,50,52
Sec 3.4: 4,8,10
