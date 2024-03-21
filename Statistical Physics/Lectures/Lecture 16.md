**Date: 3/19/2024**


### Thermodynamic Potentials and Free Energy
| Potential             | Relation          |
| --------------------- | ----------------- |
| Enthalpy              | $H=U+PV$          |
| Gibb Free Energy      | $G=U+PV-TS$       |
| Helmholtz Free Energy | $F=U-TS$          |
| Grand Free Energy     | $\Phi=U-TS-\mu N$ |


Microcanonical Ensemble:
 - Describes an isolated system.
 - Number of particles, Volume, and Energy is constant.

Canonical Ensemble:
 - Describes a closed system.
 - Number of particles and Volume is constant.
 - Energy can be exchanged with environment.

Grand Canonical Ensemble:
 - Describes an open system.
 - Volume is constant.
 - Energy and particles can be exchanged with environment.


### Microcanonical Ensemble
A system which is completely isolated from its surroundings has constant energy, volume, and number of particles.
 - There is no heat or work input to the system.
 - The internal energy $U$ is fixed.

Entropy: $S=k_B\log\Omega$
Temperature: $\dfrac{1}{T}=\dfrac{\partial S}{\partial U}$
Pressure: $\dfrac{P}{T}=\dfrac{\partial S}{\partial V}$


### Canonical Ensemble
A system that can exchange energy with a bath, but not particle number and volume.

Equilibrium Distribution: $\rho(s)=\dfrac{1}{Z}e^{-\tfrac{E_s}{k_BT}}, \ \ \ Z=\displaystyle\sum_se^{-\tfrac{E_s}{k_BT}}$
$E_s = 0$ is defined for the ground-state energy.

Helmholtz Free Energy: $F(T,V,N) = U - TS = -k_BT\log Z$
Entropy: $S=-\dfrac{\partial F}{\partial T}$
Pressure: $P=-\dfrac{\partial F}{\partial V}$
Chemical Potential: $\mu=\dfrac{\partial F}{\partial N}$
Energy: $\langle E\rangle = -\dfrac{1}{Z}\dfrac{\partial Z}{\partial \beta}$
Total Energy: $U=N\langle E\rangle$

Note : What if classical systems used entropy instead of energy like microcanonical?


### Grand Canonical Ensembles
Oh god oh fuck.

Equilibrium Distribution: $\rho(s)=\dfrac{1}{Z}e^{-\tfrac{E_s-\mu N_s}{k_BT}}, \ \ \ Z=\displaystyle\sum_se^{-\tfrac{E_s-\mu N_s}{k_BT}}$

Grand Free Energy: $\Phi(T,V,N) = U - TS -\mu N$
