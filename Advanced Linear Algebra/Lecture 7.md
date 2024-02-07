### Eigenvalues and Eigenvectors
German for "own" as in "your own". They are special values and vectors of square matrices.

DEF : Let $A$ be an $n\times n$ matrix and scalar $\lambda$ is called an *eigenvalue* of $A$ if there is a non-zero vector $\vec{x}$ such that:
$$A\vec{x}=\lambda\vec{x}$$
Where $\vec{x}$ is called an *eigenvector* of $A$ with an eigenvalue $\lambda$ (scale factor).

#### Example
Show that $\vec{x}=\begin{bmatrix}5\\5\end{bmatrix}$ is an eigenvector of $A=\begin{bmatrix}3&1\\1&3\end{bmatrix}$.
$$A\vec{x}=\begin{bmatrix}3&1\\1&3\end{bmatrix}\begin{bmatrix}5\\5\end{bmatrix} = \begin{bmatrix}20\\20\end{bmatrix} = 4\begin{bmatrix}5\\5\end{bmatrix}$$
Note: The set of eigenvectors corresponding to an eigenvalue $\lambda$ of $A_{n\times n}$ is the set of non-zero vectors in the $\mathrm{null}(A-\lambda\mathbb{I})$.

### Example Pg. 261 #11
$$A=\begin{bmatrix}1&0&2\\-1&1&1\\2&0&1\end{bmatrix}, \ \ \ \lambda = -1$$
$$A-\lambda\mathbb{I}=\begin{bmatrix}2&0&2\\-1&2&1\\2&0&2\end{bmatrix} \rightarrow \begin{bmatrix}1&0&1\\0&1&1\\0&0&0\end{bmatrix}$$
Letting $\vec{x} = \begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix}$, then $\vec{\lambda}_{-1}=\dfrac{1}{\sqrt{3}}\begin{bmatrix}-1\\-1\\1\end{bmatrix}$.

DEF : $\lambda$ is an eigenvalue of $A$ if $A-\lambda\mathbb{I}$ is non-invertible or that $\det(A-\lambda\mathbb{I})=0$.

DEF : Eigenvalues of a square matrix are precisely the solutions $\lambda$ of the equation.
The polynomial in $\lambda$ of $\det(A-\lambda\mathbb{I})=0$ is the *characteristic polynomial*.


Algorithms:
Given a square matrix:
1) Compute the characteristic polynomial of $A-\lambda\mathbb{I}$.
2) Solve for the values $\lambda$ that satisfy $\det(A-\lambda\mathbb{I})=0$.
3) Find vectors $\vec{x}$ that satisfy $(A-\lambda\mathbb{I})\vec{x} = 0$.

### Pg. 298 #1
$$A = \begin{bmatrix}1&3\\-2&6\end{bmatrix} \implies A-\lambda\mathbb{I} = \begin{bmatrix}1-\lambda&3\\-2&6-\lambda\end{bmatrix}$$
$$\det(A-\lambda\mathbb{I}) = (1-\lambda)(6-\lambda) - (3)(-2) = \boxed{\lambda^2-7\lambda+12 = 0}$$
$$\lambda = 3 \mathrm{\ or\ } \lambda = 4$$
If $\lambda = 3$:
$$\begin{align}
\vec{\lambda}_{3}&: A-\lambda\mathbb{I} = \begin{bmatrix}-2&3\\-2&3\end{bmatrix}\begin{bmatrix}x_1\\x_2\end{bmatrix} = \begin{bmatrix}0\\0\end{bmatrix}\\
\implies& \boxed{\vec{\lambda}_{3}=\dfrac{1}{\sqrt{13}}\begin{bmatrix}3\\2\end{bmatrix}}
\end{align}$$
If $\lambda = 4$:
$$\begin{align}
\vec{\lambda}_{4}&: A-\lambda\mathbb{I} = \begin{bmatrix}-3&3\\-2&2\end{bmatrix}\begin{bmatrix}x_1\\x_2\end{bmatrix} = \begin{bmatrix}0\\0\end{bmatrix}\\
\implies& \boxed{\vec{\lambda}_{4}=\dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\1\end{bmatrix}}
\end{align}$$



DEF : The algebraic multiplicity of an eigenvalue $\lambda$ is the multiplicity of the root $\lambda$ of the characteristic polynomial. This depends on the degree of the polynomial factors.

