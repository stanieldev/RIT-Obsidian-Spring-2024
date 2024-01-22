Goals of the equation are to find:
$$\begin{align}
\bar{\boldsymbol\theta}&={\arg\min}_\theta\ E(\boldsymbol\theta)\\
E(\boldsymbol\theta) &= \bra{\phi(\boldsymbol\theta)}\hat{H}\ket{\phi(\boldsymbol\theta)}
\end{align}$$
Where $\boldsymbol\theta$ is a vector of real number parametrizations of a trial quantum state.

Note: $\ket{\phi(\boldsymbol\theta)}$ is prepared by Quantum Gates. 










Expected Value of Energy at a Theta Point.
$$\begin{align}
\langle E(\boldsymbol\theta)\rangle &= \sum_{\alpha,\beta=1}^n K(\boldsymbol\theta,\boldsymbol\theta_\alpha)[\bar{K}^{-1}]_{\alpha\beta}E_{\beta} \\
K(\boldsymbol\theta_1,\boldsymbol\theta_2) &= \dfrac{t^{-1}}{(2\pi)^d}\sum_\boldsymbol k e^{i\boldsymbol k\cdot(\boldsymbol\theta_1-\boldsymbol\theta_2)}\\
\bar{K}_{\alpha\beta} &= K(\boldsymbol\theta,\boldsymbol\theta_\alpha) + \sigma_\alpha^2\delta_{\alpha\beta} \\
E_\beta &= \dfrac{1}{N}\sum_{r=1}^NE_{\beta r}
\end{align}$$
Questions about equations:
1) Why is $E_\beta$ have components? It looks to be the mean of single-value measurements.

