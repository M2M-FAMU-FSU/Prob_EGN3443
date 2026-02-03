# Module 4 - Formula Sheet (3 Sessions, Under Construction) 

* Expected Values
    * Mean, Variance Definitions.


### 7. Students' t-distribution $t(n-1)$
* Variable (continuous), $x \in (-\infty,\infty)$
* $n$ is the sample size typically
* $n-1$ degrees of freedom

### 8. Chi-squared Distribution $\chi^2(n-1)$
* Variable (continuous) but can only take positive real numbers $x \in [0,\infty)$
* $n$ is the sample size typically
* $n-1$ degrees of freedom




### 3. Exponential Distribution $Exp.Dist.(\lambda)$ (used mostly in reliability engineering)
* Variable (continuous)
* $f(x) = \lambda \exp(-\lambda x) \,\, \forall \,\, x \in [0,\infty) $
* $F(x) = 1 - \exp(-\lambda x)$

### 4. Binomial Distribution $\mathcal{B}(N,p)$
* Attribute (discrete)
* $N$ - Number of Trials, $p$ - probability of success in one trial
* $p(x) = \binom{N}{x} p^{x}(1-p)^{N-x} \,\, \forall \,\, x \in \{0,1,2,..., N\} $
* $F(x) = \sum_{i=0}^{x}  \binom{N}{i} p^{i}(1-p)^{N-i}$ 


2. **Normal Distribution** $\mathcal{N}(\mu,\sigma^2)$ *** 
    * Variable (continuous)
    * $\mu$ - Mean, $\sigma^2$- Variance 
    * $f(x) = \frac{1}{\sqrt{2\pi\sigma^2}}\exp(-\frac{(x-\mu)^2}{2 \sigma^2}) \,\, \forall \,\, x \in (-\infty,\infty) $
    * $F(x)$ - use standard normal tables using z-score!
    * ***  *Standard Normal Score* or *z-score* $z(x) = \frac{x - \mu}{\sigma}$   
    * *** $\Phi(x)$ - cdf of standard normal distribution $\mathcal{N}(0,1)$  
    * ***  $F(x) = \Phi(z(x))$ 
