**Stanley Goodwin, 3/21/2024**

<hr>

### Problem 5.2
Can we burn information as fuel?

a) *Assuming the gas expands at a constant temperature $T$, how much work $\int P \ \mathrm{d}V$ is done by the atom as the piston retracts?*

$\Delta V = 2V - V \implies W = PV$
$\Delta E = -PV = -k_B T$   (loss by tape, gain by engine)

For each bit, $W = k_B T$ is done onto the piston.



b) *Give a sequence of partition insertion, partition removal, and adiabatic side-wall motions that will reversibly convert a bit-zero into a bit-one, with no next work done on the system.*

1) Top piston moves up.
2) Bottom piston moves up.
3) Partition added at the bottom piston.
4) Move bottom piston back down.

The net energy between having each piston move in sequence or in parallel is identical.
It is identical to the process given in Fig. 5.12 in time-reverse. It is a reversible process.



c) *Suppose the atom location in the n-th box is initially known. What is the change in entropy, if the partition is removed and the available volume doubles? Give both thermodynamic entropy and informational entropy.*

$\Delta S = k_B \ln \dfrac{2V}{V} = k_B \ln2$
$\Delta S = k_B \ln \dfrac{2V}{V} = \log_22 = 1$

The change in thermodynamic entropy is $+k_B \ln2$, and is $+1$ bit of information entropy.



d) *After the bit has been burned, is the demon in a known state? What is its entropy? How much energy would it take to return the demon to the original state, and temperature $T$? Is the second law violated?*

After a bit has been burned, there is no known state, based on the definitions presented earlier.
It is identical to the state in "Forgetting a Bit." Is it not determined.

The entropy of the new state is $+1$ bit of informational entropy.
It would require as much energy to return the state back pre-burning, so $W = k_B T$.

The second law wouldn't be violated, since any operation would yield as much entropy as before at worst, assuming 100% efficiency, but this is not the case for an isolated system.


<hr>


### Problem 5.10
Initial problem givens:
$$S = -k_B \int_{-\infty}^\infty \rho(x)\log\rho(x)\ \mathrm{d}x, \ \ \ \dfrac{\partial\rho(x,t)}{\partial t} = D\dfrac{\partial^2\rho(x,t)}{\partial x^2}$$
To differentiate with respect to time, we can do the following chain of calculus:
$$\begin{align}
\dfrac{dS}{dt} &= -k_B \dfrac{d}{dt}\left(\int_{-\infty}^\infty \rho(x,t)\log\rho(x,t)\ \mathrm{d}x\right)\\
&= -k_B \int_{-\infty}^\infty \dfrac{\partial}{\partial t}\left(\rho(x,t)\log\rho(x,t)\right)\ \mathrm{d}x \\
&= -k_B \int_{-\infty}^\infty \dfrac{\partial \rho(x,t)}{\partial t}\log\rho(x,t) + \rho(x,t)\dfrac{\partial \log\rho(x,t)}{\partial t}\ \mathrm{d}x \\
&= -k_B \int_{-\infty}^\infty \dfrac{\partial \rho(x,t)}{\partial t}\log\rho(x,t) + \rho(x,t)\dfrac{1}{\rho(x,t)}\dfrac{\partial \rho(x,t)}{\partial t}\ \mathrm{d}x \\
&= -k_B \int_{-\infty}^\infty \dfrac{\partial \rho(x,t)}{\partial t}\left(\log\rho(x,t) + 1\right)\ \mathrm{d}x
\end{align}$$
Substituting with the diffusion equation, we have:
$$\begin{align}
\dfrac{dS}{dt} &= -k_B D \int_{-\infty}^\infty \dfrac{\partial^2\rho(x,t)}{\partial x^2}\left(\log\rho(x,t) + 1\right)\ \mathrm{d}x \\
\end{align}$$
With integration by parts, we get that:
$$\begin{align}
\dfrac{dS}{dt} &= -k_B D \int_{-\infty}^\infty \dfrac{\partial^2\rho(x,t)}{\partial x^2}\left(\log\rho(x,t) + 1\right)\ \mathrm{d}x \\
&= -k_B D \left(\log\rho(x,t) + 1\right)\left.\dfrac{\partial\rho(x,t)}{\partial x}\right|_{-\infty}^\infty + k_B D \int_{-\infty}^\infty \dfrac{1}{\rho(x,t)}\left(\dfrac{\partial\rho(x,t)}{\partial x}\right)^2\ \mathrm{d}x \\
&= k_B D \int_{-\infty}^\infty \dfrac{1}{\rho(x,t)}\left(\dfrac{\partial\rho(x,t)}{\partial x}\right)^2\ \mathrm{d}x > 0\\
\Aboxed{\dfrac{dS}{dt} &> 0}
\end{align}$$


<hr>


### Problem 5.11
a) Is the residual entropy $\left(S_\mathrm{res} = S_l - \displaystyle\int\dfrac{1}{T}\dfrac{dQ}{dT}dT\right)$ experimentally larger on heating or on cooling?
$$S_\mathrm{res} = S_l - \displaystyle\int\dfrac{C(T)}{T}dT$$
Since it shifts the capacity toward higher temperatures, the integral values for the heating will have a smaller integral than the cooling.

With heat having a smaller integral, the $S_\mathrm{res}$ is larger for the heating process than the cooling process.
