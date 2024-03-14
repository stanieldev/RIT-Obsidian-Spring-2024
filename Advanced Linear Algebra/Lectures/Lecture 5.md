**Date: 1/30/2024**
<hr>

### Example Pg. 190 #9
$$\begin{bmatrix}1&0&0\\0&1&0\\0&-3&1\end{bmatrix}\begin{bmatrix}1&0&0\\0&1&0\\-8&0&1\end{bmatrix}\begin{bmatrix}1&0&0\\-4&1&0\\0&0&1\end{bmatrix}\begin{bmatrix}1&2&3\\4&5&6\\7&8&9\end{bmatrix} = \begin{bmatrix}1&2&3\\0&-3&-6\\0&0&3\end{bmatrix}$$
$$L = \begin{bmatrix}1&0&0\\-4&1&0\\0&0&1\end{bmatrix}^{-1}\begin{bmatrix}1&0&0\\0&1&0\\-8&0&1\end{bmatrix}^{-1}\begin{bmatrix}1&0&0\\0&1&0\\0&-3&1\end{bmatrix}^{-1}$$
$$\boxed{L = \begin{bmatrix}1&0&0\\4&1&0\\8&3&1\end{bmatrix}, \ \ \ U = \begin{bmatrix}1&2&3\\0&-3&-6\\0&0&3\end{bmatrix}}$$


DEF : A subspace of $\mathbb{R}^n$ is any collection $S$ of vectors in $\mathbb{R}^n$ such that:
i) The zero-vector is in $S$.
ii) If $u,v$ is in $S$, then $u+v$ is in $S$.
iii) If $u$ is in $S$, then any scalar multiple $cu$ is in $S$.

Theorem: If $v_1, v_2,\dots v_k$ are vectors in $\mathbb{R}^n$, then $\mathrm{Span}(v_1, v_2,\dots v_k)$ is a subspace of $\mathbb{R}^n$.

DEF : Given $A_{m\times n}$, the row space of $A$ is the subspace $\mathrm{row}(A)$ spanned by the rows of $A$ and column space is spanned by the columns of $A$.
 - If $B$ is row-equivalent to $A$, then $\mathrm{row}(B)=\mathrm{row}(A)$.

DEF : Given $A_{m\times n}$, the null space of $A$, denoted $\mathrm{null}(A)$, is the subspace of $\mathbb{R}^n$ consisting of the solutions of $A\vec{x} = \vec{0}$.

Theorem: If $A$ is a matrix with real entries and $A\vec{x}=\vec{b}$ is a system of linear equations, the one of the following is true.
1) There is no solution.
2) There is a unique solution.
3) There are infinitely many solutions.

DEF : A basis for a subspace of $\mathbb{R}^n$ is a set of vectors in $S$ that:
i) Span S
ii) Linear Independent

### Example
Given $A = \begin{bmatrix}1&1&3&1&6\\2&-1&0&1&-1\\-3&2&1&-2&1\\4&1&6&1&3\end{bmatrix}$, find basis for $\mathrm{row}(A), \mathrm{col}(A), \mathrm{null}(A)$
$$A\rightarrow \begin{bmatrix}1&0&1&0&-1\\0&1&2&0&3\\0&0&0&1&4\\0&0&0&0&0\end{bmatrix}$$
A basis for $\mathrm{row}(A)$ is $\left\{ \ \begin{bmatrix}1&0&1&0&-1\end{bmatrix}, \begin{bmatrix}0&1&2&0&3\end{bmatrix}, \begin{bmatrix}0&0&0&1&4\end{bmatrix} \ \right\}$

Using RREF, only the columns who's rows start with $1$, then use the original matrix.
A basis for $\mathrm{col}(A)$ is $\left\{\begin{bmatrix}1\\2\\-3\\4\end{bmatrix}, \begin{bmatrix}1\\-1\\2\\1\end{bmatrix}, \begin{bmatrix}1\\1\\-2\\1\end{bmatrix}\right\}$
To find null space, use the RREF as an augmented matrix with the vector $\vec{0}$.
$$[A|0]\rightarrow\left[\begin{array}{ccccc|c}1&0&1&0&-1&0\\0&1&2&0&3&0\\0&0&0&1&4&0\\0&0&0&0&0&0\end{array}\right]$$
There are 5 columns, rank 3, and so there are 2 free variables.
Letting $x_3$ and $x_5$ being the free variable, since they have trailing numbers after their value of 1 and no 1 underneath it.
$\vec{x}=\begin{bmatrix}-x_3+x_5\\-2x_3-3x_5\\x_3\\-4x_5\\x_5\end{bmatrix} = x_3\begin{bmatrix}-1\\-2\\1\\0\\0\end{bmatrix} + x_5\begin{bmatrix}1\\-3\\0\\-4\\1\end{bmatrix}$
So a basis for $\mathrm{null}(A) = \left\{ \begin{bmatrix}-1\\-2\\1\\0\\0\end{bmatrix} + \begin{bmatrix}1\\-3\\0\\-4\\1\end{bmatrix} \right\}$

