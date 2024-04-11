<hr>

### Question 1
Relationships between response functions and fluctuations. Some of this has been
discussed in class. All symbols below have meanings used in class. Show the following.
$$\begin{align}
&(a)&\dfrac{\partial\langle E\rangle}{\partial T} = \dfrac{1}{k_BT^2}\left(\left\langle E^2\right\rangle-\left\langle E\right\rangle^2\right)\\
&(b)&\dfrac{\partial\langle N\rangle}{\partial \mu} = \dfrac{1}{k_BT}\left(\left\langle N^2\right\rangle-\left\langle N\right\rangle^2\right)\\
&(c)&\dfrac{\partial\langle M\rangle}{\partial H} = \dfrac{1}{k_BT}\left(\left\langle M^2\right\rangle-\left\langle M\right\rangle^2\right)\\
\end{align}$$
a)




b) 





c) 






<hr>

### Question 2 : Two-state system
Consider the statistical mechanics of a tiny object with only two discrete states:
One of energy $E_1$ and the other of higher energy $E_2 > E_1$.
Related formula: Boltzmann probability = Z(T ) exp(−E/kT ) ∝ exp(−E/kT ).

a.1) Find the ratio of the equilibrium probabilities $\rho_2/\rho_1$ to find our system in the two states, when weakly coupled to a heat bath of temperature T. 





a.2) What is the limiting probability as T → ∞?




a.3) As T → 0? 




b.1) Use the normalization of the probability distribution (the system must be in one or the other state) to find $\rho_1$ and $\rho_2$ separately.



b.2) What is the average value of the energy $E$?



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
the phase diagram

$$\dfrac{dP}{dT}=\dfrac{s_1-s_2}{v_1-v_2}$$






