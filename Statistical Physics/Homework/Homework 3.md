**Stanley Goodwin, 2/26/2024**

### 3.7 | Gas Mixture
Notes:
$$\begin{align}
\Omega_1(E_1)\propto E_1^{3N/2}, \ \ \ \Omega_2(E_2)\propto E_1^{5N/2}\\
\rho(E_1)\propto\Omega_1(E_1)\Omega_2(E-E_1)
\end{align}$$
a) Calculate the probability density of system 1 being at energy $E_1$.
	What value of $E_1$ maximizes the probability.
$$\begin{align}
\rho(E_1)&\propto\Omega_1(E_1)\Omega_2(E-E_1)\\
\rho(E_1)&\propto E_1^{3N/2}(E-E_1)^{5N/2}\\
\end{align}$$
Probability density:
$$\begin{align}
\int_0^E\rho(E_1)dE_1&=\int_0^E E_1^{3N/2}(E-E_1)^{5N/2}dE_1\\
\left(x=\dfrac{E_1}{E}\right) \ \ \ \ \ \ \ \ \ \ \ \ &= E\cdot E^{3N/2} E^{5N/2}\int_0^1 x^{3N/2}(1-x)^{5N/2}dx\\
&= E^{4N+1}\int_0^1 x^{3N/2}(1-x)^{5N/2}dx\\
&= E^{4N+1}\beta\left(\dfrac{3N}{2}+1,\dfrac{5N}{2}+1\right)\\
&= E^{4N+1}\dfrac{\Gamma\left(\dfrac{3N}{2}+1\right)\Gamma\left(\dfrac{5N}{2}+1\right)}{\Gamma\left(4N+2\right)}\\
&= E^{4N}\dfrac{\left(\dfrac{3N}{2}\right)!\left(\dfrac{5N}{2}\right)!}{\left(4N+1\right)!}\\
\Aboxed{\rho(E_1)&=\dfrac{4N+1}{E^{4N+1}}\left(\begin{array}{c}4N\\\tfrac{3N}{2}\end{array}\right)\cdot E_1^{3N/2}(E-E_1)^{5N/2}}
\end{align}$$
Maximal energy state:
$$\begin{align}
\rho(E_1)&=\dfrac{4N+1}{E^{4N+1}}\left(\begin{array}{c}4N\\\tfrac{3N}{2}\end{array}\right)\cdot E_1^{3N/2}(E-E_1)^{5N/2} \\
\implies \dfrac{\partial \rho(E_1)}{\partial E_1} &= \dfrac{\partial}{\partial E_1}\left(\dfrac{4N+1}{E^{4N+1}}\left(\begin{array}{c}4N\\\tfrac{3N}{2}\end{array}\right)\cdot E_1^{3N/2}(E-E_1)^{5N/2}\right)\\
&= \dfrac{4N+1}{E^{4N+1}}\left(\begin{array}{c}4N\\\tfrac{3N}{2}\end{array}\right)\cdot\dfrac{\partial}{\partial E_1}\left( E_1^{3N/2}(E-E_1)^{5N/2}\right)\\
&=\dfrac{N}{2}\left(\dfrac{3}{E_1}-\dfrac{5}{(E-E_1)}\right)\rho(E_1) = 0\\
\implies 5E_1&=3E-3E_1\\
\Aboxed{E^\mathrm{max}_1 &= \dfrac{3}{8}E}
\end{align}$$

b) Approximate the previous answer as a gaussian, expanding using Taylor series.
	What is the mean energy?
	What is the energy fluctuations per particle?
	Are the fluctuations small relative to $1/\sqrt{N}$ ?

For the sake of the time before I could submit this, I did this without Taylor, but it isn't really needed.
I don't need Taylor series for these ones, since I have the binomial variable for large values of $N$ that follow the very simple relationships:
$$\begin{align}
\mu_E &= E_1^{\mathrm{max}}=\dfrac{3}{8}E\\
2\sigma_E^2 &= \dfrac{3}{8}\cdot\dfrac{5}{8}\cdot\dfrac{1}{N}\\
\implies \sigma_E &= \left(\dfrac{\sqrt{15}}{16}N^{-1/2}\right) E
\end{align}$$
Summarizing it to the following:
$$\boxed{\begin{align}
&\mu_E =\dfrac{3}{8}E &\sigma_E = \left(\dfrac{\sqrt{15}}{16}\dfrac{1}{\sqrt N}\right) E
\end{align}}$$
With the coefficient of the sigma term being approximately 1/4, the fluctuations are relatively small, especially as you take the number of $N$ increases beyond about 20.





### 3.9 | Gauss and Poisson

