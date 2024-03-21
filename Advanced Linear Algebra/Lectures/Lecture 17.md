
Exam #2 : March 28th, 2024



Theorem: Let $B$ be a basis for vector space $V$.
1) Any set more than $n$ vectors in $V$ is linearly dependent.
2) Any set of fewer than $n$ vectors cannot span $V$.

Basis Theorem: If a basis for $V$ has $n$ vectors, then every basis for $V$ has $n$ vectors.
$$\mathrm{dim}(V)= \#\mathrm{\ of\ vectors\ in\ any\ basis}$$

Theorem : Let $V$ be a vector space with $\mathrm{dim}(V)=n$
1) Any linearly independent set in $V$ contains $n$ or fewer vectors.
2) Any spanning set for $V$ has at least $n$ vectors.
3) Any $n$ linearly independent vectors form a basis.
4) Any $n$ spanning set of vectors form a basis.
5) Any linearly independent set can be extended to a basis.
6) Any spanning set can be reduced to a basis.

#### Pg. 456 #1
Start with a vector space $\mathbb{R}^{2\times2}$ :
$$\left\{\begin{bmatrix}1&1\\0&-1\end{bmatrix}, \begin{bmatrix}1&-1\\1&0\end{bmatrix}, \begin{bmatrix}1&0\\3&2\end{bmatrix}\right\}$$
$$\left[\begin{array}{ccc|c}1&1&1&0\\1&-1&0&0\\0&1&3&0\\-1&0&2&0\end{array}\right]
\rightarrow\left[\begin{array}{ccc|c}1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&0\end{array}\right]$$
Only the trivial solution exists, therefore Linearly Independent.

Def : Let $B$ and $C$ be two bases of a vector space $V$.
	There exists an $A_{n\times n}$ (linear transform) between them.

Theorem : Let $B$ and $C$ be two bases of a vector space $V$.
		Let $P_{C\leftarrow B}$ be the change of basis from $B$ to $C$.
1) $P_{C\leftarrow B}[x]_B = [x]_c$
2) $P_{C\leftarrow B}$ is unique.
3) $P_{C\leftarrow B}$ is invertible, and $\left(P_{C\leftarrow B}\right)^{-1}=P_{B\leftarrow C}$
4) The REF applied to $[C|B]$ produces $[I|P_{C\leftarrow B}]$


#### Pg. 471 #3
$$X=\begin{bmatrix}1\\0\\1\end{bmatrix},B=\mathbb{I}, C=\begin{bmatrix}1&0&0\\1&1&0\\1&1&1\end{bmatrix}$$
$$[C|B]=\left[\begin{array}{ccc|ccc}1&0&0&1&0&0\\1&1&0&0&1&0\\1&1&1&0&0&1\end{array}\right] \rightarrow\left[\begin{array}{ccc|ccc}1&0&0&1&0&0\\0&1&0&-1&1&0\\0&0&1&0&-1&1\end{array}\right]$$
$$P_{C\leftarrow B}X=\begin{bmatrix}1&0&0\\-1&1&0\\0&-1&1\end{bmatrix}\begin{bmatrix}1\\0\\1\end{bmatrix}_B=\begin{bmatrix}1\\-1\\1\end{bmatrix}_C$$
