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
$$\begin{align}
E_\gamma &= \boxed{\dfrac{3h^2}{8m_eD^2}}
\end{align}$$
$$\begin{align}\lambda &= \boxed{\dfrac{8m_ec^2D^2}{3hc}}\end{align}$$
### 3-Dimensional Infinite Cube Potential Well with Gap Energy
$$\begin{align}
E_\gamma &= \boxed{\dfrac{3h^2}{8m_eD^2} + |E_g|}
\end{align}$$
$$\begin{align}
\lambda &= \dfrac{hc}{\dfrac{3(hc)^2}{8(m_ec^2)D^2} + |E_g|}
\end{align}$$
### Infinite Spherical Potential Well with Gap Energy
$$E_{n,l} = z_{n,l}\cdot\dfrac{\hbar^2}{2mD^2}, \mathrm{\ where\ } z_{n,l} \mathrm{\ are\ the\ zeros\ of\ the\ Bessel\ function.}$$
$$\begin{align}
E_\gamma &= \boxed{\dfrac{\hbar^2}{2mD^2}\left(\pi-0\right) + |E_g|}
\end{align}$$
$$\begin{align}
\lambda &= \dfrac{hc}{\dfrac{\pi(hc)^2}{8\pi^2(m_ec^2)D^2} + |E_g|}
\end{align}$$
### Adjusted Infinite Spherical Potential Well with Gap Energy
$$\lambda = \dfrac{hc}{\dfrac{h^2}{2m_e^*D^2}+\dfrac{h^2}{2m_h^*D^2}+|E_g|}$$
