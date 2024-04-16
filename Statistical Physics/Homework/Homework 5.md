<hr>
Stanley Goodwin, 4/15/2024


### Question 1
Relationships between response functions and fluctuations. Some of this has been
discussed in class. All symbols below have meanings used in class. Show the following.
$$\begin{align}
&(a)&\dfrac{\partial\langle E\rangle}{\partial T} = \dfrac{1}{k_BT^2}\left(\left\langle E^2\right\rangle-\left\langle E\right\rangle^2\right)\\
&(b)&\dfrac{\partial\langle N\rangle}{\partial \mu} = \dfrac{1}{k_BT}\left(\left\langle N^2\right\rangle-\left\langle N\right\rangle^2\right)\\
&(c)&\dfrac{\partial\langle M\rangle}{\partial H} = \dfrac{1}{k_BT}\left(\left\langle M^2\right\rangle-\left\langle M\right\rangle^2\right)\\
\end{align}$$
a) $Z=\sum_se^{-\tfrac{E_s}{k_BT}}$
$$\begin{align}
\langle E\rangle Z &= \sum_sE_se^{-\tfrac{E_s}{k_BT}}\\
\dfrac{\partial\left(\langle E\rangle Z\right)}{\partial T} &= \dfrac{\partial}{\partial T}\sum_sE_se^{-\tfrac{E_s}{k_BT}}\\
\dfrac{\partial\langle E\rangle}{\partial T}Z + \langle E\rangle\dfrac{\partial Z}{\partial T}&=\dfrac{\partial}{\partial T}\sum_sE_se^{-\tfrac{E_s}{k_BT}}\\
\dfrac{\partial\langle E\rangle}{\partial T}Z + \left(\dfrac{-1}{k_BT^2}\right)\langle E\rangle\sum_sE_ne^{-\tfrac{E_s}{k_BT}}&= \left(\dfrac{-1}{k_BT^2}\right)\sum_sE_n^2e^{-\tfrac{E_s}{k_BT}}\\
\dfrac{\partial\langle E\rangle}{\partial T} + \left(\dfrac{-1}{k_BT^2}\right)\langle E\rangle\dfrac{\sum_sE_ne^{-\tfrac{E_s}{k_BT}}}{Z} &= \left(\dfrac{-1}{k_BT^2}\right)\dfrac{\sum_sE_n^2e^{-\tfrac{E_s}{k_BT}}}{Z}\\
\dfrac{\partial\langle E\rangle}{\partial T} + \left(\dfrac{-1}{k_BT^2}\right)\langle E\rangle\langle E\rangle &= \left(\dfrac{-1}{k_BT^2}\right)\langle E^2\rangle\\
\Aboxed{\dfrac{\partial\langle E\rangle}{\partial T} &= \dfrac{1}{k_BT^2}\left(\langle E^2\rangle - \langle E\rangle^2\right)} 
\end{align}$$

b) $Z=\sum_se^{-\tfrac{E_s-\mu N_s}{k_BT}}$
$$\begin{align}
\langle N\rangle Z&= \sum_sN_se^{-\tfrac{E_s-\mu N_s}{k_BT}}\\
\dfrac{\partial(\langle N\rangle Z)}{\partial\mu} &= \dfrac{\partial}{\partial\mu}\sum_sN_se^{-\tfrac{E_s-\mu N_s}{k_BT}}\\
\dfrac{\partial\langle N\rangle}{\partial\mu}Z+\langle N\rangle\dfrac{\partial}{\partial\mu}\sum_se^{-\tfrac{E_s-\mu N_s}{k_BT}} &= \sum_s\dfrac{\partial}{\partial\mu}N_se^{-\tfrac{E_s-\mu N_s}{k_BT}}\\
\dfrac{\partial\langle N\rangle}{\partial\mu}Z+\dfrac{-1}{k_bT}\langle N\rangle\sum_sN_se^{-\tfrac{E_s-\mu N_s}{k_BT}} &= \dfrac{-1}{k_bT}\sum_sN_s^2e^{-\tfrac{E_s-\mu N_s}{k_BT}}\\
\dfrac{\partial\langle N\rangle}{\partial\mu} &= \dfrac{1}{k_bT}\left(\langle N\rangle\dfrac{\sum_sN_se^{-\tfrac{E_s-\mu N_s}{k_BT}}}{Z} - \dfrac{\sum_sN_s^2e^{-\tfrac{E_s-\mu N_s}{k_BT}}}{Z}\right)\\
\Aboxed{\dfrac{\partial\langle N\rangle}{\partial\mu} &= \dfrac{1}{k_bT}\left(\langle N\rangle^2 -\langle N^2\rangle\right)}
\end{align}$$
Not sure why the answer is off by a negative, but the calculation seems correct.

c) $Z=\sum_se^{-\tfrac{\hat{H}}{k_BT}}$
$$\begin{align}
\langle M\rangle Z &= \sum_sMe^{-\tfrac{\hat{H}}{k_BT}}\\
\dfrac{\partial (\langle M\rangle Z)}{\partial H} &= \dfrac{\partial}{\partial H}\sum_sMe^{-\tfrac{\hat{H}}{k_BT}}\\
\dfrac{\partial\langle M\rangle}{\partial H}Z + \langle M\rangle\dfrac{\partial Z}{\partial H} &= \sum_sM\dfrac{\partial}{\partial H}e^{-\tfrac{\hat{H}}{k_BT}}\\
\dfrac{\partial\langle M\rangle}{\partial H}Z + \langle M\rangle\dfrac{1}{k_BT}\sum_sMe^{-\tfrac{\hat{H}}{k_BT}} &= \dfrac{1}{k_BT}\sum_sM^2e^{-\tfrac{\hat{H}}{k_BT}}\\
\dfrac{\partial\langle M\rangle}{\partial H} &= \dfrac{1}{k_BT}\left(\dfrac{\sum_sM^2e^{-\tfrac{\hat{H}}{k_BT}}}{Z} - \langle M\rangle\dfrac{\sum_sMe^{-\tfrac{\hat{H}}{k_BT}}}{Z}\right)\\
\Aboxed{\dfrac{\partial\langle M\rangle}{\partial H} &= \dfrac{1}{k_BT}\left(\langle M^2\rangle - \langle M\rangle^2\right)}
\end{align}$$



