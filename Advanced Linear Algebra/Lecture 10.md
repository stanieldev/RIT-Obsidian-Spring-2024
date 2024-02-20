**Date: 2/20/2024**



Homework:
4.5, 1-10, 47-50

Solving for a characteristic equation is impractical.
Computation of a determinant is time-consuming.
There are no formulas for solving polynomials of degree 5 or more.
Approximating roots of polynomials are sensitive to round-off.
 - Let's bypass the characteristic polynomial.

Let's approximate an eigenvector first and use it to find a corresponding eigenvalue.


### Algorithm for Finding Eigenvalues

**DEF:** The dominant eigenvalue, $\lambda_1$ , of matrix $A_{n\times n}$ , is the eigenvalue with the largest absolute value among the rest of the eigenvalues.

Let's, iteratively, produce a sequences of scalars that converge to $\lambda_1$ , and a sequence of vectors that converge to the dominant eigenvalue.

**Theorem:** If $A_{n\times n}$ is diagonalizable with dominant eigenvalue $\lambda_1$ , then there exists a non-zero vector $\vec{x}_0$ such that the sequence of $\vec{x}_k$ defined by $\vec{x}_{k+1}=A\vec{x}_k$, that $\vec{x}_k\approx A\vec{x}_k$.

#### Example: Find the dominant eigenvector

$A = \begin{bmatrix}1&1\\2&0\end{bmatrix}, \ \ \ \vec{x_0} = \begin{bmatrix}1\\0\end{bmatrix}$

| $k$ | $0$ | $1$ | $2$ | $3$ | $4$ | $5$ | $\dots$ | $n\rightarrow\infty$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $\vec{x}_k$ | $\begin{bmatrix}1\\0\end{bmatrix}$ | $\begin{bmatrix}1\\2\end{bmatrix}$ | $\begin{bmatrix}3\\2\end{bmatrix}$ | $\begin{bmatrix}5\\6\end{bmatrix}$ | $\begin{bmatrix}11\\10\end{bmatrix}$ | $\begin{bmatrix}21\\22\end{bmatrix}$ | $\dots$ | $\approx t\begin{bmatrix}1\\1\end{bmatrix}$ |
We can say relatively confidently that $\vec{\lambda}=\dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\1\end{bmatrix}$, $\lambda = 2$.
The eigenvector values come from the ratio of components.
The eigenvalue comes from the scale factor at the end of the matrix multiplications.


#### Constraints
**Warning:** As the components of $\vec{x}_k$ gets large very quickly, significant round-off errors occur.
To fix, we use *scaling*: Replacing $\vec{y}_k=\dfrac{1}{m_k}\vec{x}_k$ , where $m_k$ is the largest absolute component of $\vec{x}_k$.


#### Example: Find the dominant eigenvector (scaling)

$A = \begin{bmatrix}1&1\\2&0\end{bmatrix}, \ \ \ \vec{x_0} = \begin{bmatrix}1\\0\end{bmatrix}$

| $k$ | $0$ | $1$ | $2$ | $3$ | $4$ | $5$ | $\dots$ | $n\rightarrow\infty$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $\vec{x}_k$ | $\begin{bmatrix}1\\0\end{bmatrix}$ | $\begin{bmatrix}0.5\\1\end{bmatrix}$ | $\begin{bmatrix}1\\0.667\end{bmatrix}$ | $\begin{bmatrix}0.883\\1\end{bmatrix}$ | $\begin{bmatrix}1\\0.909\end{bmatrix}$ | $\begin{bmatrix}0.995\\1\end{bmatrix}$ | $\dots$ | $\begin{bmatrix}1\\1\end{bmatrix}$ |


### Power Method
Let $A$ be a diagonalizable $n\times n$ matrix with a dominant eigenvalue $\lambda_1$.
1) Let $\vec{x}_0=\vec{y}_0$ be the initial vector in $\mathbb{R}^n$ whose largest component is 1.
2) Use the recursion $\vec{x}_k = A\vec{y}_{k-1}$ , where $m_k$ is the largest absolute component of $\vec{x}_k$.
3) Set $\vec{y}_k = \dfrac{1}{m_k}\vec{x}_k$.
DEF : Let $A_{n\times n}$ be a real or complex matrix and define the Gerschgorin disk $D_i$ to be the circle centered at $a_{ij}$ having radius $r_i = \sum_{i\ne j} |a_ij|$.


### Gerschgorin Disk Theorem
Eigenvalues of $A_{n\times n}$ are contained within Gerschgorin Disks.

#### Example: Find the dominant eigenvector (Gerschgorin Disk Theorem)

$A = \begin{bmatrix}2&1&0\\0.5&6&0.5\\2&0&8\end{bmatrix}$

$x = 2$, $r = |1| + |0| = 1$
$x = 6$, $r = |0.5| + |0.5| = 1$
$x = 8$, $r = |2| + |0| = 2$

