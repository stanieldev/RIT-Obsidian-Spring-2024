DEF: Given $A_{n\times n}, B_{n\times n}$, we say that $A$ is similar to $B$, $A\sim B$, if there is an invertible matrix $P_{n\times n}$ such that:
$$P^{-1}A\ P = B \iff AP = PB$$

DEF : $A_{n\times n}$ is *diagonalizable* if there is a diagonal matrix $D$ and invertible matrix $P_{n\times n}$, where:
$$P^{-1}A\ P = D \implies PDP^{-1} = A$$

Theorem: $A_{n\times n}$ is diagonalizable iif $A$ has $n$ linearly independent eigenvectors.
$$\left[\begin{array}{c|c|c|c}\vec{\lambda}_1&\vec{\lambda}_2&\dots&\vec{\lambda}_n\end{array}\right]^{-1}[A]\left[\begin{array}{c|c|c|c}\vec{\lambda}_1&\vec{\lambda}_2&\dots&\vec{\lambda}_n\end{array}\right] = \left[\begin{array}{cccc}\lambda_1&0&\dots&0&\\0&\vec{\lambda}_2&\dots&0\\\dots&\dots&\dots&0\\0&0&0&\vec{\lambda}_n\end{array}\right]$$
Facts:
1) If $\lambda_1, \lambda_1,\dots,\lambda_n,$ are distinction eigenvalues of $A_{n\times n}$ and B is a basis for eigenspace , then B is linearly independent.
2) If $\lambda_1, \lambda_1,\dots,\lambda_n,$ are distinction eigenvalues of $A_{n\times n}$, then $A$ is diagonalizable.
3) The geometric multiplicity of $\lambda$ of $A$ is less than or equal to the algebraic multiplicity.

### Diagonalization Theorem
$$A_{n\times n} \mathrm{\ is\ diagonalizable} \ \ \iff \ \ |\mathrm{Basis}|=n \ \ \iff \ \ \mathrm{Alg\ Mult. = Geo\ Mult.}$$


### Pg. 310 #11
$$\begin{bmatrix}1&0&1\\0&1&1\\1&1&0\end{bmatrix} \rightarrow \lambda = \left\{-1, 1, 2\right\} \ \& \ B_\lambda=\left\{\dfrac{1}{\sqrt{6}}\begin{bmatrix}1\\1\\-2\end{bmatrix}, \dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\-1\\0\end{bmatrix}, \dfrac{1}{\sqrt{3}}\begin{bmatrix}1\\1\\1\end{bmatrix}\right\}$$
$$P=\begin{bmatrix}-1&-1&1\\-1&1&1\\2&0&1\end{bmatrix}, \ \ \ P^{-1}=\dfrac{1}{6}\begin{bmatrix}-1&-1&2\\-3&3&0\\2&2&2\end{bmatrix}, \ \ \ D=\begin{bmatrix}-1&0&0\\0&1&0\\0&0&2\end{bmatrix}$$

### Magic of Diagonalization
Suppose $P^{-1} A\ P = D \iff P\ D\ P^{-1} = A$.
$$\begin{align}A^k &= \left(PDP^{-1}\right)^k \\
&= PDP^{-1}PDP^{-1}\dots PDP^{-1} \\
&= PD^kP^{-1} \\
\Aboxed{A^k &=P D^k P^{-1}}
\end{align}$$


Random Question #17
$$\begin{bmatrix}-1&6\\1&0\end{bmatrix} \rightarrow \lambda=\left\{-3, 2\right\} \ \&\ B=\left\{\dfrac{1}{\sqrt{10}}\begin{bmatrix}3\\-1\end{bmatrix}, \dfrac{1}{\sqrt{5}}\begin{bmatrix}2\\1\end{bmatrix}\right\} $$
$$\dfrac{1}{5}\begin{bmatrix}-3&2\\1&1\end{bmatrix}\begin{bmatrix}-3&0\\0&2\end{bmatrix}\begin{bmatrix}-1&2\\1&3\end{bmatrix} = \begin{bmatrix}-1&6\\1&0\end{bmatrix}$$
$$\begin{bmatrix}-1&6\\1&0\end{bmatrix}^10 = \dfrac{1}{5}\begin{bmatrix}-3&2\\1&1\end{bmatrix}\begin{bmatrix}3^{10}&0\\0&2^{10}\end{bmatrix}\begin{bmatrix}-1&2\\1&3\end{bmatrix}$$
$$A^{10} = \begin{bmatrix}35839&-69630\\-11605&24234\end{bmatrix}$$

Random Question #21
$$\begin{bmatrix}1&1&1\\0&-1&0\\0&0&-1\end{bmatrix} \rightarrow \lambda=\left\{-1,1\right\} \ \&\ B=\left\{
\begin{bmatrix}1\\0\\0\end{bmatrix}, 
\dfrac{1}{\sqrt{5}}\begin{bmatrix}-1\\2\\0\end{bmatrix}, 
\dfrac{1}{\sqrt{5}}\begin{bmatrix}-1\\0\\2\end{bmatrix}
\right\}$$
$$\begin{bmatrix}1&-1&-1\\0&2&0\\0&0&2\end{bmatrix}\begin{bmatrix}-1&0&0\\0&-1&0\\0&0&1\end{bmatrix}\begin{bmatrix}1&-1&-1\\0&2&0\\0&0&2\end{bmatrix}^{-1} = \begin{bmatrix}1&1&1\\0&-1&0\\0&0&-1\end{bmatrix}$$
$$\begin{align}
\begin{bmatrix}1&1&1\\0&-1&0\\0&0&-1\end{bmatrix}^{2015} &= \begin{bmatrix}1&-1&-1\\0&2&0\\0&0&2\end{bmatrix}\begin{bmatrix}-1&0&0\\0&-1&0\\0&0&1\end{bmatrix}^{2015}\begin{bmatrix}1&-1&-1\\0&2&0\\0&0&2\end{bmatrix}^{-1} \\
&= \begin{bmatrix}1&-1&-1\\0&2&0\\0&0&2\end{bmatrix}\begin{bmatrix}(-1)^{2015}&0&0\\0&(-1)^{2015}&0\\0&0&1^{2015}\end{bmatrix}\begin{bmatrix}1&-1&-1\\0&2&0\\0&0&2\end{bmatrix}^{-1} \\
\begin{bmatrix}1&1&1\\0&-1&0\\0&0&-1\end{bmatrix}^{2015} &= \begin{bmatrix}1&1&1\\0&-1&0\\0&0&-1\end{bmatrix}
\end{align}$$