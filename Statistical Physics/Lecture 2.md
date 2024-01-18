**Date: 1/18/2024**

#### Stirling's Approximation
$$\begin{align}
N! &\approx \left(\dfrac{N}{e}\right)^N \sqrt{2\pi N}\\
\log(N!)&\approx N\log N - N + \dfrac{1}{2}\log{(2\pi N)}
\end{align}$$
Or when $N \rightarrow \infty$ in this class:
$$\begin{align}
N! &\approx N^N e^{-N}\\
\log(N!)&\approx N\log N - N
\end{align}$$

NOTE: Make a upper and lower bound for better approximation.
#### Example of Stirling
a) Calculate $\log(n!)$ for $n=2,4,50$, and estimate the error for $6.03\cdot10^{23}$.
$n=2 \implies \log(2!) \approx 2\log2-2 = -0.6137$
$n=4 \implies \log(4!) \approx 4\log4-4 = +1.5452$
$n=50 \implies \log(50!) \approx 50\log50-50 = +145.60$
For $N = 6.03\cdot10^{23}$:
$\log(N!)\approx N\log(N)-N = 1.3737\cdot10^{25}$
$\log(N!) = 3.2\cdot 10^{25}$


#### Probability of Discrete Events
Suppose you flip 20 fair coins.
1. How many possible outcomes (microstates) are there.
$$\Omega = 2^{20} \mathrm{\ Outcomes}$$
2. What is the probability of getting at singular outcome.
$$p=\dfrac{1}{\Omega} \approx 10^{-6}$$
3. What is the probability of 12 heads, 8 tails.
$$p(12H)=\dfrac{_{20}C_{12}}{\Omega} = \dfrac{\dfrac{20!}{12!\cdot 8!}}{2^{20}} = \dfrac{125970}{1048576} \approx 12.01\% $$


#### Probability of Distributions of Continuous Variables
There are 3 types usually encountered in physics:
1. Uniform distribution (Table distribution)
2. Normal distribution (Gaussian distribution)
3. Exponential distribution

