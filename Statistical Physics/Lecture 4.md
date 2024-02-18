**Date: 1/25/2024**
### Diffusion Equation
Einstein-Smoluchowski Equation:
$$\dfrac{\partial \rho(\vec{x}, t)}{\partial t} = D\nabla^2\rho(\vec{x}, t), \ \mathrm{where\ \ } D=\dfrac{\sigma^2}{2\Delta t}$$
The parameter $D$ is the *diffusion constant* of a system.

### Methods of Solving PDEs
There are 2 popular methods for solving PDEs.
#### Fourier Transforms (Computational)
Decompose $\rho(\vec{x}, t)$ into a linear combination of plane-waves:
$$\rho(\vec{x}, t) = \int \tilde{\rho}(\vec{k},t)e^{i\vec{k}\cdot\vec{x}} d\vec{k}$$
Substituting into the diffusion equation:
$$\begin{align}
\dfrac{\partial \rho(\vec{x}, t)}{\partial t} &= \int \dfrac{\partial }{\partial t}\tilde{\rho}(\vec{k},t)e^{i\vec{k}\cdot\vec{x}} d\vec{k} \\
&= \int \dfrac{\partial \tilde{\rho}(\vec{k},t)}{\partial t}e^{i\vec{k}\cdot\vec{x}} d\vec{k}\\
D\nabla^2\rho(\vec{x}, t) &= D\int \nabla^2\tilde{\rho}(\vec{k},t)e^{i\vec{k}\cdot\vec{x}} d\vec{k} \\
&= -D\vec{k}^2\int \tilde{\rho}(\vec{k},t)e^{i\vec{k}\cdot\vec{x}} d\vec{k}
\end{align}$$
Rewriting and solving for $\tilde{\rho}(\vec{k},t)$, we get:
$$\dfrac{\partial \tilde{\rho}(\vec{k}, t)}{\partial t} = -D\vec{k}^2 \tilde{\rho}(\vec{k}, t) \implies \boxed{\tilde{\rho}(\vec{k}, t) = \tilde{\rho}(\vec{k}, 0)e^{-D\vec{k}^2t}}$$
Performing an inverse Fourier transform:
$$\boxed{\rho(\vec{x}, t) = \dfrac{1}{2\pi}\int \tilde{\rho}(\vec{k}, 0)e^{i\vec{k}\cdot\vec{x}-D\vec{k}^2t} d\vec{k}}$$

#### Green's Function (Analytical)
We start with the initial conditions:
$$\begin{align}
\rho(\vec{x}\ne \vec{0}, t=0) &= 0 \\
\rho(\vec{x}=\vec{0}, t=0) &= \delta(\vec{x})
\end{align}$$
Define the Green's function $G(\vec{x}, t)$ to be the time evolution of the density $G(\vec{x}, 0) = \delta(x)$.
In combination with the Fourier method, you can get a closed-form solution.

### Current (Needs fixing)
Since $\rho(\vec{x}, t)$ is a locally conserved quantity, then the net current through space is 0.
Let $J(\vec{x})$ be the current through a point $\vec{x}$, then it can be expressed in terms of $\rho(\vec{x}, t)$:
$$\dfrac{\partial \rho(\vec{x}, t)}{\partial t} =-\nabla I(\vec{x})=-\vec{J}(\vec{x})$$
Based on the *diffusion equation*, one can express the diffusion current as:
$$\vec{I}_\mathrm{diffusion} = -D \nabla \rho(\vec{x},t)$$
On average, diffusion occurs from high density toward lower density, hence the negative sign.

### External Forces (Needs fixing)
$$\dfrac{dx}{dt} = F\gamma, \ \mathrm{where\ } \gamma=\dfrac{D}{mv_0^2}$$
Where $\gamma$ is the *mobility* of the particles.
$$\dfrac{\partial \rho(\vec{x}, t)}{\partial t} = \left(D\nabla^2-\gamma F \cdot  \nabla\right)\rho(\vec{x}, t)$$
With a current resembling:
$$I= \gamma F\rho-D \dfrac{\partial \rho}{\partial x}$$

