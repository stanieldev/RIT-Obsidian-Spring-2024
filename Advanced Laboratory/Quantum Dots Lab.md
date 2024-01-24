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


### Table of Peak Emitted Wavelengths
| Wavelength | $500\mathrm{nm}$ | $520\mathrm{nm}$ | $560\mathrm{nm}$ | $600\mathrm{nm}$ | $620\mathrm{nm}$ | $640\mathrm{nm}$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 1D Square | 8.243e+26 nm | 8.916e+26 nm | 1.034e+27 nm | 1.187e+27 nm | 1.267e+27 nm | 1.351e+27 nm |
| 3D Square | 2.748e+26 nm | 2.972e+26 nm | 3.447e+26 nm | 3.957e+26 nm | 4.228e+26 nm | 4.502e+26 nm |
| 3D Square + Gap | 7.230e-34 nm | 6.684e-34 nm | 5.763e-34 nm | 5.021e-34 nm | 4.702e-34 nm | 4.413e-34 nm |
| 3D Sphere + Gap | 712.6 nm | 712.6 nm | 712.56 nm | 712.56 nm | 712.56 nm | 712.56 nm |
| 3D Sphere + G + Rm | 712.6 nm | 712.6 nm | 712.56 nm | 712.56 nm | 712.56 nm | 712.56 nm |


### Regression Data
| Diameter | Wavelength Peak<br>(Gaussian) | $\chi^2$ | Wavelength Peak<br>(Skewed Voigt) | $\chi^2$ |
| ---- | ---- | ---- | ---- | ---- |
| 500nm | 525.2±0.5 nm | 152.2 | 524.3±0.5 nm | 150.1 |
| 520nm | 535.4±0.8 nm | 170.2 | 538.2±0.8 nm | 146.5 |
| 560nm | 558.3±0.3 nm | 82.02 | 558.3±0.3 nm | 81.30 |
| 600nm | 620.6±0.3 nm | 104.6 | 620.7±0.3 nm | 104.2 |
| 620nm | 635.4±0.1 nm | 124.2 | 635.4±0.1 nm | 124.3 |
| 640nm | 656.7±0.3 nm | 89.20 | 656.7±0.3 nm | 89.23 |
