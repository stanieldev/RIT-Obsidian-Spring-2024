A Canonical Ensemble has:
 - A constant number of particles.
 - A constant chemical potential.
 - A constant temperature.
 - A constant volume.
### Configuration
$$\begin{align}
&\mathrm{Probability\ Density}&\rho(s)&=\dfrac{1}{Z}e^{-\tfrac{E_s}{k_BT}}\\
&\mathrm{Partition\ Function}&Z&=\displaystyle\sum_se^{-\tfrac{E_s}{k_BT}}\\
&\mathrm{Expected\ Value}&\langle A\rangle &=\dfrac{1}{Z}\displaystyle\sum_sAe^{-\tfrac{E_s}{k_BT}}
\end{align}$$
### Derived Quantities
For reference, $\beta=\dfrac{1}{k_BT}$.
$$\begin{align}
&\mathrm{Helmholz\ Energy}&F&=-k_BT\log Z\\
&\mathrm{Entropy}&S&=-\dfrac{\partial F}{\partial T}\\
&\mathrm{Pressure}&P&=-\dfrac{\partial F}{\partial V}\\
&\mathrm{Chemical\ Potential}&\mu&=\dfrac{\partial F}{\partial N}\\
&\mathrm{Average\ Energy}&\langle E\rangle&=-\dfrac{\partial \log Z}{\partial \beta}\\
&\mathrm{Specific\ Heat}&C_V&=\dfrac{1}{N k_B T^2}\dfrac{\partial^2 \log Z}{\partial \beta^2}\\
\end{align}$$
### Thermodynamic Potential
Helmholtz free energy is the thermodynamic potential of a canonical ensemble.
$$\begin{align}
&\mathrm{Quantity}&F &= U - TS\\
&\mathrm{Relationship}&dF &= -P dV - SdT + \mu \ dN
\end{align}$$
