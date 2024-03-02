**Date: 2/27/2024**

Homework:
5.1: 2-18 (Even)
5.2: 2-14 (Even)




Ex: $\vec{u}_1=\begin{bmatrix}0\\0\\1\end{bmatrix}, \vec{u}_2=\begin{bmatrix}1\\0\\0\end{bmatrix}, \vec{u}_3=\begin{bmatrix}0\\1\\0\end{bmatrix}$.

Theorem: The columns of $Q_{m\times n}$ form an orthonormal basis iff $Q^TQ = \mathbb{I}$.

Def: An $n\times n$ matrix $Q$ whose columns form an orthonormal set is called a *orthonormal matrix.*
This is identical to saying that $Q^T = Q^{-1}$.

Theorem: A square matrix is orthogonal iff $Q^{-1}=Q^T$.


Example: $A=\begin{bmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{bmatrix}$.
$A^{-1} = \dfrac{1}{\cos^2\theta+\sin^2\theta}\begin{bmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{bmatrix} = A^T$
This matrix is orthogonal.


Theorem: If $Q$ is an $n\times n$ matrix, then the following are equivalent.
i) $Q$ is orthogonal.
ii) $|Q\vec{x}| = |\vec{x}|$ for all $x\in\mathbb{R}^n$ (length preserving).
iii) $Q\vec{x}\cdot Q\vec{y}=\vec{x}\cdot\vec{y}$ for every $x, y\in\mathbb{R}^n$.

Theorem: If $Q$ is an orthogonal matrix, then its rows form an orthonormal set.
Proof: Remember that orthogonal means that $Q^{-1}=Q^T$.
$\left(Q^{T}\right)^{-1}=\left(Q^{-1}\right)^{-1} = Q$.
So if $Q^T$ is orthogonal, and this means that Q forms an orthonormal set.

Theorem: Let $Q$ be an orthogonal matrix, then:
i) $Q^{-1}$ is orthogonal.
ii) $\det Q = \pm1$
iii) $|\lambda|=1$ for all eigenvalues $\lambda$ of $Q$.
iv) If $Q_1, Q_2$ are $n\times n$ orthogonal matrices, then so is $Q_1Q_2$.


## Sec 5.2: Orthogonal Complements
Def : Let $W$ be a subspace of $\mathbb{R}^n$.
We say that a vector $\vec{V}\in\mathbb{R}^n$ is orthogonal to $W$ if $\vec{V}$ is orthogonal to every vector in $W$.

Def : The set of all vectors orthogonal to $W$, $W^\perp$, is called the orthogonal complement of $W$.

Theorem: Let $W$ be a subspace of $\mathbb{R}^n$, then
i) $W^\perp$ is a subspace of $\mathbb{R}^n$.
ii) $\left(W^\perp\right)^\perp = W$
iii) $W\cap W^\perp = \left\{\vec{0}\right\}$
iv) If $W=\mathrm{span}\left\{ \vec{w}_1,\vec{w}_2,\dots,\vec{w}_k \right\}$, then $\vec{V}\in W^\perp$ **iff** $\vec{V}\cdot w_i = 0 \ \forall i\in\mathbb{Z}$


### The 4 Fundamental Subspaces
Theorem: Let $A$ be an $m\times n$ matrix, then:
$\left[\mathrm{row}(A)\right]^\perp = \mathrm{null}(A)$ and $\left[\mathrm{col}(A)\right]^\perp = \mathrm{null}\left(A^T\right)$



### Pg. 387 #1
$$W=\left\{\begin{bmatrix}x\\y\end{bmatrix}: 2x-y=0\right\}$$
$W$ is a column space of $A=\begin{bmatrix}1\\2\end{bmatrix}$, so $W^\perp=\mathrm{null}\left(A^T\right)=\begin{bmatrix}2&-1&|&0\end{bmatrix}$.
$$W^\perp=\left\{\begin{bmatrix}x\\y\end{bmatrix}: x+2y=0\right\}$$


### Pg. 387 #3
$$W=\left\{\begin{bmatrix}x\\y\\z\end{bmatrix}: x+y-z=0\right\}=\left\{\begin{bmatrix}x\\y\\x+y\end{bmatrix}\right\}=\mathrm{span}\left\{\begin{bmatrix}1\\0\\1\end{bmatrix},\begin{bmatrix}0\\1\\1\end{bmatrix}\right\}$$
$W$ is a column space of $A=\begin{bmatrix}1&0\\0&1\\1&1\end{bmatrix}$, so $W^\perp=\mathrm{null}\left(A^T\right)$
$$\implies W^\perp=\mathrm{span}\left\{\begin{bmatrix}1\\1\\-1\end{bmatrix}\right\}$$


