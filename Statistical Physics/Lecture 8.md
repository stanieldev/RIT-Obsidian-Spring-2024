For microcanonical systems, the *entropy* is a thermodynamic potential, following:
$$\begin{align}
dS &= \dfrac{1}{T}dE + \dfrac{P}{T}dV - \dfrac{\mu}{T}dN \ \mathrm{\ \ \ (Statistical\ Physics)}\\
\implies dE &= -P dV + TdS + \mu \ dN \ \ \ \ \mathrm{\ \ \ (Thermodynamics)}
\end{align}$$
Maxwell relations are based on the symmetry of taking differentials.
Suppose that $dN = 0$ (constant number of particles), we can find that:
$$\dfrac{\partial}{\partial S}\dfrac{\partial E}{\partial V}=\dfrac{\partial}{\partial V}\dfrac{\partial E}{\partial S} \implies \boxed{-\dfrac{\partial P}{\partial S} = \dfrac{\partial T}{\partial V}}$$

Extensive Quantities : Dependent on physical dimensions of the system.
 - Values that change linearly (sum) when 2 systems are merged.
 - Energy $(E)$
 - Entropy $(S)$
Intensive Quantities : Independent of physical dimensions of the system.
 - Values that don't change linearly (sum) when 2 systems are merged.
 - Temperature $(T)$
Faster Quantities:
 - Phase Volume $(\Omega)$, since it scales by the product.

### Microcanonical Ideal Gas
The potential between all particles is 0, as in they have no effect on each other.
It's also assumed this idea gas is in 3-dimensional space.
$$\hat{H} = \dfrac{\mathbb{P}^2}{2m} = \sum_{\alpha=1}^{3N} \dfrac{p_\alpha^2}{2m}$$
$$\begin{align}
\Omega(E=\hat{H}) &= \int \mathrm{d}\mathbb{P}\ \mathrm{d}\mathbb{Q} \\
&= \int \mathrm{d}\mathbb{P} \int\mathrm{d}\mathbb{Q} \ \ \ \mathrm{(Independent)} \\
&= \dfrac{V^N}{N!} \cdot \mathbb{S}^{3N-1}_{\sqrt{2mE}} \ \ \ \mathrm{(Classical, Indistinguishable)} \\
&= \dfrac{V^N}{N!} \cdot \dfrac{\partial}{\partial E}\left(\dfrac{\sqrt{\pi^{3N}(2mE)^{3N}}}{\left(\tfrac{3N}{2}\right)!}\right) \\
&= \dfrac{V^N}{N!} \cdot \left(\dfrac{3N}{2E}\right) \cdot \dfrac{\sqrt{\pi^{3N}(2mE)^{3N}}}{\left(\tfrac{3N}{2}\right)!} \\
\Aboxed{\Omega(E)&\approx \dfrac{1}{h^{3N}} \cdot \dfrac{V^N}{N!} \cdot \dfrac{\sqrt{\pi^{3N}(2mE)^{3N}}}{\left(\tfrac{3N}{2}\right)!}} \ \ \ \mathrm{(To\ make\ unitless)}
\end{align}$$
To find the entropy of the system, we can take the natural log:
$$\begin{align}
S &= k_B \log\left(\Omega(E)\right) \\
&= k_B \log\left(\dfrac{1}{h^{3N}} \cdot \dfrac{V^N}{N!} \cdot \dfrac{\sqrt{\pi^{3N}(2mE)^{3N}}}{\left(\tfrac{3N}{2}\right)!}\right) \\
&= -3Nk_B\log\left(h\right)+Nk_B\log\left(V\right)-k_B\log\left(N!\right)+\dfrac{3N}{2}k_B\log\left(2\pi mE\right)-k_B\log\left(\left(\tfrac{3N}{2}\right)!\right) \\
&\approx S = Nk_B\left(\dfrac{5}{2}-\log\left(\rho\lambda^3\right)\right)
\end{align}$$
Where $\rho = N/V$ and $\lambda = \dfrac{h}{\sqrt{4\pi m E/3N}}$.

Temperature can then be found with:
$$\dfrac{1}{T} = \dfrac{\partial S}{\partial E} \implies T = \dfrac{3Nk_B}{2E}$$
Leading directly to the equipartition energy theorem.








