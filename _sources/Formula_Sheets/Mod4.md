# Module 4 - Formula Sheet (3 Sessions) 

## Population Mean and Variance
* $\mu_X = \mathbb{E}[X]$
* $\sigma^2_X = \mathbb{E}[(X-\mu_X)^2] = \mathbb{E}[X^2] - (\mathbb{E}[X])^2$ 

## Distributions of i.i.d. Sample Statistics
* $\mathbb{E}[T] = n\mu$
* $\mathbb{V}[T] = n\sigma^2$
* $\mathbb{E}[\bar{X}] = \mu_{\bar{X}} = \mu $
* $\mathbb{V}[\bar{X}] = \frac{\sigma^2}{n} $

## Linear Combination of independent RVs.
* If $Y = \sum_{i=1}^{n} a_iX_i$
   * $\mu_{Y} = \sum_{i=1}^{n} a_i\mu_i$
   * $\sigma^2_{Y} = \sum_{i=1}^{n} a_i^2\sigma^2_i$


### Binomial Distribution $\mathcal{B}(N,p)$
 * If $X \sim Bernoulli(p)$, then $Y = (X_1 + X_2 + X_3 + ... + X_N) \sim Binomial (N,p)$
    * Attribute (discrete)
    * *Use cases*: Probability of defective items in a batch, \# of rainy days in a year.  
    * $N$ - Number of Trials, $p$ - probability of success in one trial
    * $p(x) = \binom{N}{x} p^{x}(1-p)^{N-x} \,\, \forall \,\, x \in \{0,1,2,..., N\} $
    * $F(x) = \sum_{i=0}^{x}  \binom{N}{i} p^{i}(1-p)^{N-i}$ 


### **Normal/Gaussian Distribution** $\mathcal{N}(\mu,\sigma^2)$ *** 
 * From Central Limit Theorem!   
    * Variable (continuous)
    * Most Widely Used Distribution: *Some Examples*: Drug Trials (or broadly hypothesis testing), Quality Control, AI/Machine Learning. 
    * $\mu$ - Mean, $\sigma^2$- Variance 
    * $f(x) = \frac{1}{\sqrt{2\pi\sigma^2}}\exp(-\frac{(x-\mu)^2}{2 \sigma^2}) \,\, \forall \,\, x \in (-\infty,\infty) $
    * $F(x)$ - use standard normal tables using z-score!
    * ***  *Standard Normal Score* or *z-score* $z(x) = \frac{x - \mu}{\sigma}$   
    * *** $\Phi(x)$ - cdf of standard normal distribution $\mathcal{N}(0,1)$  
    * ***  $F(x) = \Phi(z(x))$ 