<hr>

### Question 2 : Two-state system
Consider the statistical mechanics of a tiny object with only two discrete states:
One of energy $E_1$ and the other of higher energy $E_2 > E_1$.

a.1) Find the ratio of the equilibrium probabilities $\rho_2/\rho_1$ to find our system in the two states, when weakly coupled to a heat bath of temperature T. 
$$\begin{align}
\Aboxed{\dfrac{\rho_2}{\rho_1} &= e^{\tfrac{E_1-E_2}{k_BT}}}
\end{align}$$

a.2) What is the limiting probability as T → ∞?
$$\lim_{T\rightarrow\infty}\dfrac{\rho_2}{\rho_1} = \lim_{T\rightarrow\infty}e^{\tfrac{E_1-E_2}{k_BT}} = e^0 = \boxed{1}$$

a.3) As T → 0? 
$$\lim_{T\rightarrow\infty}\dfrac{\rho_2}{\rho_1} = \lim_{T\rightarrow\infty}e^{\tfrac{E_1-E_2}{k_BT}} = \left\{\begin{array}{c}+\infty, E_1 > E_2\\0, E_2 > E_1\end{array}\right.$$
Since $E_2 > E_1$, the limit approaches $\boxed{0}$.



b.1) Use the normalization of the probability distribution (the system must be in one or the other state) to find $\rho_1$ and $\rho_2$ separately.
$$\begin{align}
Z&= e^{-\tfrac{E_1}{k_BT}}+e^{-\tfrac{E_2}{k_BT}}\\
\rho_1&=\dfrac{e^{-\tfrac{E_1}{k_BT}}}{e^{-\tfrac{E_1}{k_BT}}+e^{-\tfrac{E_2}{k_BT}}}\\
\rho_2&=\dfrac{e^{-\tfrac{E_2}{k_BT}}}{e^{-\tfrac{E_1}{k_BT}}+e^{-\tfrac{E_2}{k_BT}}}
\end{align}$$

b.2) What is the average value of the energy $E$?
$$\begin{align}
\langle E\rangle = \dfrac{E_1e^{-\tfrac{E_1}{k_BT}}+E_2e^{-\tfrac{E_2}{k_BT}}}{e^{-\tfrac{E_1}{k_BT}}+e^{-\tfrac{E_2}{k_BT}}}
\end{align}$$



<hr>

### Question 3 : Gibbs-Duhem
As a state function, $E$ is supposed to depend only on $S$, $V$, and $N$ . 
But equation 6.75 seems to show explicit dependence on T , P , and μ as well;
Another answer is to consider a small shift of all six variables. How can this be?

We know that $dE=TdS−PdV+\mu dN$ , but if we shift all six variables in
Euler’s equation we get $dE=TdS−PdV+\mu dN+SdT−VdP+Nd\mu$. 
This implies the *Gibbs–Duhem relation*:
$$0=SdT-VdP+Nd\mu$$
This relation implies that the intensive variables $T$, $P$, and $\mu$ are not all independent; 
the change in $\mu$ is determined given a small change in $T$ and $P$.

a) Write μ as a suitable derivative of the Gibbs free energy $G(T, P, N)$.
This makes $\mu$ a function of the three variables $T$, $P$, and $N$. 
The Gibbs–Duhem relation says it must be independent of $N$.

$$\begin{align}
dU &= -PdV+TdS+\mu dN\\
dG &= dU + PdV + VdP -TdS-SdT\\
&= VdP - SdT + \mu dN\\
dG &= \dfrac{\partial G}{\partial P}dP - \dfrac{\partial G}{\partial T}dT + \dfrac{\partial G}{\partial N}dN\\
\Aboxed{\mu &= \dfrac{\partial G}{\partial N}}
\end{align}$$





<hr>

### Question 4 (pg.165)
Problem 6.10 (a) from the book.

Consider the phase diagram in Fig. 6.14. Along an equilibrium phase boundary, the temperatures, pressures, and chemical potentials of the two phases must agree; 
otherwise a flat interface between the two phases would transmit heat, shift sideways, or leak particles, respectively (violating the assumption of equilibrium).


(a) Apply the Gibbs–Duhem relation 6.77 to both
phases, for a small shift by ∆T along the phase
boundary. Let s1, v1, s2, and v2 be the molecu-
lar entropies and volumes (s = S/N , v = V /N
for each phase); derive the Clausius–Clapeyron
equation for the slope of the coexistence line on
the phase diagram.
$$\dfrac{dP}{dT}=\dfrac{s_1-s_2}{v_1-v_2}$$
$$0=SdT-VdP+Nd\mu$$

>Along an equilibrium phase boundary, the temperatures, pressures, and **chemical potentials** of the two phases must agree.

This means that $d\mu = 0$, so we can safely ignore it.
Therefore, we get the following equation:
$$VdP=SdT \implies \dfrac{dP}{dT}=\dfrac{S}{V}$$
Since the number of particles is the same, we can do a nice trick:
$$\boxed{\dfrac{dP}{dT}=\dfrac{\Delta S / N}{\Delta V / N}=\dfrac{\Delta s}{\Delta v} = \dfrac{s_a-s_b}{v_a-v_b}}$$




