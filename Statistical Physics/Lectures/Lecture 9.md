**Date: 2/13/2024**

### The Hard Sphere Gas
Improve the realism of the ideal gas by giving the particles a small radius.
If we make the potential energy infinite inside the radius of the hard spheres, the potential energy is simple (0 unless the spheres overlap).

We will calculate the pressure for a 2D gas:

### 2D Hard Sphere Gas
A 2D $L\times L$ box with hard walls contains a gas of $N$ distinguishable hard disks of radius $r \ll L$.
The area of each disk is $\pi r^2$. The system is dilute, where $N\pi r^2 \ll L^2$.

**What is the area allowed for the disk to access in the box?**
$$A(n) = (L-2r)^2 - (n-1)\pi (2r)^2$$
The total configuration space for $N$ particles, then:
$$\begin{align}
\Omega_\mathbb{Q} &= \prod_{n=1}^N A(n) = \prod_{n=1}^N\left((L-2r)^2 - (n-1)\pi (2r)^2\right) \\
&\approx \left[(L-2r)^2-\dfrac{Na}{2}\right]^N
\end{align}$$
The entropy of the system can be approximated as:
$$S_\mathbb{Q} = k_B \log\Omega_\mathbb{Q} \approx Nk_B$$
Pressure in 2D can be expressed as:








**What is the allowed momenta for the disk to access in the box?**


The total momentum space for $N$ particles, then





### 3D Hard Sphere Gas
A 3D $L\times L\times L$ box with hard walls contains a gas of $N$ distinguishable hard spheres of radius $r \ll L$.
The volume of each disk is $\dfrac{4}{3}\pi r^3$. The system is dilute, where $N\dfrac{4}{3}\pi r^3 \ll L^3$.

**What is the volume allowed for the sphere to access in the box?**
$$V(n) = (L-2r)^3 - \dfrac{4}{3}(n-1)\pi (2r)^3$$
The total configuration space for $N$ particles, then:
$$\Omega_\mathbb{Q} = \prod_{n=1}^N V(n) = \prod_{n=1}^N\left((L-2r)^3 - \dfrac{4}{3}(n-1)\pi (2r)^3\right)$$
**What is the allowed momenta for the disk to access in the box?**


The total momentum space for $N$ particles, then