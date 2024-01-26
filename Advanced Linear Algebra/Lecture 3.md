**Date: 1/23/2024**
<hr>
### Vector Linear Independence
A set of vectors are linearly independent if it is not possible to represent any vector as a linear combination of the remaining vectors in the set.

**Theorem:** A set of vectors in $\mathbb{R}$ is linearly dependent **iff** at least one of them can be expressed as linear combination of the others in the set.

**Theorem:** Let vectors in $\mathbb{R}^n$ and let $A$ be the $n\times m$ matrix $\left[v_1, v_2,\dots, v_m\right]$. Then the set of vectors is linear dependent **iff** $[A|0]$ has non-trivial solutions. This is identical to saying that no linear combinations of vector returns to the origin.

**Theorem**: Any set of $m$ vectors in $\mathbb{R}^n$ is linearly dependent if $m>n$.

<hr>
### Matrix Operations
#### Matrix Multiplication
In linear algebra, *matrix multiplication* is the process of combining 2 matrix through multiplication.
The operation is defined as:
$$C = A\times B, \ \ c_{ij} = \sum_{k=1}^{n}a_{ik}b_{kj}$$

**Theorem:** If $A$ is a matrix of size $n\times m$ and matrix $B$ is a matrix of size $m\times l$, then the resulting product $C = A\times B$ will be of size $n\times l$. If matrices do not match this scheme, then it is not possible to multiply $A\times B$.
#### Matrix Exponentiation
The process of *matrix exponentiation* is similar to that of real numbers, where it is the repeated multiplication of the same matrix.
$A^1 = A$ only if $A_{n\times n}$.
$A^2 = A\times A$
$A^k = A\times A\times\dots\times A$, $k$ times.

**Theorem:** Given a matrix $A$, $A^k$ where $k\ne1$ exists **iff** the size of $A$ takes the form of $n\times n$.

<hr>
### Matrix Properties
#### Matrix Transpose
The transpose of $A_{m\times n}$ is the $n\times m$ matrix $A^T$ taking the form of:
$$[A^T]_{ij} = [A]_{ji}$$
#### Symmetric Matrix
A *symmetric matrix* is a matrix where $A=A^T$.
 - The size of $A$ must be square ($n\times n$).

**Theorem:** 
i) If $A_{n\times n}$, then $A+A^T$ is symmetric.
Proof: $\left(A+A^T\right)^T = \left(A^T+A\right) = \left(A+A^T\right) \ \ \blacksquare$
ii) For any matrix $A$, $AA^T$ and $A^TA$ are symmetric.
Proof: $(AA^T)^T=(A^T)^TA^T = AA^T \ \ \blacksquare$
Proof: $(A^TA)^T=A^T(A^T)^T = A^TA \ \ \blacksquare$

### Matrix Linear Independence
A set of matrices of same size are said to be linear independent if it is not possible to represent any other matrix as a linear combination of the remaining matrices in the set.

**Theorem:** A set of matrices are linearly dependent **iff** $\sum_i c_iA_i = 0$ has non-trivial solutions.

### Matrix Inverse
The inverse of $A_{n\times n}$, $A^{-1}$, is a $n\times n$ matrix where:
$$A \ A^{-1} = A^{-1}A = \mathbb{I}$$
**Theorems:**
1) If $A^{-1}$ exists, then $A$ is called _invertible_.
2) If $A$ is invertible, then $A^{-1}$ is unique.
3) If $A$ is invertible, then the system $A\vec{x}=\vec{b}$ has a unique solution $\vec{x} = A^{-1}\vec{b}$.

**Theorem:** If $A = \begin{bmatrix}a&b\\c&d\end{bmatrix}$, then $A^{-1}=\dfrac{1}{ad-bc}\begin{bmatrix}d&-b\\-c&a\end{bmatrix}$.
 - If $\det A = 0$, then $A^{-1}$ doesn't exist ($A$ is non-invertible).

<hr>
