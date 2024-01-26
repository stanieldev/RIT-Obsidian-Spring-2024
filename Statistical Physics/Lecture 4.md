### Diffusion Equation
Einstein-Smoluchowski Equation:
$$\dfrac{\partial \rho(\vec{x}, t)}{\partial t} = D\nabla^2\rho(\vec{x}, t), \ \mathrm{where\ \ } D=\dfrac{\sigma^2}{2\Delta t}$$
The parameter $D$ is the *diffusion constant* of a system.

### Methods of Solving PDEs
There are 2 popular methods for solving PDEs.
#### Fourier Transforms (FFTs Computationally)
Decompose $\rho(\vec{x}, t)$ into a linear combination of plane-waves:
$$\rho(\vec{x}, t) = \sum \tilde{\rho}_k(t)e^{ik\vec{x}}$$
Substituting into the diffusion equation:
$$\dfrac{\partial \rho(\vec{x}, t)}{\partial t} = \dfrac{\partial \left(\sum_k \tilde{\rho}_k(t)e^{ik\vec{x}}\right)}{\partial t} = \sum_k\dfrac{\partial \tilde{\rho}_k(t)}{\partial t}e^{ik\vec{x}}$$
$$D\nabla^2\rho(\vec{x}, t) = D\nabla^2\left(\sum_k \tilde{\rho}_k(t)e^{ik\vec{x}}\right) = D\sum_k \tilde{\rho}_k(t)\nabla^2e^{ik\vec{x}}$$
$$\dfrac{\partial \tilde{\rho}_k(t)}{\partial t} = -Dk^2 \tilde{\rho}_k(t) \implies \tilde{\rho}_k(t) = \tilde{\rho}_k(0)e^{-Dk^2t}$$
Converting back to real space using the IFT (FINISH LATER):
$$\rho(\vec{x}, t) = \dfrac{1}{2\pi}\int_{-\infty}^{\infty}\tilde{\rho}_k(\lambda)e^{-\omega \lambda} d\lambda$$


#### Green's Function (Analytical)
We start with the initial conditions:
$$\begin{align}
\rho(\vec{x}\ne \vec{0}, t=0) &= 0 \\
\rho(\vec{x}=\vec{0}, t=0) &= \delta(\vec{x})
\end{align}$$
Define the Green's function $G(\vec{x}, t)$ to be the time evolution of the density $G(\vec{x}, 0) = \delta(x)$.
 - The function obeys the differential equation.
Using the Fourier transform method:
$$\tilde{G}_k(0) = \int G(\vec{x}, 0)e^{-ikx}dx = \int \delta(\vec{x})e^{-ikx}dx = 1$$
$$G(\vec{x}, t) = \dfrac{1}{2\pi}\int e^{ik\vec{x}} \tilde{G}_k(0)e^{-Dk^2t} dk = \dfrac{1}{2\pi}\int e^{ik\vec{x}} e^{-Dk^2t} dk$$
$$\implies G(\vec{x}, t) = \dfrac{1}{\sqrt{4\pi D t}}e^{\tfrac{-x^2}{4Dt}}$$

### Current
Since $\rho(\vec{x}, t)$ is a locally conserved quantity, then the net current through space is 0.
Let $J(\vec{x})$ be the current through a point $\vec{x}$, then it can be expressed in terms of $\rho(\vec{x}, t)$:
$$\dfrac{\partial J(\vec{x})}{\partial x} = -\dfrac{\partial \rho(\vec{x}, t)}{\partial t}$$
Based on the *diffusion equation*, one can express the diffusion current as:
$$J_\mathrm{diffusion} = -D \dfrac{\partial \rho}{\partial x}$$
On average, diffusion occurs from high density toward lower density, hence the negative sign.


### External Forces
$$\dfrac{dx}{dt} = F\gamma, \ \mathrm{where\ } \gamma=\dfrac{D}{mv_0^2}$$
Where $\gamma$ is the *mobility* of the particles.
$$\dfrac{\partial \rho(\vec{x}, t)}{\partial t} = \left(D\nabla^2-\gamma F \cdot  \nabla\right)\rho(\vec{x}, t)$$
With a current resembling:
$$J= \gamma F\rho-D \dfrac{\partial \rho}{\partial x}$$

