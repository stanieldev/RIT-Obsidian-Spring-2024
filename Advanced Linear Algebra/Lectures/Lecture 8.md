DEF : $\lambda$ is an eigenvalue of a square matrix $A$ corresponding an eigenvector $\vec{\lambda}$ if $A\vec{\lambda}_\lambda = \lambda \cdot\vec{\lambda}_\lambda$.

### Pg. 310 #11
$$A= \begin{bmatrix}1&0&1\\0&1&1\\1&1&0\end{bmatrix} \rightarrow A-\lambda\mathbb{I} = \begin{bmatrix}1-\lambda&0&1\\0&1-\lambda&1\\1&1&-\lambda\end{bmatrix}$$
$$\left|\begin{array}1-\lambda&0&1\\0&1-\lambda&1\\1&1&-\lambda\end{array}\right| = -\lambda^3+2\lambda^2+\lambda-2 = 0$$
$$\begin{align}
(\lambda-1)(\lambda+1)(\lambda-2) = 0 \\
\lambda \in \{-1, 1, 2\}
\end{align}$$
$$\begin{align}
&\vec{\lambda}_{-1} = \dfrac{1}{\sqrt{6}}\begin{bmatrix}1\\1\\-2\end{bmatrix}
&\vec{\lambda}_{1} = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\-1\\0\end{bmatrix} \ \ \ \ \ \ \ \ \
&\vec{\lambda}_{2} = \dfrac{1}{\sqrt{3}}\begin{bmatrix}1\\1\\1\end{bmatrix}
\end{align}$$
### Pg. 299 #15
Suppose $A_{2\times2}$, given that:
$\lambda_1 = \dfrac{1}{2}$, $\vec{\lambda}_{1} = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\-1\end{bmatrix}$        $\lambda_2 = 2$, $\vec{\lambda}_{2} = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\1\end{bmatrix}$
$$\vec{x}= \begin{bmatrix}5\\1\end{bmatrix} = (2\sqrt{2})\cdot\vec{\lambda}_1+(3\sqrt{2})\cdot\vec{\lambda}_2$$
$$\begin{align}
A^{10}\vec{x} &= (2\sqrt{2})\cdot A^{10}\vec{\lambda}_1+(3\sqrt{2})\cdot A^{10}\vec{\lambda}_2\\
&= (2\sqrt{2})\left(\dfrac{1}{2}\right)^{10}\vec{\lambda}_1+(3\sqrt{2})\left(2\right)^{10}\vec{\lambda}_2 \\
&= \dfrac{2}{2^{10}}\begin{bmatrix}1\\-1\end{bmatrix}+(3)\left(2\right)^{10}\begin{bmatrix}1\\1\end{bmatrix}\\
&= \begin{bmatrix}\dfrac{1}{512}+3072\\-\dfrac{1}{512}+3072\end{bmatrix}
\end{align}$$

### Similarity and Diagonalization
Triangular and diagonal matrices are nice (their eigenvalues are transparently displayed).

DEF : Given $A_{n\times n}, B_{n\times n}$, we say that $A$ is similar to $B$, $A\sim B$, if there is an invertible matrix $P_{n\times n}$ such that:
$$P^{-1}A\ P = B \iff AP = PB$$
Where $P$ is a matrix who's columns are the eigenvectors of $A$.
