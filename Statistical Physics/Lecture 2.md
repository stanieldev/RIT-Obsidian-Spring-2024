**Date: 1/18/2024**

### Stirling's Approximation
#### Formulation
Start off with $N!$ using exponential and log properties:
$$\begin{align}
N! &= e^{\log N!} = e^{\log(1\times2\times3\times\dots\times N)} = e^{\log(1)+\log(2)+\log(3)+\dots+\log(N)}\\
N! &= e^{\sum_{n=1}^N \log n}
\end{align}$$
Taking the natural log of both sides and using approximate integrals:
$$\begin{align}
\log(N!) &= \sum_{n=1}^N \log n \approx \int_{0}^N dx\log x = N\log N - N\\
\end{align}$$
A more precise approximation uses $\Gamma(x)$, leading to (for $N\gg 1$):
$$\begin{aligned}
\Aboxed{\log(N!) &\approx N\log N - N + \dfrac{1}{2}\log(2\pi N)} \\
\Aboxed{\log(N!) &\approx N^Ne^{-N}\sqrt{2\pi N}}
\end{aligned}$$
#### Examples of Approximation
| $n$ | $\log(n!)$ | $n\log n-n+\dfrac{1}{2}\log(2\pi n)$ | $n\log n-n+\dfrac{1}{2}\log(2\pi n)$ |
| ---- | ---- | ---- | ---- |
| 1 | $0$ | $0.0810615\dots$ | $-1$ |
| 2 | $0.693147\dots$ | $0.651806\dots$ | $-0.613706\dots$ |
| 4 | $3.17805\dots$ | $3.15726\dots$ | $1.54518\dots$ |
| 50 | $148.477\dots$ | $145.60\dots$ | $148.476\dots$ |
| $6.02\cdot10^{23}$ | $3.2\dots\ \cdot10^{25}$ | $3.2\dots\ \cdot10^{25}$ | $3.2\dots\ \cdot10^{25}$ |
As the value of $n$ get's larger, the full approximation becomes extremely close.

### Probability of Discrete Events
#### Example of Discrete Events
*Suppose you flip 20 fair coins.*
1. How many possible outcomes (microstates) are there?
$$\Omega = 2^{20} \mathrm{\ Outcomes}$$
2. What is the probability of getting at singular outcome?
$$p=\dfrac{1}{\Omega} \approx 10^{-6}$$
3. What is the probability of 12 heads, 8 tails?
$$p(12H)=\dfrac{_{20}C_{12}}{\Omega} = \dfrac{\dfrac{20!}{12!\cdot 8!}}{2^{20}} = \dfrac{125970}{1048576} \approx 12.01\% $$

### Probability Distributions of Continuous Variables
A function that describes the probability density of a set of variables.
The integral of the distribution must be $1$ ($100\%$).
#### Types of Distributions
There are 3 types usually encountered in physics:
1. Uniform distribution (Table distribution)
	1. $\rho(x)=\begin{cases}1,&0\le x\lt 1\\0,&x\lt0,x \ge 1\end{cases}$
2. Normal distribution (Gaussian distribution)
	1. $\rho(x)=\dfrac{1}{\sigma\sqrt{2\pi}}e^{-\tfrac{x^2}{2\sigma^2}}$
3. Exponential distribution
	1. $\rho(x)=\dfrac{1}{\tau}e^{-\tfrac{t}{\tau}}$
#### Examples of Distributions
1. Probability that a Uniform Distribution will fall in $x\in(0.70, 0.75)$
$$\int_{0.70}^{0.75}dx \ \rho(x) = (0.75-0.70) = \boxed{5\%}$$
2. That your score on an exam (Normal Distribution) has $x\in(2\sigma, \infty)$
$$\int_{\mu+2\sigma}^{\infty}dx \ \rho(x) = \int_{2}^{\infty}dz \ \rho(z) \approx 2.3\%$$


