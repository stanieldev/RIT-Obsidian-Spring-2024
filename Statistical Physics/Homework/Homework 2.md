Stanley Goodwin, 2/11/2024


2.6) $D=0.001\dfrac{\mathrm{m}^2}{\mathrm{s}}$, $\dfrac{\partial \rho}{\partial t} = D\dfrac{\partial^2 \rho}{\partial x^2}$

a) Suppose $\rho(x,0)=\cos(10x)$, find $\rho(x, 10\mathrm{s})$.
Let $\rho(x,t) = \tilde{\rho}(k,t)e^{ikx}$, then using the diffusion equations:
$$\begin{align}
\dfrac{\partial \rho}{\partial t} &= D\dfrac{\partial^2 \rho}{\partial x^2} \\
\dfrac{\partial \tilde{\rho}(k,t)}{\partial t}&= -Dk^2\tilde{\rho}(k,t) \\
\implies \Aboxed{\tilde{\rho}(k,t) &= \tilde{\rho}(k,0)e^{-Dk^2t}}
\end{align}$$
To find $\tilde{\rho}(k,0)$, we can use a Fourier transform:
$$\begin{align}
\tilde{\rho}(k,0)&=\int_{-\infty}^{\infty}\rho(x, 0)\cdot e^{-ikx}dx\\
&=\int_{-\infty}^{\infty}\cos(10x)\cdot e^{-ikx}dx\\
&= \pi\left[\delta(k-10)+\delta(k+10)\right]
\end{align}$$
Using an inverse Fourier transform, we can arrive at:
$$\begin{align}
\rho(x,t) &= \dfrac{1}{2\pi}\int_{-\infty}^{\infty}\tilde{\rho}(k,0)e^{-Dk^2t}e^{ikx}dk\\
&= \dfrac{1}{2}\int_{-\infty}^{\infty}\delta(k-10)e^{-Dk^2t}e^{ikx}dk+\dfrac{1}{2}\int_{-\infty}^{\infty}\delta(k+10)e^{-Dk^2t}e^{ikx}dk\\
&= \dfrac{1}{2}e^{-D(10)^2t}e^{i(10)x}+\dfrac{1}{2}e^{-D(-10)^2t}e^{i(-10)x}\\
&= e^{-100Dt}\dfrac{e^{i(10x)}+e^{-i(10x)}}{2}\\
\Aboxed{\rho(x,t) &= e^{-100Dt}\cos(10x)}
\end{align}$$
At $t=10\mathrm{s}$, and using $D=0.001\dfrac{\mathrm{m}^2}{\mathrm{s}}$:
$$\rho(x,t) = e^{-0.1t}\cos(10x) \implies \boxed{\rho(x,10\mathrm{s}) = e^{-1}\cos(10x)}$$

<br>




b) Suppose $\rho(x,-t_0)=\delta(x)$, find what time $t$ that reduces to a gaussian.
$$\rho(x,t) = \dfrac{1}{\sqrt{4\pi Dt}}e^{-\dfrac{x^2}{4Dt}} = \dfrac{1}{\sqrt{2\pi}}e^{-\dfrac{x^2}{2}}$$
$$\implies 4D(t-t_0)=2 \implies t=t_0+\dfrac{1}{2D}$$
Using the constant values from before:
$$\boxed{\Delta t = \dfrac{1}{2D} = 500\mathrm{s}}$$

<hr>



2.16) The diffusion constant can be density dependent; for example, proteins diffusing in a cell membrane are so crowded they can get in the way of one another. What should the diffusion equation be for a conserved particle density $\rho$ diffusing with diffusion constant $D(\rho)$?

Conserved Density: $\dfrac{\partial\rho}{\partial t} = -\dfrac{\partial J}{\partial x}$.
Diffusion Condition: $J = -D(\rho)\dfrac{\partial\rho}{\partial x}$.
Assuming there is no external driving force, we have:
$$\begin{align}
\dfrac{\partial\rho}{\partial t} &= -\dfrac{\partial J}{\partial x} = -\dfrac{\partial}{\partial x}\left(-D(\rho)\dfrac{\partial\rho}{\partial x}\right) \\
&= D(\rho)\dfrac{\partial^2\rho}{\partial x^2}+\dfrac{\partial D(\rho)}{\partial x}\dfrac{\partial\rho}{\partial x}
\end{align}$$
We can then write it as the following equation of diffusion:
$$\boxed{\dfrac{\partial\rho}{\partial t} = \dfrac{\partial D(\rho)}{\partial x}\dfrac{\partial\rho}{\partial x} + D(\rho)\dfrac{\partial^2\rho}{\partial x^2}}$$
Alternatively, we can write it in terms of density differentials:
$$\boxed{\dfrac{\partial\rho}{\partial t} = \dfrac{\partial D(\rho)}{\partial \rho}\left(\dfrac{\partial\rho}{\partial x}\right)^2 + D(\rho)\dfrac{\partial^2\rho}{\partial x^2}}$$
In this case I assumed it's 1D, but this can be written in 3D like:
$$\boxed{\dfrac{\partial\rho}{\partial t} = \nabla D(\rho)\cdot \nabla\rho + D(\rho)\nabla^2\rho}$$


