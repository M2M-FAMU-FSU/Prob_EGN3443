# Module 5 - Formula Sheet (3 Sessions) 

## Standard Distributions with Mean and Variance

| Distribution of RV | $\mathbb{E}[X]$ |  $\mathbb{V}[X]$ |
| --- | --- | --- |
| $X \sim Bernoulli(p)$ | $p$ | $p(1-p)$| 
| $X \sim Poisson(\lambda)$ | $\lambda$ | $\lambda$|  
| $X \sim Uniform(a,b)$ | $\frac{a+b}{2}$ | $\frac{(b-a)^2}{12}$ |
| $X \sim Exponential(\lambda)$ | $\frac{1}{\lambda}$ |  $\frac{1}{\lambda^2}$ |
| $X \sim Binomial(N,p)$ | $Np$ |   $Np(1-p)$  |
| $X \sim \mathcal{N}(\mu,\sigma^2)$ | $\mu$ |   $\sigma^2$  |




* Bias: ($\mathbb{E}_{\theta}[\hat{\theta}] - \theta$)
* Unbiased Estimate: $\mathbb{E}_{\theta}[\hat{\theta}] - \theta = 0$


* $\hat{\mu} = \bar{x}$ 

* $\hat{\sigma^2} = s^2$

* **Standard Error** $\sigma_{\hat{\theta}} = \sqrt{\mathbb{V}(\hat{\theta})}$ 

**rest of it is not well organized**
## Confidence Intervals 
### Useful z-score values
* Two-sided
    * $90\% \implies z_{0.05} = \pm 1.645$
    * $95\% \implies z_{0.025} = \pm 1.96$
    * $99\% \implies z_{0.005} = \pm 2.575$
* One-sided Right Tail
    * $90\% \implies z_{0.1}^{(r)} = 1.28$
    * $95\% \implies z_{0.05}^{(r)} = 1.645$
    * $99\% \implies z_{0.01}^{(r)} = 2.33$
* One-sided Left Tail
    * $90\% \implies z_{0.1}^{(l)} = -1.28$
    * $95\% \implies z_{0.05}^{(l)} = -1.645$
    * $99\% \implies z_{0.01}^{(l)} = -2.33$

### Confidence Interval on Variance
For given error rate ($\alpha$) 

$\frac{(n-1)s^2}{\chi_{\frac{\alpha}{2}}^2(n-1)} \leq \sigma^2 \leq \frac{(n-1)s^2}{\chi_{1-\frac{\alpha}{2}}^2(n-1)}$

* 95% confidence interval $\implies \bar{x} - 1.96.\frac{\sigma}{\sqrt{n}} < \mu <  \bar{x} + 1.96.\frac{\sigma}{\sqrt{n}}$
 
