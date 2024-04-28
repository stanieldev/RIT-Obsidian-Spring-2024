**Date: 4/23/2024**

**Diagonalization Theorem**
$A_{n\times n}$ is diagonalizable iff $A$ has $n$ linearly-independent eigenvectors.
$$A=PDP^{-1}$$
Where $D$ is the diagonal matrix of eigenvalues and $P$ are columns spanned by the eigenvectors.

**Spectral Theorem**
$A_{n\times n}$ is symmetric iff $A$ is orthogonally diagonalizable.
$$A=QDQ^T$$

**Spectral Decomposition**
$A = \lambda_1q_1q_1^T+\lambda_2q_2q_2^T+\dots+\lambda_nq_nq_n^T$

**Singular Value Decomposition**
Let $A_{m\times n}$ have singular values $\sigma_1\ge\sigma_2\ge\dots\ge\sigma_r\gt0$ and $\sigma_{r+1}=\sigma_{r+2}=\dots=\sigma_n=0$.
$$A=U_{m\times m}\Sigma_{m\times n}V_{n\times n}^T$$
Where $U, V$ are both orthogonal.
$V$ columns are spanned of eigenvectors of $A^TA$.
$U$ columns are $u_i=\dfrac{1}{\sigma_i}Av_i$, where $\sigma_i=\sqrt{\lambda_i}$ of the $A^TA$ matrix.


### Outer Product form of SVD
Let $A_{m\times n}$ have singular values $\sigma_1\ge\sigma_2\ge\dots\ge\sigma_r\gt0$ and $\sigma_{r+1}=\sigma_{r+2}=\dots=\sigma_n=0$.
$$A=\sum_i\sigma_iu_iv_i^T=\sum_{i=0}^r\sqrt{\lambda_i}u_iv_i^T$$
Theorem : If $A=U\Sigma V^T$ is a singular value decomposition of matrix $A_{m\times n}$, then:
1) $\mathrm{rank}(A)=r$.
2) Columns of $U$ from $0$ to $r$ is an orthonormal basis for $\mathrm{col}(A)$.
3) Columns of $U$ from $r+1$ to $n$ is an orthonormal basis for $\mathrm{null}(A^T)$.
4) Columns of $V$ from $0$ to $r$ is an orthonormal basis for $\mathrm{row}(A)$.
5) Columns of $V$ from $r+1$ to $n$ is an orthonormal basis for $\mathrm{null}(A)$.



### Fundamental Theorem of Invertible Matrices
 - $A$ is invertible





### Pg. 609 #6
$A=\begin{bmatrix}3\\4\end{bmatrix}$, $A^T=\begin{bmatrix}3&4\end{bmatrix}$
$A^TA= \begin{bmatrix}3&4\end{bmatrix}\begin{bmatrix}3\\4\end{bmatrix} = \begin{bmatrix}9&12\\12&16\end{bmatrix}$
$\lambda=\left\{0, 25\right\} \implies \sigma=\left\{0, 5\right\}$


### Pg. 609 #7
$A=\begin{bmatrix}0&0\\0&3\\-2&0\end{bmatrix}$, $A^T=\begin{bmatrix}0&0&-2\\0&3&0\end{bmatrix}$
$A^TA=\begin{bmatrix}0&0&-2\\0&3&0\end{bmatrix}\begin{bmatrix}0&0\\0&3\\-2&0\end{bmatrix} = \begin{bmatrix}4&0\\0&9\end{bmatrix}$
$\lambda=\left\{4, 9\right\} \implies \sigma=\left\{2, 3\right\}$



### Pg. 609 #17
Same as #7 for beginning.
$\vec{\lambda}=\left\{\begin{bmatrix}0\\1\end{bmatrix},\begin{bmatrix}1\\0\end{bmatrix}\right\} \implies V=\begin{bmatrix}0&1\\1&0\end{bmatrix}$
The order of $V$ is because 3 comes before 2 for our $\sigma$ values.
$$u_1=\dfrac{1}{\sigma_1}Av_1=\begin{bmatrix}0\\1\\0\end{bmatrix}\rightarrow\begin{bmatrix}0\\1\\0\end{bmatrix}$$
$$u_2=\dfrac{1}{\sigma_2}Av_2=\begin{bmatrix}0\\0\\-1\end{bmatrix}\rightarrow\begin{bmatrix}0\\0\\-1\end{bmatrix}$$
$$u_3=\begin{bmatrix}1\\0\\0\end{bmatrix}\mathrm{\ by\ assignment.}$$
$$U=\begin{bmatrix}0&0&1\\1&0&0\\0&-1&0\end{bmatrix},\Sigma=\begin{bmatrix}3&0\\0&2\\0&0\end{bmatrix}, V=\begin{bmatrix}0&1\\1&0\end{bmatrix}$$
Therefore we can say that:
$$A=U\Sigma V^T = U=\begin{bmatrix}0&0&1\\1&0&0\\0&-1&0\end{bmatrix}\begin{bmatrix}3&0\\0&2\\0&0\end{bmatrix}\begin{bmatrix}0&1\\1&0\end{bmatrix}$$


### Pg. 609 #23
Start from #17
$$A=\sum_i\sigma_iu_iv_i^T$$
$$A=3\begin{bmatrix}0&0\\1&0\\0&0\end{bmatrix} + 2\begin{bmatrix}0&0\\0&0\\-1&0\end{bmatrix}$$
You can leave in column-vector times row-vector form on the homework.




