
## Application of Statistical Ensembles In QSM Systems



### Quantum Harmonic Oscillator

$E_n = \left(n+\dfrac{1}{2}\right)\hbar\omega$

Partition Function:
$$\begin{align}
Z&=\sum_{n=0}^\infty e^{-\beta E_n}\\
&=\sum_{n=0}^\infty e^{-\beta \left(n+\dfrac{1}{2}\right)\hbar\omega}\\
&=e^{-\tfrac{\beta\hbar\omega}{2}}\sum_{n=0}^\infty \left(e^{-\beta \hbar\omega}\right)^n\\
&=e^{-\tfrac{\beta\hbar\omega}{2}}\cdot\dfrac{1}{1-e^{-\beta \hbar\omega}}\\
\Aboxed{Z&=e^{-\tfrac{\beta\hbar\omega}{2}}\cdot\left(1-e^{-\beta \hbar\omega}\right)^{-1}}
\end{align}$$
Average Energy & Average Number:
$$\begin{align}
\langle E\rangle &= -\dfrac{\partial \log Z}{\partial \beta}\\
&= \dfrac{\partial}{\partial\beta}\left(\dfrac{\beta\hbar\omega}{2}+\log\left(1-e^{-\beta \hbar\omega}\right)\right)\\
\Aboxed{\langle E\rangle&=\hbar\omega\left(\dfrac{1}{e^{\beta \hbar\omega}-1}+\dfrac{1}{2}\right)}\\
\Aboxed{\langle n\rangle&=\dfrac{1}{e^{\beta \hbar\omega}-1}}
\end{align}$$

### Grand Canonical in Quantum Statistical Mechanics
We are assuming that the particle eigenstates are non-interacting.
$Z=\displaystyle\prod_k Z_k$

For **Bosons**:
$Z_k^{\mathrm{Boson}} = \displaystyle\sum_{n_k=0}^\infty e^{-\beta(\epsilon_k-\mu)n_k} = \dfrac{1}{1-e^{-\beta(\epsilon_k-\mu)}}$
$Z^\mathrm{Boson}=\displaystyle\prod_k \dfrac{1}{1-e^{-\beta(\epsilon_k-\mu)}}$
$\begin{align}\Phi^\mathrm{Boson} &= \displaystyle\sum_k\Phi_k^\mathrm{Boson}\\ &= \displaystyle\sum_k k_BT\log\left(1-e^{-\beta(\epsilon_k-\mu)}\right) \end{align}$

Copy this down later.
$\langle n\rangle_\epsilon= \dfrac{1}{e^{\beta(\epsilon-\mu)}-1}$


For **Fermions**:
$Z_k^{\mathrm{Fermion}} = \displaystyle\sum_{n_k=0}^1 e^{-\beta(\epsilon_k-\mu)n_k} = 1+e^{-\beta(\epsilon_k-\mu)}$
$Z^\mathrm{Fermion}=\displaystyle\prod_k \dfrac{1}{1-e^{-\beta(\epsilon_k-\mu)}}$
$\begin{align}\Phi^\mathrm{Fermion} &= \displaystyle\sum_k\Phi_k^\mathrm{Fermion}\\ &= \displaystyle\sum_k k_BT\log\left(1+e^{-\beta(\epsilon_k-\mu)}\right) \end{align}$

$\langle n\rangle_\epsilon= \dfrac{1}{e^{\beta(\epsilon-\mu)}+1}$
