

### Vector Projection
$$\begin{align}
\vec{v}&=\mathrm{proj}_\vec{u}(\vec{v}) + \mathrm{perp}_\vec{u}(\vec{v})\\
\mathrm{proj}_\vec{u}(\vec{v})&=\left(\vec{v}\cdot\hat{u}\right)\hat{u} = \left(\dfrac{\vec{v}\cdot\vec{u}}{||\vec{u}||^2}\right)\vec{u}\\
\mathrm{perp}_\vec{u}(\vec{v})&=\vec{v}-\mathrm{proj}_\vec{u}(\vec{v})
\end{align}$$

DEF: Let $W$ be a subspace of $\mathbb{R}^n$ and let $\left\{\vec{u}_1, \vec{u}_2,\dots, \vec{u}_k\right\}$ be an orthogonal basis of $W$.
For any $\vec{v}$ in $\mathbb{R}^n$, the orthogonal projection of $\vec{v}$ on $W$ is:
$$\begin{align}
\mathrm{proj}_W(\vec{v})&=\mathrm{proj}_{\vec{u}_1}(\vec{v})+\mathrm{proj}_{\vec{u}_2}(\vec{v})+\dots+\mathrm{proj}_{\vec{u}_k}(\vec{v})\\
&= \left(\vec{v}\cdot\hat{u_1}\right)\hat{u_1}+\left(\vec{v}\cdot\hat{u_2}\right)\hat{u_2}+\dots+\left(\vec{v}\cdot\hat{u_k}\right)\hat{u_k}\\
&= \left(\dfrac{\vec{v}\cdot\vec{u_1}}{||\vec{u_1}||^2}\right)\vec{u_1} + \left(\dfrac{\vec{v}\cdot\vec{u_2}}{||\vec{u_2}||^2}\right)\vec{u_2} + \dots + \left(\dfrac{\vec{v}\cdot\vec{u_k}}{||\vec{u_k}||^2}\right)\vec{u_k}\\\
\Aboxed{\mathrm{proj}_W(\vec{v})&=\sum_i^k \left(\dfrac{\vec{v}\cdot\vec{u_i}}{||\vec{u_i}||^2}\right)\vec{u_i}}
\end{align}$$
To find the perpendicular vector, we follow a similar process:
$$\begin{align}
\vec{v}&=\mathrm{proj}_\vec{W}(\vec{v}) + \mathrm{perp}_\vec{W}(\vec{v})\\
\mathrm{proj}_\vec{W}(\vec{v})&=\sum_i^k \left(\dfrac{\vec{v}\cdot\vec{u_i}}{||\vec{u_i}||^2}\right)\vec{u_i}\\
\mathrm{perp}_\vec{W}(\vec{v})&=\vec{v}-\mathrm{proj}_\vec{W}(\vec{v})\\
\Aboxed{\mathrm{perp}_\vec{W}(\vec{v}) &= \vec{v}-\sum_i^k \left(\dfrac{\vec{v}\cdot\vec{u_i}}{||\vec{u_i}||^2}\right)\vec{u_i}}
\end{align}$$

### Orthogonal Decomposition Theorem
Let $W$ be a subspace of $\mathbb{R}^n$ and let $\vec{v}$ be a vector in $\mathbb{R}^n$.
Then there are unique vectors $\vec{w}\in W$ and $\vec{w}^\perp\in W^\perp$ such that $\vec{v} = \vec{w}+\vec{w}^\perp$.

Theorem: If $W$ is a subspace of $\mathbb{R}^n$, then  $\mathrm{dim}\ W+\mathrm{dim}\ W^\perp = n$.

Proof: Choose orthogonal basis $\left\{\vec{u}_1, \vec{u}_2,\dots, \vec{u}_k\right\}$ for $W$  ($\mathrm{dim}\ W=k$).
      Choose orthogonal basis $\left\{\vec{v}_1, \vec{v}_2,\dots, \vec{v}_l\right\}$ for $W^\perp$  ($\mathrm{dim}\ W\perp=l$).

Claim that $\beta = \left\{\vec{u}_1, \vec{u}_2,\dots, \vec{u}_k, \vec{v}_1, \vec{v}_2,\dots, \vec{v}_l\right\}$ is an orthogonal basis for $\mathbb{R}^n$.
	Note: $u_i\cdot u_j = U_i\delta_{ij}$ , $v_i\cdot v_j = V_i\delta_{ij}$ , $u_i\cdot v_j = K_i\delta_{ij}$.
	Therefore, all vectors in the basis are linearly independent.

If $\vec{v}$ is a vector in $\mathbb{R}^n$, by the orthogonal decomposition theorem, $\vec{v} = \vec{w}+\vec{w}^\perp$.
	But $\vec{w}$ can be written as a linear combination of $\left\{\vec{u}_1, \vec{u}_2,\dots, \vec{u}_k\right\}$
	and $\vec{w}^\perp$ can be written as a linear combination of $\left\{\vec{v}_1, \vec{v}_2,\dots, \vec{v}_l\right\}$.

$\beta$ spans $\mathbb{R}^n$, and therefore $\vec{v} = \vec{w}+\vec{w}^\perp$ spans $\mathbb{R}^n$.


Corollary: If $A$ is an $n\times n$ matrix, then $\mathrm{rank}(A)+\mathrm{null}(A)=n$.