How to find $\mathrm{row}(A), \mathrm{col}(A), \mathrm{null}(A)$:
1) Find the RREF (defined as matrix $R$).
2) Basis for $\mathrm{row}(A)$ is the non-zero vectors of $R$ containing 1's.
3) Basis for $\mathrm{col}(A)$ is the column vectors of $A$ that correspond to the columns of $R$ containing leading 1's.
4) Basis for $\mathrm{null}(A)$, solve for the leading variables of $[R|0]$. Factor the vectors in terms of free parameters, leaving the vectors for the basis of null.

### Example Pg. 210 #18
$$A = \begin{bmatrix}1&1&-3\\0&2&1\\1&-1&-4\end{bmatrix} \rightarrow R = \begin{bmatrix}1&0&-7/2\\0&1&1/2\\0&0&0\end{bmatrix}$$
$$\begin{align}
\mathrm{row}(A) &= \left\{ \ \begin{bmatrix}1&0&-7/2\end{bmatrix}, \ \begin{bmatrix}0&1&1/2\end{bmatrix} \ \right\} \\
 &= \left\{ \ \begin{bmatrix}2&0&-7\end{bmatrix}, \ \begin{bmatrix}0&2&1\end{bmatrix} \ \right\}
\end{align}$$
$$\begin{align}
\mathrm{col}(A) &= \left\{ \begin{bmatrix}1\\0\\1\end{bmatrix}, \begin{bmatrix}1\\2\\-1\end{bmatrix} \right\}
\end{align}$$
$$\begin{align}
\mathrm{null}(A) = \left[\begin{array}{ccc|c}2&0&-7&0\\0&2&1&0\\0&0&0&0\end{array}\right]
= \left\{ \begin{bmatrix}7\\-1\\2\end{bmatrix} \right\}
\end{align}$$

Basis Theorem: If $S$ is a subspace of $\mathbb{R}^n$, then any two bases of $S$ has the same number of vectors.

Theorem: Given a matrix $A_{m\times n}$, $\mathrm{dim\ row}(A) = \mathrm{dim\ col}(A) = \mathrm{rank}(A)$.

Theorem: $\mathrm{rank}\left(A^T\right) = \mathrm{rank}(A)$.

DEF : $\mathrm{Nullity}(A) = \mathrm{dim\ null}(A)$, equal to the number of free variables.

Rank Theorem: For $A_{n\times m}$, $\mathrm{rank}(A)+\mathrm{nullity}(A) = n$.

Theorem: Given $A_{m\times n}$:
i) $\mathrm{rank}(A) = \mathrm{rank}\left(A^TA\right)$.
ii) $A^TA$ is invertible **iff** $\mathrm{rank}(A)=n$.

### Fundamental Theorem of Invertible Matrices
Given matrix $A_{n\times n}$, the following are equivalent:
1) A is invertible.
2) $A\vec{x}=\vec{b}$ has a unique solution in $b\in\mathbb{R}^n$.
3) $A\vec{x}=\vec{0}$ has only the trivial solution.
4) The RREF of $A$ is $\mathbb{I}$.
5) $A$ is the product of elementary matrices.
6) $\mathrm{rank}(A)=n$
7) $\mathrm{nullity}(A)=0$
8) The column vectors of $A$ are linearly independent.
9) The column vectors of $A$ span $\mathbb{R}^n$.
10) The column vectors of $A$ form a basis in $\mathbb{R}^n$.
11) The row vectors of $A$ are linearly independent.
12) The row vectors of $A$ span $\mathbb{R}^n$.
13) The row vectors of $A$ form a basis in $\mathbb{R}^n$.

Theorem: If $S$ is a subspace of $\mathbb{R}^n$, $\mathbb{B}=\{v_1, v_2,\dots,v_k\}$ is a basis for $S$, then every vector $v$ in $S$ has exactly one linear representation, meaning it can be represented as:
$$\vec{v} = \sum c_i v_i$$


### Homework
Sec 3.3: 6,26,28,50,52
Sec 3.4: 4,8,10
**Sec 3.5: 6,16,18,29,30,36,46,48**