DEF : The geometric multiplicity of an eigenvalue $\lambda$ is the number of vectors in the dimension of the eigenspace $E_\lambda$.

Facts:
1) Eigenvalues of a triangular matrix are the entries of the diagonal.
2) A square matrix invertible iff $\lambda = 0$ is not an eigenvalue of $A$.


### Pg. 298 #5
$$A = \begin{bmatrix}1&2&0\\-1&-1&1\\0&1&1\end{bmatrix} \rightarrow R = \begin{bmatrix}1&2&0\\0&1&1\\0&0&0\end{bmatrix}$$
$$\det(A-\lambda\mathbb{I}) = -\lambda^2(\lambda-1)$$
If $\lambda = 0$:
$$\begin{bmatrix}1&2&0\\-1&-1&1\\0&1&1\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix} = \begin{bmatrix}0\\0\\0\end{bmatrix} \implies \boxed{\vec{\lambda}_{0} = \dfrac{1}{\sqrt{6}}\begin{bmatrix}2\\-1\\1\end{bmatrix}}$$
If $\lambda = 1$:
$$\begin{bmatrix}0&2&0\\-1&-2&1\\0&1&0\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix} = \begin{bmatrix}0\\0\\0\end{bmatrix} \implies \boxed{\vec{\lambda}_{1} = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\0\\1\end{bmatrix}}$$


### Pg. 298 #11
$$A = \begin{bmatrix}1&0&0&0\\0&1&0&0\\1&1&3&0\\-2&1&2&-1\end{bmatrix} \rightarrow R = \begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&3&0\\0&0&0&-1\end{bmatrix}$$
$$\det(A-\lambda\mathbb{I}) = (\lambda-1)^2(\lambda-3)(\lambda+1)$$
If $\lambda = 1$:
$$\begin{bmatrix}0&0&0&0\\0&0&0&0\\1&1&2&0\\-2&1&2&-2\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\\x_4\end{bmatrix} = \begin{bmatrix}0\\0\\0\\0\end{bmatrix} \implies \boxed{\vec{\lambda}_{1} = \dfrac{1}{\sqrt{17}}\begin{bmatrix}2\\-2\\0\\3\end{bmatrix}, \dfrac{1}{\sqrt{14}}\begin{bmatrix}-2\\0\\1\\3\end{bmatrix}}$$ 
If $\lambda = 3$:
$$\begin{bmatrix}-2&0&0&0\\0&-2&0&0\\1&1&0&0\\-2&1&2&-4\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\\x_4\end{bmatrix} = \begin{bmatrix}0\\0\\0\\0\end{bmatrix} \implies \boxed{\vec{\lambda}_{3} = \dfrac{1}{\sqrt{5}}\begin{bmatrix}0\\0\\2\\1\end{bmatrix}}$$
If $\lambda = -1$:
$$\begin{bmatrix}2&0&0&0\\0&2&0&0\\1&1&4&0\\-2&1&2&0\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\\x_4\end{bmatrix} = \begin{bmatrix}0\\0\\0\\0\end{bmatrix} \implies \boxed{\vec{\lambda}_{-1} = \dfrac{1}{\sqrt{}}\begin{bmatrix}0\\0\\0\\1\end{bmatrix}}$$
| $\lambda$ | Alg. | $E_\lambda$ | Geo. |
| --- |
| $1$ | $2$ | $\mathrm{span}()$ | $2$ | 
| $1$ | $1$ | $\mathrm{span}()$ | $1$ | 
| $1$ | $1$ | $\mathrm{span}()$ | $1$ | 



Fundamental Theorem of Invertible Matrices:
14) $\det(A) \ne 0$.
15) Zero is not an eigenvalue of $A$.

Theorem: Let $A$ be a square matrix have eigenvalue $\lambda$ and corresponding eigenvector $\vec{\lambda}_\lambda$.
i) For any positive integer $n$, $\lambda^n$ is an eigenvalue of $A^n$ corresponding to eigenvector $\vec{\lambda}_\lambda$.
ii) If $A$ is invertible, then $\dfrac{1}{\lambda}$ is an eigenvalue of $A^{-1}$ corresponding to eigenvector $\vec{\lambda}_\lambda$.
Exponentiation of a matrix $A$ changes the eigenvalues, but not the eigenvectors.