<hr>





2.19) $T=1\mathrm{s}$, $V=20\dfrac{\mu\mathrm{m}}{\mathrm{s}}$, $\tau=0.1\mathrm{s}$.

a) What's the value of $\langle\vec{r}^2(t)\rangle$? Let $t = N(T+\tau)$.
$$\begin{align}
\langle\vec{r}^2(t)\rangle &= NL^2 \\
&= \left(\dfrac{t}{T+\tau}\right)\left(V\cdot T\right)^2\\
\Aboxed{\langle\vec{r}^2(t)\rangle &= \left(\dfrac{V^2\cdot T^2}{T+\tau}\right)t}
\end{align}$$
Writing in terms of a diffusion constant:
$$\begin{align}
\langle\vec{r}^2(t)\rangle&= 2nDt = 6Dt\\
\implies \Aboxed{D &= \dfrac{1}{6}\left(\dfrac{V^2\cdot T^2}{T+\tau}\right)}
\end{align}$$

<br>
b) Suppose at a radius $a$, all food is eaten with 100% efficiency.
Solve the Diffusion equation for the density of food molecules.


Note: $\nabla^2\rho = \dfrac{1}{r^2}\dfrac{\partial}{\partial r}\left(r^2\dfrac{\partial\rho}{\partial r}\right)$ for spherical symmetry.
We can express the diffusion constant in 3D with the following equation:
$$\begin{align}
\dfrac{\partial\rho}{\partial t} &= D\nabla^2\rho = \dfrac{D}{r^2}\dfrac{\partial}{\partial r}\left(r^2\dfrac{\partial\rho}{\partial r}\right) \\
&= \dfrac{2D}{r}\dfrac{\partial\rho}{\partial r}+D\dfrac{\partial^2\rho}{\partial r^2}
\end{align}$$
At equilibrium, there will be no chance in density over time, meaning:
$$\begin{align}
0 &= \dfrac{2D}{r}\dfrac{\partial\rho}{\partial r}+D\dfrac{\partial^2\rho}{\partial r^2} \\
\implies \rho(r) &= \dfrac{A}{r} + C
\end{align}$$
Using the initial conditions that $\rho(a) = 0$ and $\rho(\infty)=N$, we get that:
$$\rho(r) = N\left(1-\dfrac{a}{r}\right)$$
The net flow through the spherical surface with radius $a$ with diffusion $D$, therefore:
$$\begin{align}
D\cdot 4\pi a^2 \left.\dfrac{d\rho(r)}{dr}\right|_{r=a} &= 4\pi a^2N\left(\dfrac{a}{a^2}\right)D\\
&= \boxed{4\pi aND}
\end{align}$$







<hr>

<br>


2.20) Boids simulation!

I used Ben Eater's simulation found here: https://eater.net/boids

Well Captured:
 - The general shape of flocking patterns.
 - Complex behavior based on simple rules.

Not-so-well Captured:
 - Individual birds.
 - Long-Distance communication (sounds / displays).
 - Missing environmental things like weather, obstacles, and food.



b) Flocking Dynamics.
Describe the dynamics. Does the flock end up going largely in a single direction?
 - Since objects are pulled to the "center of mass" and velocity thereof, all paths converge to a similar heading, and so will stick together for the most part. In every time I've run it, it tends to go in a radial rotation direction.

If so, is the direction of motion the same for different simulation runs?
 - No, it is dependent on the initial conditions.
 - The initial direction is effectively random, but it's a feedback loop to stay that direction.

Identify the slow particles in the animation. How do the slow particles forming this bump differ from the rest?
 - Most of them stay outside the center mass of red-particles.

Increase the noise strength. Estimate the noise level at which the particles stop moving collectively.
 - At about 4 (slowly rising from 0), the motion is mostly just random shuffling without a collective mass movement. Interestingly, starting with 10 and reducing from there, I could get to about 2 before they start having coherent rotational movement.