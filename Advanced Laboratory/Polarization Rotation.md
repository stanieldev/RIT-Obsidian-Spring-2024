$$I = I_0 \cos(\theta)^2$$


$$I = I_0\cos(\theta-\phi)^2$$



$$\begin{align}
B&=\mu_0 NIL\\
&=\left(4\pi\cdot10^{-7}\dfrac{\mathrm{H}}{\mathrm{m}}\right) \left(10\mathrm{\ layers}\cdot140\ \dfrac{\mathrm{turns}}{\mathrm{layers}}\right) (3A) (0.15\mathrm{\ m})\\
\Aboxed{B&= 0.791\ \mathrm{mT}}
\end{align}$$

$$\begin{align}
L_\mathrm{wire} &= (2\pi R)\cdot N\\
&= \left(2\pi\ \dfrac{0.0174\mathrm{\ m}+0.0366\mathrm{\ m}}{4}\right) \left(10\mathrm{\ layers}\cdot140\ \dfrac{\mathrm{turns}}{\mathrm{layers}}\right)\\
\Aboxed{L_\mathrm{wire} &= 118.75\mathrm{\ m}}
\end{align}$$
$$\begin{align}
R_\mathrm{wire} &= \dfrac{\rho L}{A}\\
&= \dfrac{\left(1.7\cdot10^{-8}\mathrm{\ \Omega\ m}\right) (118.75\mathrm{\ m})}{\tfrac{\pi}{4}\left(1.024\cdot10^{-3}\mathrm{\ m}\right)^2}\\
\Aboxed{R_\mathrm{wire} &= 2.451\mathrm{\ \Omega}}
\end{align}$$


$\Delta\theta = BL\nu$
$B$ is the magnetic field.
$L$ is the length of the sample.
$\nu$ is the Verdet constant.


$$Z_L = j\omega L$$

$$\begin{align}
Z(\omega) &= R+R_L+j\omega L \\
&= 2\ohm + 2.5\ohm + j\omega \left(6\cdot10^{-3}\ \mathrm{H}\right)\\
\Aboxed{Z(\omega)&= 4.5\ohm + j\omega \left(6\cdot10^{-3}\ \mathrm{H}\right)}
\end{align}$$

$$\begin{align}
Z(1\ \mathrm{kHz})&= 4.5\ohm + j \left(1\cdot10^{3}\ \mathrm{Hz}\right)\left(6\cdot10^{-3}\ \mathrm{H}\right)\\
&= \left(4.5+6j\right)\ \ohm\\
|Z(1\ \mathrm{kHz})|&=\sqrt{10.5}\ \ohm\\
\Aboxed{V(1\ \mathrm{kHz}) &= \sqrt{10.5}\ \mathrm{V} \approx 3.24\ \mathrm{V}}
\end{align}$$

$$\begin{align}
Z(50\ \mathrm{kHz})&= 4.5\ohm + j \left(50\cdot10^{3}\ \mathrm{Hz}\right)\left(6\cdot10^{-3}\ \mathrm{H}\right)\\
&= \left(4.5+300j\right)\ \ohm\\
|Z(50\ \mathrm{kHz})|&=\sqrt{304.5}\ \ohm\\
\Aboxed{V(50\ \mathrm{kHz}) &= \sqrt{304.5}\ \mathrm{V} \approx 17.45\ \mathrm{V}}
\end{align}$$


$$\begin{align}
f&=\dfrac{1}{2\pi\sqrt{LC}}\\
&= \dfrac{1}{2\pi\sqrt{\left(6\ \mathrm{mH}\right)\left(1\ \mu\mathrm{F}\right)}}\\
\Aboxed{f&=2054.68\ \mathrm{Hz}}
\end{align}$$


$$I(\omega)=\dfrac{V_\mathrm{in}}{\sqrt{R^2 + \left(\omega L-\dfrac{1}{\omega C}\right)^2}}$$




$$\begin{align}
&f=\dfrac{1}{2\pi\sqrt{LC}} &\delta f=\dfrac{f}{2}\sqrt{\left(\dfrac{\delta L}{L}\right)^2+\left(\dfrac{\delta C}{C}\right)^2}
\end{align}$$

$$f=2089.46\pm 56.04\ \mathrm{Hz}$$


$$\begin{align}
Q&=\dfrac{1}{R}\sqrt{\dfrac{L}{C}}\\
&=\dfrac{1}{4.5\ \Omega}\sqrt{\dfrac{6\cdot10^{-3}\ \mathrm{H}}{1\cdot10^{-6}\ \mathrm{F}}}\\
&= 17.213
\end{align}$$
Calculate Theoretical



$$Q=\dfrac{1}{R}\sqrt{\dfrac{L}{C}}$$
Calculate after Fit
Compare Difference

$$\begin{align}
Q&=\dfrac{f_0}{\Delta f}\\
&= \dfrac{2089.5 \ \mathrm{Hz}}{\left(
2180.37-2002.33\right) \ \mathrm{Hz}}\\
\Aboxed{Q &= 11.736}
\end{align}$$
at half power, find value and compare to theory.







