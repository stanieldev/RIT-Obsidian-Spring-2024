### Distributions: $\chi^2$ Statistics
$$\chi^2_T = \sum \left(\dfrac{y-f(x)}{\delta_y}\right)^2$$
For appropriate error bars, we expect $\chi^2 \approx 1$, where $\chi^2 = \dfrac{\chi^2_T}{df}$.
The p-value of the $\chi^2$ is related to the probability that a dataset would exceed this $\chi^2$.

### Propagation of Uncertainty
You've measure some values of $x_i\pm \delta x_i$.
Given a function $f(x_i)$, how would you determine $\delta f(x_i)$?
$$\delta f(x_i) = \sqrt{\sum_i\left|\dfrac{\partial f}{\partial x_i}\delta x_i\right|^2}$$
For non-derivable variables, we can express it as:
$$\delta \hat{X} = \sqrt{\sum{(\delta X_{x_i})^2}}, \mathrm{\ where\ } \delta X_{x_i}=X_{x_i}-\dfrac{X(x_i+\delta x_i)+X(x_i-\delta x_i)}{2}$$
