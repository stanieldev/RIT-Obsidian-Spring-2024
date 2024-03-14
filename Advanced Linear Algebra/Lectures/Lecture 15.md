Sec. 5.4: Orthogonal Diagonalization of Symmetric Matrices
Reminder: $A_{n\times n}$ is diagonalizable iff there is a diagonal matrix $D$ such that $A\sim D$.
		That is, there exists an invertible matrix $P$ where $P^{-1}AP=D$.

### Pg. 407 #1
Given matrix $A=\begin{bmatrix}4&1\\1&4\end{bmatrix}$, orthogonally diagonalize $A$.
$\det A = (4-\lambda)^2-1 = \lambda^2-8\lambda+15 = (\lambda-5)(\lambda-3) \implies \lambda = 3,5$.
$$\begin{align}
&\vec{\lambda}_3=\begin{bmatrix}1\\-1\end{bmatrix} &\vec{\lambda}_5=\begin{bmatrix}1\\1\end{bmatrix}
\end{align}$$
This time, let's use G-S process to orthonormalize.
$$\begin{align}
&\vec{v}_1=\dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\-1\end{bmatrix}
&\vec{v}_2=\dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\1\end{bmatrix}
& \ \ \ \ \ \ \ Q=\dfrac{1}{\sqrt{2}}\begin{bmatrix}1&1\\-1&1\end{bmatrix}
\end{align}$$
$Q$ makes it really easy, so we can do:
$$Q^{-1} = Q^T =\dfrac{1}{\sqrt{2}}\begin{bmatrix}1&-1\\1&1\end{bmatrix}$$
Meaning the diagonalizable metric can be written as:
$$Q^T A \ Q = D$$

Def : $A_{n\times n}$ is orthogonally diagonalizable if thee is an orthogonal matrix $Q$ and a diagonal matrix $D$ such that $Q^T A \ Q = D$.

Theorem: If $A$ is orthogonal diagonalizable, then $A$ is symmetric.
Proof: If $A$ is O.D., then there are $Q$ and $D$ such that $Q^T A \ Q = D$
	Also $Q$ is orthogonal, then $Q^T = Q^{-1}$ or $QQ^T=I$.
	$QD\ Q^T = Q(Q^TA\ Q)Q^T = QQ^TAQQ^T = IAI = A$.
	$A^T = (QDQ^T)^T = QD^TQ^T = QDQ^T = A$
	Therefore $A$ is symmetric.

Theorem: If $A$ is a real symmetric matrix, then the eigenvalues of $A$ are all real.

Theorem: If $A$ is symmetric, then the eigenvectors corresponding to distinct eigenvalues of $A$ are orthogonal.

### Spectral Theorem
$A_{n\times n}$ is Symmetric$\iff$$A_{n \times n}$ is Orthogonal Diagonalizable.



### Pg. 407 #5
Given matrix $A=\begin{bmatrix}5&0&0\\0&1&3\\0&3&1\end{bmatrix}$, orthogonally diagonalize $A$.
$\lambda \in \left\{5,4,-2\right\}$, $\vec{\lambda}\in\left\{\begin{bmatrix}1\\0\\0\end{bmatrix}, \dfrac{1}{\sqrt2}\begin{bmatrix}0\\1\\1\end{bmatrix},\dfrac{1}{\sqrt2}\begin{bmatrix}0\\1\\-1\end{bmatrix}\right\}$, $Q=\begin{bmatrix}1&0&0\\0&1/\sqrt2&1/\sqrt2\\0&1/\sqrt2&-1/\sqrt2\end{bmatrix}$, $D=\begin{bmatrix}5&0&0\\0&4&0\\0&0&-2\end{bmatrix}$.
$$Q^T A\ Q = D$$

### Spectral Decomposition
If $A$ is symmetric and $Q^T A\ Q = D$, then $A = Q\ D\ Q^T$.
Where $D$ is the diagonal of eigenvalues, and $Q$ is the orthogonal columns of the eigenvectors.
Observe: $Q\ D\ Q^T = \sum_i \lambda_i q_i q_i^T$


### Pg. 407 #17

Given matrix $A=\begin{bmatrix}4&1\\1&4\end{bmatrix}$
$$\dfrac{1}{2}\begin{bmatrix}1&-1\\1&1\end{bmatrix} \begin{bmatrix}4&1\\1&4\end{bmatrix} \begin{bmatrix}1&1\\-1&1\end{bmatrix} = \begin{bmatrix}3&0\\0&5\end{bmatrix}$$
To do spectral decomposition, we write it as the following:
$$\begin{align}
A&=3\begin{bmatrix}1/2&-1/2\\-1/2&1/2\end{bmatrix}+5\begin{bmatrix}1/2&1/2\\1/2&1/2\end{bmatrix} \\
&=3\cdot\dfrac{1}{2}\begin{bmatrix}1&-1\\-1&1\end{bmatrix}+5\cdot\dfrac{1}{2}\begin{bmatrix}1&1\\1&1\end{bmatrix}
\end{align}$$

### Pg. 407 #19
Given matrix $A=\begin{bmatrix}5&0&0\\0&1&3\\0&3&1\end{bmatrix}$.
$\lambda \in \left\{5,4,-2\right\}$, $\vec{\lambda}\in\left\{\begin{bmatrix}1\\0\\0\end{bmatrix}, \dfrac{1}{\sqrt2}\begin{bmatrix}0\\1\\1\end{bmatrix},\dfrac{1}{\sqrt2}\begin{bmatrix}0\\1\\-1\end{bmatrix}\right\}$, $Q=\begin{bmatrix}1&0&0\\0&1/\sqrt2&1/\sqrt2\\0&1/\sqrt2&-1/\sqrt2\end{bmatrix}$, $D=\begin{bmatrix}5&0&0\\0&4&0\\0&0&-2\end{bmatrix}$.
$$Q^T A\ Q = D$$
To do spectral decomposition, we write it as the following:
$$\begin{align}
A&=5\begin{bmatrix}1&0&0\\0&0&0\\0&0&0\end{bmatrix}
+4\begin{bmatrix}0&0&0\\0&1/2&1/2\\0&1/2&1/2\end{bmatrix}
-2\begin{bmatrix}0&0&0\\0&1/2&-1/2\\0&-1/2&1/2\end{bmatrix}
\end{align}$$
