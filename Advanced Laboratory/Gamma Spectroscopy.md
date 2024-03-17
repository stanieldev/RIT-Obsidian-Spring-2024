Rewriting E' in terms of the rest of the variables.
$$\begin{align}
\dfrac{1}{E'}-\dfrac{1}{E} &= \dfrac{1}{m_ec^2}\left(1-\cos\theta\right)\\
\implies \dfrac{1}{E'} &= \dfrac{1}{m_ec^2}\left(1-\cos\theta\right)+\dfrac{1}{E}\\
\implies \dfrac{1}{E'} &= \dfrac{E}{Em_ec^2}\left(1-\cos\theta\right)+\dfrac{m_ec^2}{Em_ec^2}\\
\implies \dfrac{1}{E'} &= \dfrac{E\left(1-\cos\theta\right)+m_ec^2}{Em_ec^2}\\
\implies \Aboxed{E' &= E\cdot\dfrac{m_ec^2}{E\left(1-\cos\theta\right)+m_ec^2}}\\
\end{align}$$
The kinetic energy of the electron can then be expressed as:
$$\begin{align}
E-E' &= E-E\cdot\dfrac{m_ec^2}{E\left(1-\cos\theta\right)+m_ec^2}\\
&= E\left(1-\dfrac{m_ec^2}{E\left(1-\cos\theta\right)+m_ec^2}\right)\\
&= E\left(\dfrac{E\left(1-\cos\theta\right)+m_ec^2-m_ec^2}{E\left(1-\cos\theta\right)+m_ec^2}\right)\\
\mathrm{KE}_{e}&= E\left(\dfrac{E\left(1-\cos\theta\right)}{E\left(1-\cos\theta\right)+m_ec^2}\right)\\
\Aboxed{\mathrm{KE}_{e}&= E\left(1+\dfrac{m_ec^2}{E\left(1-\cos\theta\right)}\right)^{-1}}
\end{align}$$
To find the maximum kinetic energy, we have to find the critical point:
$$\begin{align}
\dfrac{d\mathrm{KE}_{e}}{d\theta}&= \left(E\left(1+\dfrac{m_ec^2}{E\left(1-\cos\theta\right)}\right)^{-1}\right)\\
&= -E\left(1+\dfrac{m_ec^2}{E\left(1-\cos\theta\right)}\right)^{-2}\left(\dfrac{m_ec^2}{E}\right)(-1)\left(1-\cos\theta\right)^{-2}\sin\theta\\
0 &= m_ec^2\left(1+\dfrac{m_ec^2}{E\left(1-\cos\theta\right)}\right)^{-2}\left(1-\cos\theta\right)^{-2}\sin\theta\\
\Aboxed{\theta&=n\pi, n\in\mathbb{Z}}
\end{align}$$
Taking a look at the second derivative, and realizing angles loop after $2\pi$, then the only solution to maximize the electron kinetic energy is $\boxed{\theta = \pi}$.

The equation for maximum kinetic energy from Compton scattering can be written as:
$$\begin{align}
\Aboxed{\mathrm{KE}_{\mathrm{max}}&= E\left(1+\dfrac{m_ec^2}{2E}\right)^{-1}}
\end{align}$$
For a photon energy of $E = 662\ \mathrm{keV}$:
$$\begin{align}
\mathrm{KE}_{\mathrm{max}}&= E\left(1+\dfrac{m_ec^2}{2E}\right)^{-1}\\
&= 662\ \mathrm{keV} \cdot\left(1+\dfrac{511\ \mathrm{keV}}{2\cdot 662\ \mathrm{keV}}\right)^{-1}\\
\Aboxed{\mathrm{KE}_{\mathrm{max}} &= 477.65\ \mathrm{keV}}
\end{align}$$
Using the maximum kinetic energy angle, the photon's final energy comes to be:
$$\begin{align}
\dfrac{1}{E'}-\dfrac{1}{E} &= \dfrac{1}{m_ec^2}\left(1-\cos\theta\right)\\
\implies \dfrac{1}{E'} &= \dfrac{1}{511\ \mathrm{keV}}\left(1-\cos\pi\right)+\dfrac{1}{662\ \mathrm{keV}}\\
\implies \Aboxed{E'=184.35\ \mathrm{keV}}
\end{align}$$
Using this kinetic energy and the initial photon energy, the scattered photon has energy:
$$\begin{align}
E'&=E-\mathrm{KE}_{\mathrm{max}}\\
\Aboxed{E'&=184.35\ \mathrm{keV}}
\end{align}$$
It's expected these are the same if I did my math correctly.



$$G(x;A,\mu,\sigma) = \dfrac{1}{\sigma\sqrt{2\pi}}\cdot e^{-\dfrac{(x-\mu)^2}{2\sigma^2}}$$
$x$ is the domain of the function.
$a_1=A$ is the maximum probability density, given at $x=\mu$.
$a_2=\mu$ is the mean, median, and mode, of the function.
$a_3=\sigma$ is the standard deviation, represented as $\sqrt{\mathrm{Variance}}$.

$$\mathrm{FWHM}=\sigma\sqrt{8\ln2}$$



$$\sigma^2\rightarrow\dfrac{\sigma^2}{\tfrac{120}{20}}=\dfrac{\sigma^2}{6} \implies \sigma\rightarrow \dfrac{\sigma}{\sqrt{6}}$$
$$\mathrm{SE}=\dfrac{s}{\sqrt{5}}=\dfrac{\sigma}{\sqrt{30}}$$

| Method            | $\mu$ (V)       | $\mathrm{FWHM}$ (V) |
| ----------------- | --------------- | ------------------- |
| Eyeball           | $6.825\pm0.075$ | $0.9\pm0.4$         |
| Gaussian          | $6.826\pm0.007$ | $1.033\pm0.018$     |
| Gaussian + Linear | $6.817\pm0.009$ | $0.951\pm0.030$     |
Table 1: Tabulation of different methods for finding
	  the photopeak characteristics.




$$E = \left(\dfrac{0.662\ \mathrm{MeV}}{6.826\ \mathrm{V}}\right)V$$





## MCA Section
$$\begin{align}
\dfrac{1}{E'}-\dfrac{1}{E} &= \dfrac{1}{m_ec^2}\left(1-\cos\theta\right)\\
\dfrac{1}{E'}&= \dfrac{1}{m_ec^2}\left(1-\cos\pi\right)+\dfrac{1}{E}\\
\dfrac{1}{E'}&= \dfrac{2}{m_ec^2}+\dfrac{1}{E}\\
\implies \Aboxed{E'&= \left(\dfrac{2}{m_ec^2}+\dfrac{1}{E}\right)^{-1}}
\end{align}$$

$$\begin{align}
E'_\mathrm{min}&= \left(\dfrac{2}{m_ec^2}+\dfrac{1}{E}\right)^{-1}\\
&= \left(\dfrac{2}{m_ec^2}+\dfrac{1}{E}\right)^{-1}\\
&= \left(\dfrac{2}{511\ \mathrm{keV}}+\dfrac{1}{662\ \mathrm{keV}}\right)^{-1}\\
\Aboxed{E'_\mathrm{min}&= 184.35\ \mathrm{keV}}
\end{align}$$

$$\begin{align}
\lim_{E\rightarrow\infty}E'_\mathrm{min}&= \lim_{E\rightarrow\infty}\left(\dfrac{2}{m_ec^2}+\dfrac{1}{E}\right)^{-1}\\
&= \left(\dfrac{2}{m_ec^2}\right)^{-1}\\
\Aboxed{E'_\mathrm{min}&= \dfrac{m_ec^2}{2}}
\end{align}$$

$$\begin{align}
E'_\mathrm{min}&= \dfrac{m_ec^2}{2}\\
E'_\mathrm{min}&= \dfrac{511\ \mathrm{keV}}{2}\\
\Aboxed{E'_\mathrm{min}&= 255.5\ \mathrm{keV}}
\end{align}$$



| Source              | $E$                     | $E'$                   | $\mathrm{KE}_\mathrm{max}$  |
| ------------------- | ----------------------- | ---------------------- | --------------------------- |
| $^{137}\mathrm{Cs}$ | $\ \ 662\ \mathrm{keV}$ | $184.35\ \mathrm{keV}$ | $\ \ 447.65\ \mathrm{keV}$  |
| $^{54}\mathrm{Mn}$  | $\ \ 835\ \mathrm{keV}$ | $195.64\ \mathrm{keV}$ | $\ \ 639.36\ \mathrm{keV}$  |
| $^{22}\mathrm{Na}$  | $\ \ 511\ \mathrm{keV}$ | $170.33\ \mathrm{keV}$ | $\ \ 340.67\ \mathrm{keV}$  |
| -                   | $1277\ \mathrm{keV}$    | $212.90\ \mathrm{keV}$ | $\ \ 1064.10\ \mathrm{keV}$ |
| $^{60}\mathrm{Co}$  | $1172\ \mathrm{keV}$    | $209.77\ \mathrm{keV}$ | $\ \ 962.23\ \mathrm{keV}$  |
| -                   | $1333\ \mathrm{keV}$    | $214.40\ \mathrm{keV}$ | $1118.60\ \mathrm{keV}$     |
Table 2: Photopeak, Backscattering, and Compton Edge Energies





| Source              | $E$                     | $E'$                   | $\mathrm{KE}_\mathrm{max}$  |
| ------------------- | ----------------------- | ---------------------- | --------------------------- |
| $^{137}\mathrm{Cs}$ | $\ \ 662\ \mathrm{keV}$ | $184.35\ \mathrm{keV}$ | $\ \ 447.65\ \mathrm{keV}$  |
| $^{54}\mathrm{Mn}$  | $\ \ 835\ \mathrm{keV}$ | $195.64\ \mathrm{keV}$ | $\ \ 639.36\ \mathrm{keV}$  |
| $^{22}\mathrm{Na}$  | $\ \ 511\ \mathrm{keV}$ | $170.33\ \mathrm{keV}$ | $\ \ 340.67\ \mathrm{keV}$  |
| -                   | $1277\ \mathrm{keV}$    | $212.90\ \mathrm{keV}$ | $\ \ 1064.10\ \mathrm{keV}$ |
| $^{60}\mathrm{Co}$  | $1172\ \mathrm{keV}$    | $209.77\ \mathrm{keV}$ | $\ \ 962.23\ \mathrm{keV}$  |
| -                   | $1333\ \mathrm{keV}$    | $214.40\ \mathrm{keV}$ | $1118.60\ \mathrm{keV}$     |
