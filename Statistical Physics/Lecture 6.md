**Date: 2/1/2024**
<hr>

Random walks diffuse at long times, with $\langle x^2\rangle \propto Dt$, with a proportionality constant that depends on the dimensions.

At short times, in most cases, the motion is ballistic, meaning it's a straight line with constant velocity (or no acceleration).

The cross-over from ballistic motion and diffusion is a decaying exponential:
$$\left\langle\dfrac{d(r^2)}{dt}\right\rangle = 2D\left(1-e^{-\tfrac{t}{\Delta t}}\right)$$
As $t \rightarrow 0$, we can express this equation as:
$$\left\langle\dfrac{d(r^2)}{dt}\right\rangle = 2D\left(1-\left(1-\dfrac{t}{\Delta t}\right)\right) = \dfrac{2Dt}{\Delta t}$$
$$\left\langle r^2\right\rangle = \left(\dfrac{D}{\Delta t}\right)t^2, \ \ \ t \rightarrow 0$$
As $t \rightarrow \infty$, we can express this equation as: 
$$\left\langle\dfrac{d(r^2)}{dt}\right\rangle = 2D$$
$$\left\langle r^2\right\rangle = 2Dt, \ \ \ t \rightarrow \infty$$
For an exact value, we can integrate both sides to get the following:
$$\left\langle r^2\right\rangle = \int_0^t \left\langle\dfrac{d(r^2)}{dt}\right\rangle dt = 2D\left(t+ \Delta t \cdot e^{-\tfrac{t}{\Delta t}}\right|_0^t = 2Dt + 2D \Delta t\left(e^{-\tfrac{t}{\Delta t}} - 1\right)$$




### Problem 2.22
$$v'(t) = \sum_\alpha\left(v_\alpha+(F/m)\right)\left(t'-t_\alpha\right)\Theta\left(t'-t_\alpha\right)\Theta\left(t_{\alpha+1}-t'\right)$$
Where $\Theta$ is the Heaviside step function (0 for negative, 1 for positive).
We assume the following as well:
$$\begin{align}
\langle v_\alpha\rangle &= 0 \\
\langle v_\alpha v_\beta\rangle &= \delta_{\alpha\beta}
\end{align}$$
Use also the distribution:
$$\rho(t) = \dfrac{1}{\Delta t}e^{-\tfrac{t}{\Delta t}}$$

a) Show the expectation value of $\langle v(t) \rangle$ is given by $F/m$ times the mean time $\langle t - t_\Omega \rangle$ since the last collision. Calculate the mobility in terms of $\Delta t$ and $m$.

Since $t_\Omega \lt t \lt t_{\Omega+1}$, equation 2.41 tells us that
$$v(t) = v_\Omega + \dfrac{F}{m}\left(t-t_\Omega\right)$$
$$\begin{align}
\langle v(t) \rangle &= \langle v_\Omega \rangle + \left\langle \dfrac{F}{m}\left(t-t_\Omega\right) \right\rangle = \dfrac{F}{m}\left\langle t-t_\Omega\right\rangle \\
&= \dfrac{F}{m}\int_{-\infty}^t (t-t_\Omega)\rho(t-t_\Omega) dt_\Omega \\
&= \dfrac{F}{m}\dfrac{1}{\Delta t}\int_{-\infty}^t (t-t_\Omega)e^{-\tfrac{t-t_\Omega}{\Delta t}} dt_\Omega \\
&= \dfrac{F}{m}\dfrac{1}{\Delta t}\int_{-\infty}^t (t-t_\Omega)e^{-\tfrac{t-t_\Omega}{\Delta t}} dt_\Omega \\
\Aboxed{\langle v(t)\rangle &= \dfrac{F}{m}\Delta t = \gamma F}
\end{align}$$
Where $\gamma$ is the mobility.


### What is Temperature?
Zeroth law of Thermodynamics:
Two physical systems in *thermal equilibrium* will have the same temperature.
To better understand it, equilibrium statistical mechanics is necessary.
### Ensemble
A collection of systems instead of individual ones. It's much easier to describe statistical properties of a lot of particles than to evaluate each particle for results.
### Entropy
Fundamental measure of information and disorder.

