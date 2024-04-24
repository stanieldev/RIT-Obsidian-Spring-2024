**Date: 4/23/2024**


### Order Parameter and Criticality in the Ising Model
In specific, near the phase transition.

**Hamiltonian Equation**
$$\hat{H}=-J\sum_{\langle i, j\rangle} s_is_j - H\sum_is_i$$
**Magnetization**
$$m\equiv\dfrac{1}{N}\sum_i\langle s_i\rangle$$
When describing magnetism, magnetization is the order parameter.
When $m=0$, it is the paramagnetic state (disordered spins).
When $m\ne 0$, it is the ferromagnetic state (ordered spins).

We can express the average spin with the following:
$$\langle s_i\rangle=\dfrac{\mathrm{Tr}\left(s_ie^{-\beta\hat{H}}\right)}{Z}, Z=\mathrm{Tr}\left(e^{-\beta\hat{H}}\right)$$
It is the ensemble average spin for the system.


### Mean Field Theory
Gives analytical answers to get an approximation of the qualitative behavior.

MFT assumes the thermal fluctuations are small and can be neglected to a certain extent.
Can be treated as a system of interacting with an average field of the neighbor contributions.
MFT decouples the Hamiltonian into a non-interacting system.
It also allows for solving things we cannot solve directly.

$s_i = \langle s_i\rangle + \delta s_i \implies s_is_j=-\langle s_i\rangle\langle s_j\rangle + \langle s_i\rangle\delta s_j + \langle s_j\rangle\delta s_i + \delta s_i\delta s_j$

Given $q$ as the coordinate number ($4$ for square, $6$ for triangles).
$$\begin{align}
\hat{H}_\mathrm{ME}&=-mJ\sum_{\langle i, j\rangle} (s_i+s_j-m) - H\sum_is_i\\
&=-mJ\sum_{\langle i, j\rangle} (2s_i-m) - H\sum_is_i\\
&=-mJ\dfrac{q}{2}\sum_{i} (2s_i-m) - H\sum_is_i\\
&=-mJq\sum_{i} s_i - H\sum_is_i+m^2J\dfrac{q}{2}N\\
\Aboxed{\hat{H}_\mathrm{ME} &= \left(\dfrac{qJm^2}{2}\right)N-(mJq+H)\sum_is_i}\\
\Aboxed{\hat{H}^0_\mathrm{ME} &= -(mJq+H)\sum_is_i}
\end{align}$$
The coefficient outside the sum becomes the effective magnetic field.

$$\begin{align}
Z&=\mathrm{Tr}\left(e^{-\beta\hat{H}}\right)\\
&=\prod_i\sum_{s_i=\pm1}e^{-\beta\hat{H}}\\
&=\prod_i\sum_{s_i=\pm1}e^{-\beta\left(\tfrac{qJm^2}{2}\right)N+\beta(mJq+H)s_i}\\
&=e^{-\beta\left(\tfrac{qJm^2}{2}\right)N}\prod_i\sum_{s_i=\pm1}e^{\beta(mJq+H)s_i}\\
&=e^{-\beta\left(\tfrac{qJm^2}{2}\right)N}\prod_i\left(e^{\beta(mJq+H)}+e^{-\beta(mJq+H)}\right)\\
&=e^{-\beta\left(\tfrac{qJm^2}{2}\right)N}\prod_i2\cosh\left(\beta(mJq+H)\right)\\
&=e^{-\beta\left(\tfrac{qJm^2}{2}\right)N}2^N\cosh\left(\beta(mJq+H)\right)^N\\
Z &=\left(e^{-\beta\left(\tfrac{qJm^2}{2}\right)}2\cosh\left(\beta(mJq+H)\right)\right)^N\\
\Aboxed{Z&=\left(e^{-\beta\left(\tfrac{qJm^2}{2}\right)}2\cosh\left(\beta(H_\mathrm{eff})\right)\right)^N}
\end{align}$$

For magnetization, we can write $m$ as:
$$\begin{align}
m&=\dfrac{1}{N\beta}\dfrac{1}{Z_\mathrm{MF}}\dfrac{\partial Z_\mathrm{MF}}{\partial H_\mathrm{eff}}\\
&= \dfrac{1}{N\beta}\dfrac{\partial \log Z_\mathrm{MF}}{\partial H_\mathrm{eff}}\\
\Aboxed{m &= \tanh(\beta H_\mathrm{eff})}
\end{align}$$
Critical temperature is when $k_BT_c = qJ \implies T_c = \dfrac{qJ}{k_B}$
Below that temperature, there are 3 intercepts at 0 and $\pm m_0$.
That is when it is ferromagnetic (spontaneous magnetization when H=0).

