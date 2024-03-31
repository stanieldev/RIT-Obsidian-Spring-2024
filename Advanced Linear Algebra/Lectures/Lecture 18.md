Def : A transform $T: \mathbb{R}^n \rightarrow \mathbb{R}^m$ is a linear transform if:
1) $T(u+v) = T(u) + T(v)$ for all $u,v \in \mathbb{R}^n$.
2) $T(cu) = cT(u)$ for all $u \in \mathbb{R}^n, c \in \mathbb{R}$.

Show that $T: \mathbb{R}^3 \rightarrow \mathbb{R}^2$ by $T\begin{bmatrix}x\\y\\z\end{bmatrix}=\begin{bmatrix}x-y+z\\2x+y-3z\end{bmatrix}$.
Let $u=\begin{bmatrix}x_1\\y_1\\z_1\end{bmatrix}$ and $v=\begin{bmatrix}x_2\\y_2\\z_2\end{bmatrix}$, which means $u+v = \begin{bmatrix}x_1+x_2\\y_1+y_2\\z_1+z_2\end{bmatrix}$
$$\begin{align}
T(u+v)&=T\begin{bmatrix}x_1+x_2\\y_1+y_2\\z_1+z_2\end{bmatrix}\\
&= \begin{bmatrix}(x_1+x_2)-(y_1+y_2)+(z_1+z_2)\\2(x_1+x_2)+(y_1+y_2)-3(z_1+z_2)\end{bmatrix}\\
&= \begin{bmatrix}x_1+x_2-y_1-y_2+z_1+z_2\\2x_1+2x_2+y_1+y_2-3z_1-3z_2\end{bmatrix}\\
&= \begin{bmatrix}x_1-y_1+z_1\\2x_1+y_1-3z_1\end{bmatrix}+\begin{bmatrix}x_2-y_2+z_2\\2x_2+y_2-3z_2\end{bmatrix}\\
\Aboxed{T(u+v)&=T(u)+T(v)}
\end{align}$$
$$\begin{align}
T(cu)&= T\begin{bmatrix}cx_1\\cy_1\\cz_1\end{bmatrix}\\
&= \begin{bmatrix}cx_1-cy_1+cz_1\\2cx_1+cy_1-3cz_1\end{bmatrix}\\
&= c\begin{bmatrix}x_1-y_1+z_1\\2x_1+y_1-3z_1\end{bmatrix}\\\
\Aboxed{T(cu)&=cT(u)}
\end{align}$$
Therefore, this transformation is a *linear transform*.
Note: It is possible to both parts at the same time. Use that for homework.


Theorem : Given $A_{m\times n}$ and $X\in \mathbb{R}^n$, the matrix transformation $T_A: \mathbb{R}^n\rightarrow \mathbb{R}^m$ defined by $T_A(X)=AX$ is a linear transform. I.e. All linear transforms can be written as a matrix.

