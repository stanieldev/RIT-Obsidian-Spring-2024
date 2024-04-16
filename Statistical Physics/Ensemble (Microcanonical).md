A Microcanonical Ensemble has:
 - A constant number of particles.
 - A constant amount of internal energy.
 - A constant volume.
### Configuration
$$\begin{align}
&\mathrm{State\ Hamiltonian}&\hat{H}&=\dfrac{\mathbb{P}^2}{2m} + U(\mathbb{Q}) = \sum_{\alpha=1}^{k\times N} \dfrac{p_\alpha^2}{2m} + U(q_1, q_2,\dots,q_{k\times N})\\
&\mathrm{State\ Configuration}&\Omega(E) &= \int \mathrm{d}\mathbb{P}\ \mathrm{d}\mathbb{Q}\\
&\mathrm{State\ Expected\ Value}&\langle A\rangle_E &= \dfrac{1}{\Omega(E)}\int A(\mathbb{P, \mathbb{Q}} )\ \mathrm{d}\mathbb{P}\ \mathrm{d}\mathbb{Q}\\
\end{align}$$
### Derived Quantities
$$\begin{align}
&\mathrm{Entropy}&S(E)&=k_B\log \Omega(E)\\
&\mathrm{Temperature}&\dfrac{1}{T}&=\dfrac{\partial S}{\partial E}\\
&\mathrm{Pressure}&\dfrac{P}{T}&=\dfrac{\partial S}{\partial V}\\
&\mathrm{Chemical\ Potential}&\dfrac{\mu}{T}&=-\dfrac{\partial S}{\partial N}\\
\end{align}$$
### Thermodynamic Potential
Entropy is the thermodynamic potential of a microcanonical ensemble.
$$\begin{align}
&\mathrm{Statistical\ Physics}&dS&=\dfrac{\partial S}{\partial E}dE + \dfrac{\partial S}{\partial V}dV - \dfrac{\partial S}{\partial N}dN \\
&&&=\dfrac{1}{T}dE + \dfrac{P}{T}dV - \dfrac{\mu}{T}dN\\
&\mathrm{Thermodynamics}&dE &= -P dV + TdS + \mu \ dN
\end{align}$$
