
**Diagonalization** : If $A_{n\times n}$ has $n$ eigenvectors, then $A$ can be written as $A=PDP^{-1}$.
 - $D$ is the diagonal matrices of eigenvalues.
 - $P$ is the matrix spanned by the eigenvectors.

**Spectral Theorem** : Matrix $A_{n\times n}$ is symmetric$\iff A=QDQ^{T}$   $\left(Q^T=Q^{-1}\right)$.
 - $D$ is the diagonal matrices of eigenvalues.
 - $Q$ is the orthogonal matrix spanned by the eigenvectors.

Now every matrix (symmetric or not, square or not), has a factorization $A=PDQ^T$
  - $D$ is diagonal.
  - $P, Q$ are orthogonal.


**Fact** : Given $A_{m\times n}$, $A^TA$ is an $n\times n$ symmetric matrix.
By spectral theorem, $A^TA$ can be orthogonally diagonalized.

**Def** : The singular values of $A_{m\times n}$ are the square roots of eigenvalues of $A^TA$, denoted by:
$$\sigma_1\ge\sigma_2\ge\dots\ge\sigma_n$$

### Pg. 609, #2
Find singular values of matrix $A=\begin{bmatrix}2&1\\1&2\end{bmatrix}$.
$$A^TA = \begin{bmatrix}2&1\\1&2\end{bmatrix}\begin{bmatrix}2&1\\1&2\end{bmatrix} = \begin{bmatrix}5&4\\4&5\end{bmatrix}$$
$$\lambda = \left\{1, 9\right\} \implies \sigma = \left\{1, 3\right\}$$

### Pg. 609, #10
Find singular values of matrix $A=\begin{bmatrix}1&0&1\\0&-3&0\\1&0&1\end{bmatrix}$.
$$A^TA = \begin{bmatrix}1&0&1\\0&-3&0\\1&0&1\end{bmatrix}\begin{bmatrix}1&0&1\\0&-3&0\\1&0&1\end{bmatrix} = \begin{bmatrix}2&0&2\\0&9&0\\2&0&2\end{bmatrix}$$
$$\lambda = \left\{0, 4,9\right\} \implies \sigma = \left\{0,2,3\right\}$$

### Singular Value Decomposition (SVD)
Let $A_{m\times n}$ have singular values $\sigma_1\ge\sigma_2\ge\dots\ge\sigma_r\gt0$ and $\sigma_{r+1}\ge\sigma_{r+2}\ge\dots\ge\sigma_n=0$.
Then there exists an orthogonal matrix $U_{m\times m}$ and orthogonal matrix $V_{n\times n}$, and an $m\times n$ matrix $\Sigma$ that contains the $\sigma$ in descending order, then:
$$A=U\Sigma V^T$$
Columns of $U$ are called left-singular vectors.
Columns of $V$ are called right-singular vectors.
The matrix $\Sigma$ is called the *Singular Value Decomposition*.

$V = [v_1\ v_2\ \dots v_n]$ consisting of orthonormal basis $S_v$ for $\mathbb{R}^n$ consisting of the eigenvectors of $A^TA$.
$U = [u_1\ u_2\ \dots u_n]$ where $u_i = \dfrac{1}{\sigma_i}Av_i$ for $i=1,2,3,\dots,r$.
$U$ must be extended to an orthonormal basis $u_1, u_2,\dots,u_n$ for $\mathbb{R}^n$.


### Pg. 609, #11
Find the SVD of matrix $A=\begin{bmatrix}1&1\\0&0\end{bmatrix}\implies A^T=\begin{bmatrix}1&0\\1&0\end{bmatrix}$.
$$A^TA=\begin{bmatrix}1&0\\1&0\end{bmatrix}\begin{bmatrix}1&1\\0&0\end{bmatrix} = \begin{bmatrix}1&1\\1&1\end{bmatrix}$$
$$\lambda = \left\{0, 2\right\} \implies \sigma = \left\{0, \sqrt2\right\}$$
$$\vec{\lambda_2}=\dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\1\end{bmatrix}, \vec{\lambda_0}=\dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\-1\end{bmatrix}$$
$$u_1=\dfrac{1}{\sqrt2}\begin{bmatrix}1&1\\0&0\end{bmatrix}\dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\1\end{bmatrix} = \begin{bmatrix}1\\0\end{bmatrix}$$
$$u_2=\begin{bmatrix}0\\1\end{bmatrix},\mathrm{to\ finish\ basis.}$$

