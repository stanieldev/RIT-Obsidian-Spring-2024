**Date: 2/22/2024**

## Entropy as Disorder

### Entropy of Socks
If a billion children neatened their bedrooms by organizing their socks, how big is the decrease $\Delta S_Q$ of the position-space entropy of their socks?
Assumptions:
 - Each child has 10 distinguishable socks on average.
 - Initially the socks are randomly placed in a bedroom with $V=5\mathrm{m}^3$.
 - Finally the socks end up located in their place in the draw with the COM confined to a region $1\mathrm{cm}^3$.
 - Assume the internal entropies of the socks are unchanged in the process.
#### Solution
$N = 10^9 \times 10=10^{10}$, $V_0=5\mathrm{m}^3$, $V_f=1\mathrm{cm}^3$.
$$\begin{align}
\Delta S &= k_B \log\left(\dfrac{V_f^N}{V_0^N}\right) = k_B N\log\left(\dfrac{V_f}{V_0}\right)\\
&= -1.54\times10^{11}k_B\\
\Aboxed{\Delta S &= -2.13\times10^{-12} \mathrm{\ J/K}}
\end{align}$$
### Air Balloon Configuration Entropy
$V_0=10^{-3}\mathrm{m}^3$, $V_f=0.99\cdot10^{-3}\mathrm{m}^3$
Assumptions:
 - The air inside the balloon are indistinguishable.
 - The air is an ideal gas.
$N=22.4\dfrac{\mathrm{L}}{\mathrm{mol}} \times 1\mathrm{L}$
$$\begin{align}
\Delta S &=  k_B N\log\left(\dfrac{V_f}{V_0}\right)\\ \\
\Aboxed{\Delta S &= -3.73\cdot10^{-3} \mathrm{\ J/K}}
\end{align}$$
#### Comparison
The amount of entropy for the socks example is extremely tiny with respect to reducing a volume of air by 1% of the volume, and so we can say that it is relatively small.

### Other Materials
Liquids tend to have more entropy, since there are more arrangements that lead to the same outcome.

## Entropy of Mixing
Consider a 3D box separated by a partition into two equal volumes $V$.
 - There are $N/2$ undistinguishable ideal yellow gas atoms on one side.
 - There are $N/2$ undistinguishable ideal blue gas atoms on the other side.
### Calculating the Entropy
$$\begin{align}
S_\mathrm{Unmixed} &= 2k_B\log\left(\dfrac{V^{N/2}}{\left(N/2\right)!}\right)\\
S_\mathrm{Mixed} &= 2k_B\log\left(\dfrac{(2V)^{N/2}}{\left(N/2\right)!}\right)\\
\Delta S_\mathrm{Mixing} &= Nk_B\log2\\
\dfrac{\partial S}{\partial N} &= k_B\log2 \ \ \ (\mathrm{Entropy\ per\ Atom})
\end{align}$$
Note, in a system where both gases are undistinguishable with each other, the entropy...

## Residual Entropy of Glasses
What happens at $T=0\mathrm{\ K}$ ?
For systems with a unique ground state, such as elementary crystals, then $S = 0$.
This isn't always the case for all systems.
As $T\rightarrow0$ for glasses, there will be a minimum entropy called the *residual entropy*.
### What Is A Glass?
Disordered like liquids, but have finite rigidity like crystals.
Formed when liquids are cooled too rapidly to form the crystalline equilibrium state.
They are not in equilibrium, unlike an elementary crystal.
### How Do We Measure It?
$$S_\mathrm{Residual} = S_\mathrm{Liquid}(T_l) - \int_0^{T_l} \dfrac{1}{T}\dfrac{\partial Q}{\partial T} dT$$
Where $T_l$ is the temperature of the equilibrium liquid.
