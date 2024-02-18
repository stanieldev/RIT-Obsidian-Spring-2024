1. Refer to Figure 1 in the MI Lab Manual.
![[interferometer.png|400]]

2. Sketch a copper rod of length $l$ at room temperature $T_0$, with one end of the rod attached to the rear of Mirror 2.
![[interferometer2.png|400]]

3. Sketch a displacement of the mirror after the copper rod is heated, and has expanded  
to a new length $l + \Delta l$.
![[interferometer3.png|400]]

4. Express the change in the difference in path length for light that travels down the $L_2$ arm of the interferometer in terms of $\Delta l$.
$$\Delta s = 2\left[(l+\Delta l) - (l)\right] = 2\Delta l$$
5. During this heating of the rod, you observe $N$ complete fringes pass on the oscilloscope, indicating that the change in the difference in path length was equal to $N\lambda$. Solve for $\Delta l$ in terms of $N\lambda$.
$$\Delta s = N\lambda = 2\Delta l \implies \boxed{\Delta l =\dfrac{N\lambda}{2}}$$



$$d\sin(\theta) = n\lambda \implies d \cdot \dfrac{\Delta x}{\sqrt{L^2+(\Delta x)^2}} = n \lambda$$
Where $d$ is the distance between the diffraction grating slits, $\Delta x$ is the distance of a bright spot from the center of the grating, $L$ is the distance between the grating and the flat surface, and $n$ being the diffraction order based on order counted from the center.

$$\lambda = \dfrac{d}{n} \cdot \dfrac{\Delta x}{\sqrt{L^2+(\Delta x)^2}}$$
$$\delta\lambda = \lambda \sqrt{\left(\dfrac{1}{\Delta x}+\dfrac{\Delta x}{L^2+(\Delta x)^2}\right)^2\delta (\Delta x)^2 + \left(\dfrac{L}{L^2+(\Delta x)^2}\right) \delta L^2}$$

$$\lambda = (627.9 \pm 5.4)\mathrm{\ nm}$$

$$627.9-632.990 \approx 95\% \ \delta \lambda$$







$$\begin{aligned}
\delta\left(\dfrac{\Delta l}{L_0}\right) &= \sqrt{\left(\dfrac{\tfrac{\Delta l}{L_0}}{N}\right)^2\delta N^2+\left(\dfrac{\tfrac{\Delta l}{L_0}}{\lambda}\right)^2\delta \lambda^2+\left(\dfrac{\tfrac{\Delta l}{L_0}}{L_0}\right)^2\delta L_0^2} \\
&= \dfrac{\Delta l}{L_0}\sqrt{\left(\dfrac{\delta \lambda}{\lambda}\right)^2+\left(\dfrac{\delta L_0}{L_0}\right)^2} \\
&= \dfrac{\Delta l}{L_0}\sqrt{\left(\dfrac{2\mathrm{\ nm}}{632.990\mathrm{\ nm}}\right)^2+\left(\dfrac{0.01\mathrm{\ nm}}{64.66\mathrm{\ nm}}\right)^2} \\
&\approx \left(3.164\cdot 10^{-3}\right) \dfrac{\Delta l}{L_0}
\end{aligned}$$



### Copper Heating Thermal Expansion
| Trial | $\alpha \ (\degree C^{-1})$ | $\delta\alpha \ (\degree C^{-1})$ | $r^2$ | $\chi_T^2$ | $\chi^2$ | $p(\chi^2)$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | $15.5\cdot10^{-6}$ | $\lt0.1\cdot10^{-6}$ | $99.92\%$ | $2.44\cdot10^{-9}$ | $2.06\cdot10^{-11}$ | $\approx100\%$ |
| 2 | $17.3\cdot10^{-6}$ | $\lt0.1\cdot10^{-6}$ | $99.86\%$ | $4.73\cdot10^{-9}$ | $4.00\cdot10^{-11}$ | $\approx100\%$ |
$$\overline{\alpha} = 16.4\cdot 10^{-6} K^{-1}, \ \ \ s_\overline{\alpha} = 0.64\cdot 10^{-6} K^{-1}$$


### Copper Cooling Thermal Contraction
| Trial | $\alpha \ (\degree C^{-1})$ | $\delta\alpha \ (\degree C^{-1})$ | $r^2$ | $\chi_T^2$ | $\chi^2$ | $p(\chi^2)$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | $17.9\cdot10^{-6}$ | $\lt0.1\cdot10^{-6}$ | $99.98\%$ | $2.95\cdot10^{-10}$ | $2.63\cdot10^{-12}$ | $\approx100\%$ |
| 2 | $17.8\cdot10^{-6}$ | $\lt0.1\cdot10^{-6}$ | $99.99\%$ | $2.58\cdot10^{-10}$ | $2.31\cdot10^{-12}$ | $\approx100\%$ |

