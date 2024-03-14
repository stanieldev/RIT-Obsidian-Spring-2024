
### Microcanonical Ensemble
Equilibrium behavior of $N$ particles in a box of volume $V$.
Energy is conserved within the confines of the volume.
#### Formulation
Consider an isolated system of $k$-dimensions consisting of $N$ particles in a volume $V$.
Configuration space can be defined as $\mathbb{Q}^{(k\times N)}$.
Momentum space can be defined as $\mathbb{P}^{(k\times N)}$.
Phase spaces is the cartesian product of the two prior spaces $\mathbb{Q}^{(k\times N)} \times \mathbb{P}^{(k\times N)}$.

There are $2\times k\times N$ equations:   $\dot{\mathbb{Q}} = m^{-1}\mathbb{P}, \ \ \ \dot{\mathbb{P}} = \mathbb{F}(\mathbb{Q})$.
Where $m$ is the particle masses and $\mathbb{F}$ is an external force due to other particles and the walls.

#### Statistical Energy
We can define the energy differential as the probability density, which can be written in terms of the configuration and momentum spaces of the system.
$$\Omega(E\lt \hat{H} < E + \delta E)\cdot\delta E = \int \mathrm{d}\mathbb{P}\ \mathrm{d}\mathbb{Q}$$
$$\hat{H} = \dfrac{\mathbb{P}^2}{2m} + U(\mathbb{Q}) = \sum_{\alpha=1}^{k\times N} \dfrac{p_\alpha^2}{2m} + U(q_1, q_2,\dots,q_{k\times N})$$
$$\langle A\rangle_E = \dfrac{1}{\Omega(E)\delta E}\int A(\mathbb{P, \mathbb{Q}} )\ \mathrm{d}\mathbb{P}\ \mathrm{d}\mathbb{Q}$$
Taking when $\delta E \rightarrow 0$:
$$\Omega(E = \hat{H}) = \int \mathrm{d}\mathbb{P}\ \mathrm{d}\mathbb{Q}$$
$$\hat{H} = \dfrac{\mathbb{P}^2}{2m} + U(\mathbb{Q}) = \sum_{\alpha=1}^{k\times N} \dfrac{p_\alpha^2}{2m} + U(q_1, q_2,\dots,q_{k\times N})$$
$$\langle A\rangle_E = \dfrac{1}{\Omega(E)}\int A(\mathbb{P, \mathbb{Q}} )\ \mathrm{d}\mathbb{P}\ \mathrm{d}\mathbb{Q}$$
Typically, we use the log of $\Omega$, leading to the definition of *entropy*:
$$S(E) = k_b\log \Omega(E)$$
Therefore we can also express *temperature*:
$$\dfrac{1}{T} = \left.\dfrac{\partial S}{\partial E}\right|_{V,N}$$

### Derivation of Temperature
Consider an isolated system of total energy $E$, consisting of 2 sub-systems with a fixed quantity of particles and volumes $\left(N_A, V_A\right)$ and $\left(N_B, V_B\right)$.
They are weakly connected, with energies $E_A$ and $E_B$, with a combined energy $E = E_A + E_B$.
Equilibrium behavior of the full system assumes equal weight between all states of the 2 subsystems.

Phase Space Volume (assumed systems are weakly coupled):
$$\begin{align}
\Omega(E) &= \int\Omega_A(E_A)\mathrm{d}E_A \cdot \Omega_B(E_B)\mathrm{d}E_B \cdot \delta(E_A+E_B-E) \\
&= \int\Omega_A(E_A)\Omega_B(E-E_A)\cdot \mathrm{d}E_A \\
\end{align}$$
We can then define a probability density:
$$\rho(E_1) = \dfrac{\Omega_A(E_A)\cdot\Omega_B(E-E_A)}{\Omega(E)}$$
At energy equilibrium, probability density will be maximized.
This will occur when $E_A = E_A^*$.
$$\begin{align}
\dfrac{d\rho(E_A)}{dE_A} &= \dfrac{d\Omega_A}{dE_A}\Omega_B+\dfrac{d\Omega_B}{dE_A}\Omega_A \\
0 &= \dfrac{d\Omega_A}{dE_A}\Omega_B+\dfrac{d\Omega_B}{dE_B}\Omega_A \\
\implies& \left.\dfrac{1}{\Omega_A}\dfrac{d\Omega_A}{dE_A}\right|_{E_A^*} = \left.\dfrac{1}{\Omega_B}\dfrac{d\Omega_B}{dE_B}\right|_{E -E_A^*}
\end{align}$$
Using a value of entropy, we can write differentials as:
$$\dfrac{dS}{dE} = k_B \dfrac{1}{\Omega}\dfrac{\partial \Omega}{\partial E}$$
Therefore we can write equilibrium as:
$$\left.\dfrac{dS_A}{dE_A}\right|_{E_A^*}=\left.\dfrac{dS_B}{dE_B}\right|_{E-E_A^*}$$
Define temperature in terms of thermal equilibrium, that total entropy is maximized.
Therefore, temperature is the inverse of entropy per unit energy.
$$\dfrac{1}{T} = \left.\dfrac{\partial S}{\partial E}\right|_{V,N}$$
Expressed as entropy, the Thermodynamic Identity can be written as:
$$\begin{align}
dS &= \dfrac{\partial S}{\partial E}dE + \dfrac{\partial S}{\partial V}dV - \dfrac{\partial S}{\partial N}dN \\
&= \dfrac{1}{T}dE + \dfrac{P}{T}dV - \dfrac{\mu}{T}dN
\end{align}$$


