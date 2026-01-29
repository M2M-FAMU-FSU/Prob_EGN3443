# Module 3 - Formula Sheet (2 sessions, Under Construction)

*** - denotes **IMPORTANT**

* $\mathbb{E}[X] = \sum_{i=1}^n  p(x_i)x_i$ (or)  $\sum_{i}  p(x_i)x_i$ 

## Basic Probability Definitions
* $F(x) = p(\omega \leq x) = \int_{-\infty}^{x}f(\omega)d\omega$ (integral will convert to summation for attributes/pmfs)
* $p(a \leq x \leq b) = \int_{a}^{b}f(x)dx$ (integral will convert to summation for attributes/pmfs)
* $p(\Omega) = \int_{\Omega} f(x)dx = 1$


## Standard (five) Distributions
### 1. Uniform Distribution $\mathcal{U}(a,b)$
* Variable (continuous)
* $a$ - lower limit or bound, $b$- upper limit or bound
* $f(x) = \frac{1}{b-a} \,\, \forall \,\, a \leq x \leq b$ ($0$ otherwise)
* $F(x) = \begin{cases} 0, \,\, \text{if} \,\, x \leq a \\ \frac{x-a}{b-a}, \,\, \text{if} \,\, a \leq x \leq b \\ 1, \,\, \text{if} \,\, x \geq b \end{cases}$ 

### 2. Normal Distribution $\mathcal{N}(\mu,\sigma^2)$ *** 
* Variable (continuous)
* $\mu$ - Mean, $\sigma^2$- Variance 
* $f(x) = \frac{1}{\sqrt{2\pi\sigma^2}}\exp(-\frac{(x-\mu)^2}{2 \sigma^2}) \,\, \forall \,\, x \in (-\infty,\infty) $
* $F(x)$ - use standard normal tables using z-score!
* ***  *Standard Normal Score* or *z-score* $z(x) = \frac{x - \mu}{\sigma}$   
* *** $\Phi(x)$ - cdf of standard normal distribution $\mathcal{N}(0,1)$  
* ***  $F(x) = \Phi(z(x))$ 


### 3. Exponential Distribution $Exp.Dist.(\lambda)$ (used mostly in reliability engineering)
* Variable (continuous)
* $f(x) = \lambda \exp(-\lambda x) \,\, \forall \,\, x \in [0,\infty) $
* $F(x) = 1 - \exp(-\lambda x)$

### 4. Binomial Distribution $\mathcal{B}(N,p)$
* Attribute (discrete)
* $N$ - Number of Trials, $p$ - probability of success in one trial
* $p(x) = \binom{N}{x} p^{x}(1-p)^{N-x} \,\, \forall \,\, x \in \{0,1,2,..., N\} $
* $F(x) = \sum_{i=0}^{x}  \binom{N}{i} p^{i}(1-p)^{N-i}$ 

### 5. Poisson Distribution $Poisson(\lambda)$
* Attribute (discrete)
* $p(x) = \frac{e^{-\lambda} \lambda^x}{x!} \,\, \forall \,\, x \in \{0,1,2,..., \infty\} $
* $F(x) = \sum_{i=0}^{x}  \frac{e^{-\lambda} \lambda^x}{x!} $


## Other Distributions (in this course)
### 6. Bernoulli distribution $Bernoulli(p)$
* Attribute (Discrete), $x \in \{0,1\}$
* $p$ is the probability of success, i.e., probability of getting 1. 
* $(1-p)$ is the probability of failure, i.e., probability of getting 0. 

### 7. Students' t-distribution $t(n-1)$
* Variable (continuous), $x \in (-\infty,\infty)$
* $n$ is the sample size typically
* $n-1$ degrees of freedom

### 8. Chi-squared Distribution $\chi^2(n-1)$
* Variable (continuous) but can only take positive real numbers $x \in [0,\infty)$
* $n$ is the sample size typically
* $n-1$ degrees of freedom

## Sample from a Population Distribution
* Each sample has an associated size $n$
* To draw a histogram of the sample, use approximately $\sqrt{n}$ bins.  
## Concepts
* What is Probability?
* Random Variables
* Discrete RV, Continuous RV
* PMF, PDF, CDF (No standard Distributions)

* Sample Space 
## Math Skills
* Summation <-> Integration





## Concepts
* Expected value 
    * "probablity" weighted average!
    * Expected Value of function of X