$$\overline{\alpha} = 17.9\cdot 10^{-6} K^{-1}, \ \ \ s_\overline{\alpha} = 0.04\cdot 10^{-6} K^{-1}$$










### Index of Refraction (Vacuum Pulling)
| Trial | $\dfrac{dn}{dP}  \ (\mathrm{atm}^{-1})$ | $\delta\left(\dfrac{dn}{dP}\right)  \ (\mathrm{atm}^{-1})$ | $r^2$ | $\chi_T^2$ | $\chi^2$ | $p(\chi^2)$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | $2.23\cdot10^{-4}$ | $0.03\cdot10^{-4}$ | $99.32\%$ | $1.91\cdot10^{-9}$ | $2.81\cdot10^{-11}$ | $\approx100\%$ |
| 2 | $2.44\cdot10^{-4}$ | $0.02\cdot10^{-4}$ | $99.78\%$ | $6.14\cdot10^{-10}$ | $9.03\cdot10^{-12}$ | $\approx100\%$ |
| 3 | $2.51\cdot10^{-4}$ | $0.01\cdot10^{-4}$ | $99.89\%$ | $2.90\cdot10^{-10}$ | $4.26\cdot10^{-12}$ | $\approx100\%$ |
| 4 | $2.63\cdot10^{-4}$ | $0.02\cdot10^{-4}$ | $99.79\%$ | $5.69\cdot10^{-10}$ | $8.37\cdot10^{-12}$ | $\approx100\%$ |
| 5 | $2.62\cdot10^{-4}$ | $0.01\cdot10^{-4}$ | $99.88\%$ | $7.30\cdot10^{-12}$ | $2.15\cdot10^{-13}$ | $\approx100\%$ |
$$\overline{n_P} = 2.486\cdot 10^{-4} \ (\mathrm{atm}^{-1}), \ \ \ s_\overline{n_P} = 0.04\cdot 10^{-4} \ (\mathrm{atm}^{-1})$$
### Index of Refraction (Vacuum Releasing)
| Trial | $\dfrac{dn}{dP}  \ (\mathrm{atm}^{-1})$ | $\delta\left(\dfrac{dn}{dP}\right)  \ (\mathrm{atm}^{-1})$ | $r^2$ | $\chi_T^2$ | $\chi^2$ | $p(\chi^2)$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | $2.65\cdot10^{-4}$ | $0.01\cdot10^{-4}$ | $99.95\%$ | $1.48\cdot10^{-10}$ | $2.15\cdot10^{-12}$ | $\approx100\%$ |
| 2 | $2.49\cdot10^{-4}$ | $0.02\cdot10^{-4}$ | $99.75\%$ | $6.69\cdot10^{-10}$ | $9.99\cdot10^{-12}$ | $\approx100\%$ |
| 3 | $2.62\cdot10^{-4}$ | $0.01\cdot10^{-4}$ | $99.90\%$ | $2.93\cdot10^{-10}$ | $4.18\cdot10^{-12}$ | $\approx100\%$ |
| 4 | $2.57\cdot10^{-4}$ | $0.02\cdot10^{-4}$ | $99.88\%$ | $3.58\cdot10^{-10}$ | $5.12\cdot10^{-12}$ | $\approx100\%$ |
| 5 | $2.65\cdot10^{-4}$ | $0.02\cdot10^{-4}$ | $99.91\%$ | $1.18\cdot10^{-11}$ | $4.90\cdot10^{-13}$ | $\approx100\%$ |
$$\overline{n_P} = 2.596\cdot 10^{-4} \ (\mathrm{atm}^{-1}), \ \ \ s_\overline{n_P} = 0.02\cdot 10^{-4} \ (\mathrm{atm}^{-1})$$


**Table 1:** A collection of experimental values of the thermal expansion of copper as it heats up.

Taking the mean and standard error of $\alpha$, we that that:
$$\overline{\alpha} = 6.96\cdot10^{-6}, \ \ \ \dfrac{\sigma_{\alpha}}{\sqrt{N}} = 0.09\cdot10^{-6}$$


$$F_\mathrm{expansion} - k\left(\Delta l_\mathrm{true}-\dfrac{N\lambda}{2}\right)$$

$$\Delta l_\mathrm{true} = \dfrac{N\lambda}{2}$$



$$M=2L\dfrac{n-1}{\lambda} \implies \boxed{n=\dfrac{M\lambda}{2L}+1}$$
$$\delta n = n\sqrt{\left(\dfrac{\delta\lambda}{\lambda}\right)^2+\left(\dfrac{\delta L}{L}\right)^2}$$