a) What is the probability that $n$ particles end up in a volume $V$, when the total volume is $KV$ and the total number particles $T = KN_0$.
c) As $K\rightarrow\infty$, show that this distribution becomes the Poisson distribution.
$$\begin{align}
p(n\mathrm{\ in\ }V) &= \left(\begin{array}{c}T\\n\end{array}\right)\cdot p\left(V\right)^n\cdot p\left(KV - V\right)^{T-n}\\
&= \left(\begin{array}{c}T\\n\end{array}\right)\cdot \left(\dfrac{1}{K}\right)^ n\cdot \left(1-\dfrac{1}{K}\right)^{T-n}\\
&= \left(\begin{array}{c}T\\n\end{array}\right)\cdot \left(\dfrac{N_0}{T}\right)^ n\cdot \left(1-\dfrac{N_0}{T}\right)^{T-n}\\
&=\dfrac{N_0^n}{n!}\left(\dfrac{T!}{(T-n)!}\right)\cdot \left(\dfrac{1}{T}\right)^n\cdot \left(1-\dfrac{N_0}{T}\right)^{-n}\cdot\left(1-\dfrac{N_0}{T}\right)^{T}\\
\lim_{T\rightarrow\infty} p(n\mathrm{\ in\ }V) &= \lim_{T\rightarrow\infty}\left(\dfrac{N_0^n}{n!}\left(\dfrac{T!}{(T-n)!}\right)\cdot \left(\dfrac{1}{T}\right)^n\cdot \left(1-\dfrac{N_0}{T}\right)^{-n}\cdot\left(1-\dfrac{N_0}{T}\right)^{T}\right)\\
&= \dfrac{N_0^n}{n!}\lim_{T\rightarrow\infty}\left(1-\dfrac{N_0}{T}\right)^{T}\cdot\lim_{T\rightarrow\infty} \left(\dfrac{T!}{(T-n)!}\cdot \left(\dfrac{1}{T}\right)^n\cdot \left(1-\dfrac{N_0}{T}\right)^{-n}\right)\\
&= \dfrac{N_0^n}{n!}e^{-N_0}\cdot1\\
\Aboxed{\lim_{T\rightarrow\infty} p(n\mathrm{\ in\ }V) &= \dfrac{N_0^n}{n!}e^{-N_0}}
\end{align}$$
The value $a$ equals what we set as $N_0$, therefore $a = N_0$. Rearranging and setting it in terms of the total values, $N_0$ represents the expected value of the particles in a volume $V$ using the average molar density.


b) Show that the Poisson distribution is normalized.
	Calculate the mean of the distribution.
	Calculate the variance of the distribution.
$$\rho(n)=\dfrac{a^n}{n!}e^{-a}$$
Zeroth Moment of the Poisson distribution
$$\begin{align}
\sum_n\rho(n)&=\sum_{n=0}^\infty\dfrac{a^n}{n!}e^{-a}\\
&=e^{-a}\sum_{n=0}^\infty\dfrac{a^n}{n!}\\
&=e^{-a}e^a\\
\Aboxed{\sum_n\rho(n) &= 1}
\end{align}$$
First Moment of the Poisson distribution
$$\begin{align}
\sum_nn\rho(n)&=\sum_{n=0}^\infty n\dfrac{a^n}{n!}e^{-a}\\
&=\sum_{n=1}^\infty \dfrac{a^n}{(n-1)!}e^{-a}\\
&=\sum_{n=0}^\infty \dfrac{a^{n+1}}{n!}e^{-a}\\
&=ae^{-a}\sum_{n=0}^\infty \dfrac{a^{n}}{n!}\\
&=ae^{-a}e^{a}\\
\Aboxed{\sum_nn\rho(n) &= a}
\end{align}$$
Second Moment of the Poisson distribution
$$\begin{align}
w(k+1)&=\sum_nn^{k+1}\rho(n)\\
&=\sum_{n=0}^\infty n^{k+1}\dfrac{a^n}{n!}e^{-a}\\
&=\sum_{n=1}^\infty n^k\dfrac{a^n}{(n-1)!}e^{-a}\\
&=a\sum_{n=0}^\infty (n+1)^k\dfrac{a^n}{(n)!}e^{-a}\\
&=a\sum_{n=0}^\infty\sum_{i=0}^{k} \left(\begin{array}{c}k\\i\end{array}\right)n^i1^{k-i}\dfrac{a^n}{n!}e^{-a}\\
&=a\sum_{i=0}^{k} \left(\begin{array}{c}k\\i\end{array}\right)\sum_{n=0}^\infty n^i\dfrac{a^n}{n!}e^{-a}\\
&=a\sum_{i=0}^{k} \left(\begin{array}{c}k\\i\end{array}\right)w(i)
\end{align}$$
For the choice of $k = 1$, meaning the 2nd moment, we can get that:
$$\begin{align}
w(1+1)&=a\sum_{i=0}^{1} \left(\begin{array}{c}1\\i\end{array}\right)w(i)\\
&=a\left(w(0)+w(1)\right)\\
\Aboxed{\sum_nn^2\rho(n) &= a^2+a}
\end{align}$$
To find the variance, we can write it as:
$$\begin{align}
\left|\langle(x-a)^2\rangle\right|&=\langle x^2-2ax+a^2\rangle\\
&=\langle x^2\rangle-2a\langle x\rangle+a^2\\
&= \left(a^2-a\right) - 2a(a)+a^2\\
&= |-a|\\
\Aboxed{\left|\langle(x-a)^2\rangle\right|&=a}
\end{align}$$







