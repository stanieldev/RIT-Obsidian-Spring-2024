**Date: 2/27/2024**

### Informational Entropy
For discrete probability distributions:
$$S=-k_B\sum_i\langle\log p_i\rangle = -k_B\sum_i p_i\log p_i$$
For continuous probability distributions:
$$S=-k_B\int \rho(\Omega)\log \rho(\Omega) \ d\Omega$$
For the case where we use the state-space distribution:
$$S=-k_B\int \rho(\mathbb{P}, \mathbb{Q})\log \rho(\mathbb{P}, \mathbb{Q}) \ \mathrm{d}\mathbb{P}\ \mathrm{d}\mathbb{Q}$$
For quantum mechanics, we write it as the following:
$$S=-k_B\mathrm{Tr}\left(\rho\log\rho\right)$$
Where $\rho$ is the density matrix, instead of a scalar field.


### Non-Equilibrium Entropy: Microcanonical Systems
In a microcanonical ensemble, the non-equilibrium entropy is given by
$$S_\mathrm{micro}=-k_B\log\rho_\mathrm{equilibrium}$$
Recall: Probability distributions of states in terms of phase space volume,
$$\rho_\mathrm{equilibrium}=\dfrac{1}{\Omega(E)\delta E}$$
Non-equilibrium entropy in terms of phase space volume,
$$\begin{align}
S_\mathrm{micro}&=-k_B\log\rho_\mathrm{equilibrium}\\
&=k_B\log\left(\Omega(E)\delta E\right)\\
&=k_B\log\Omega(E)+k_B\log\delta E\\
\Aboxed{S_\mathrm{micro}&= S_\mathrm{equilibrium} + k_B\log(\delta E)}
\end{align}$$

### (Mis)Information Entropy
Shannon entropy is written as the following:
$$S = -k_S\sum_ip_i\log p_i$$
For binary, $k_S = \dfrac{1}{\log2}$ and can then be expressed in the following equation:
$$S_\mathrm{Binary} = \sum_ip_i\log_2 p_i$$

