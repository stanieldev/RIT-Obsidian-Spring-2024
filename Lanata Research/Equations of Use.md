Let $\hat{H}$ be a Hamiltonian on a wavefunction $\ket{\Psi(\theta)}$, where $\theta = \theta^i e_i$ are real numbers.
Our goal is to determine:
$$\begin{align}
\theta_\mathrm{min}&={\arg\min}_\theta\ E(\theta)\\
E(\theta) &= \bra{\phi(\theta)}\ \hat{H}\ \ket{\phi(\theta)}
\end{align}$$
State $\ket{\phi(\theta)}$ can be prepared by quantum gates, leading to:
$$\ket{\phi(\theta)} = \hat{U}(\theta)\ \ket{\phi_0}$$
Where the unitary matrix can be represented as:
$$\hat{U}(\theta) = \prod_{l=1}^d\prod_{m=1}^{M_l} e^{i\hat{G}_{lm}\tfrac{\theta^l}{2}}$$





Energy:
$$\langle E(\theta)\rangle = \sum_{\alpha=1}^n\sum_{\beta=1}^n K(\theta,\theta_\alpha)[\bar{K}^{-1}]_{\alpha\beta}E_{\beta}$$
K function:
$$K(\theta_1,\theta_2) = \dfrac{t^{-1}}{(2\pi)^d}\sum_\vec{k} e^{i\vec{k}\cdot(\theta_1-\theta_2)}$$
K^-1 function
$$\bar{K}_{\alpha\beta} = K(\theta_i,\theta_j) + \sigma_i^2\delta_{ij}$$



The items ($E_{\beta}$, $\theta_\alpha$, $\sigma_i$) come from the quantum computer data.

$n$ is the number of components of $\theta$.
$t$ encodes prior information about the range of variational energy.





















Expected Value of Energy at a Theta Point.
$$\begin{align}
\langle E(\boldsymbol\theta)\rangle &= \sum_{\alpha,\beta=1}^n K(\boldsymbol\theta,\boldsymbol\theta_\alpha)[\bar{K}^{-1}]_{\alpha\beta}E_{\beta} \\
K(\boldsymbol\theta_1,\boldsymbol\theta_2) &= \dfrac{t^{-1}}{(2\pi)^d}\sum_\boldsymbol k e^{i\boldsymbol k\cdot(\boldsymbol\theta_1-\boldsymbol\theta_2)}\\
\bar{K}_{\alpha\beta} &= K(\boldsymbol\theta,\boldsymbol\theta_\alpha) + \sigma_\alpha^2\delta_{\alpha\beta} \\
E_\beta &= \dfrac{1}{N}\sum_{r=1}^NE_{\beta r}
\end{align}$$
Questions about equations:
1) Why is $E_\beta$ have components? It looks to be the mean of single-value measurements.

