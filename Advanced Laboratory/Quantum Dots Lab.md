### 1-Dimensional Infinite Square Potential Well
$$-\dfrac{\hbar^2}{2m}\dfrac{\partial^2 \psi}{\partial x^2}+V(x)\psi = E\psi$$
$$V(x)=\begin{cases}
0&0\le x\le D\\
\infty&x\lt 0, x\gt D\\
\end{cases}$$
For the case where $0\le x\le D$, the Schrödinger equation can be rewritten as:
$$-\dfrac{\hbar^2}{2m}\dfrac{\partial^2 \psi}{\partial x^2} = E\psi \implies 
\dfrac{\partial^2 \psi}{\partial x^2} = -\dfrac{2mE}{\hbar^2}\psi$$
This is a simple case of sine and cosine waves. Letting $k^2 = \dfrac{2mE}{\hbar^2}$:
$$\psi(x) = A\sin(k x)+B\cos(k x)$$
Using the initial conditions $\psi(0)=\psi(D)=0$:
$$\psi(x) = A\sin(k x), \mathrm{\ where\ } k = \dfrac{n\pi}{D}$$
With the 2 expressions for $k$, we can set them equal and find energy:
$$E=\left(\dfrac{n\pi}{D}\right)^2\dfrac{\hbar^2}{2m} = \dfrac{h^2}{8mD^2}\cdot n^2$$
To find the energy of the emitted wavelength, we notice that it must conserve energy:
$$E_\gamma = -\Delta E$$
Note: Since the particle in the 1D box is an electron, $m = m_e$.
$$\begin{align}
E_\gamma &= -\Delta E\\
&= -\left(\dfrac{h^2}{8m_eD^2}\cdot 0^2-\dfrac{h^2}{8m_eD^2}\cdot 1^2\right)\\
E_\gamma &= \boxed{\dfrac{h^2}{8m_eD^2}}
\end{align}$$
With a wavelength:
$$\dfrac{hc}{\lambda}=\dfrac{h^2}{8m_eD^2}\left(1^2-0^2\right)$$
$$\boxed{\lambda=\dfrac{8m_ec^2D^2}{hc}}$$
### 3-Dimensional Infinite Cube Potential Well
$$E_n=\dfrac{h^2}{8m_eD^2}\left(\vec{n}\cdot\vec{n}\right)=\dfrac{h^2}{8m_eD^2}\left(n_x^2+n_y^2+n_z^2\right)$$
$$E_\gamma = \boxed{\dfrac{3h^2}{8m_eD^2}}, \ \ \lambda = \boxed{\dfrac{8m_ec^2D^2}{3hc}}$$

### 3-Dimensional Infinite Cube Potential Well with Gap Energy
$$E_\gamma = \boxed{\dfrac{3h^2}{8m_eD^2} + |E_g|}, \ \ \lambda = \boxed{\dfrac{hc}{\dfrac{3(hc)^2}{8(m_ec^2)D^2} + |E_g|}}$$

### Infinite Spherical Potential Well with Gap Energy
$$E_{n,l} = z_{n,l}^2\cdot\dfrac{\hbar^2}{2mD^2}, \mathrm{\ where\ } z_{n,l} \mathrm{\ are\ the\ zeros\ of\ the\ Bessel\ function.}$$
$$E_\gamma = \boxed{\dfrac{\hbar^2}{2mD^2}\left(\pi^2-0^2\right) + |E_g|}, \ \ \lambda = \boxed{\dfrac{hc}{\dfrac{(hc)^2}{8(m_ec^2)D^2} + |E_g|}}$$

### Adjusted Infinite Spherical Potential Well with Gap Energy
$$\lambda = \dfrac{hc}{\dfrac{h^2}{2\mu D^2}+|E_g|}, \ \ \ \mu=\dfrac{m_e^*m_h^*}{m_e^*+m_h^*}$$



### Cadmium Selenide Regression Data
| Diameter | Gauss Peak | HWHM | $\chi^2$ | Voigt Peak | HWHM | $\chi^2$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 2.3nm | 525.2nm | 30.42nm | 152.2 | 524.3nm | 26.94nm | 150.1 |
| 2.6nm | 535.3nm | 87.58nm | 133.7 | 507.9nm | 17.73nm | 75.51 |
| 3.3nm | 558.3nm | 14.52nm | 85.96 | 558.3nm | 15.62nm | 85.22 |
| 4.6nm | 620.6nm | 9.550nm | 104.6 | 620.7nm | 10.43nm | 104.2 |
| 5.6nm | 635.4nm | 18.70nm | 124.2 | 635.4nm | 18.58nm | 124.3 |
| 6.9nm | 656.7nm | 13.24nm | 83.03 | 656.7nm | 16.11nm | 82.69 |


### Indium Phosphide Regression Data
| Diameter | Gauss Peak | HWHM | $\chi^2$ | Voigt Peak | HWHM | $\chi^2$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 4.7nm | 520.7nm | 46.34nm | 371.5 | 528.7nm | 24.96nm | 20.27 |
| 5.1nm | 568.5nm | 32.78nm | 545.3 | 568.2nm | 17.33nm | 89.83 |
| 5.4nm | 596.6nm | 30.04nm | 519.8 | 596.9nm | 23.71nm | 90.51 |
| 5.8nm | 620.7nm | 35.37nm | 444.3 | 621.2nm | 30.08nm | 218.2 |



| Model Name | $\chi_\mathrm{total}^2$ | $\chi^2$ |
| ---- | ---- | ---- |
| 1D Square Well | 1.757e+8 | 3.514e+7 |
| 3D Square Well | 1.903e+8 | 3.806e+6 |
| 3D Square Well + $E_g$ | 178.1 | 35.63 |
| 3D Spherical Well + $E_g$ | 284.9 | 56.98 |
| 3D Spherical Well + $E_g$ & $\mu$ | 17.94 | 3.587 |



