# Module 3 - Formula Sheet (2 sessions)

## Basic Math
* Summation in Discrete $\leftrightarrow$ Integration in Continuous
* **Binomial Theorem** $(a+b)^n = \sum_{x=0}^n$ $n \choose x$ $a^x b^{n-x}$  
* **Taylor Series** $f(x) = f(a) + \frac{f'(a)}{1!} (x-a) + \frac{f''(a)}{2!} (x-a)^2 + \cdots \infty \,\, terms$ 
    * $e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!}$ (by substituting $a = 0$)
* **Sum of Infinite terms in Geometric Series** 
    * $s = a + ar + ar^2 + \cdots \infty \,\, terms = \frac{a}{1-r}$ (only if $0<r < 1$)

## Basic Probability Definitions
* **CDF** $F(x) = p(\omega \leq x) = \int_{-\infty}^{x}f(\omega)d\omega$ (integral will convert to summation for attributes/pmfs)
* $p(a \leq x \leq b) = \int_{a}^{b}f(x)dx$ (integral will convert to summation for attributes/pmfs)
* $p(\Omega) = \int_{\Omega} f(x)dx = 1$

## Expected Values
* $\mathbb{E}[X] =   \sum_{i}  p(x_i)x_i$ (or) $\int_ {-\infty}^{\infty}xf(x)dx$
* $\mathbb{E}[g(X)] = \sum_{i}  p(x_i)g(x_i)$ (or) $\int_ {-\infty}^{\infty}g(x)f(x)dx$ 
    * $\mathbb{E}[aX + b] = a\mathbb{E}[X] + b$


## Basic PMFs
1. **Bernoulli distribution** $Bernoulli(p)$
    * *Use Cases:* Coin Toss, Defective-Not Defective, Positive-Negative
    * Discrete (Attribute), $x \in X, \,\, X = \{0,1\}$
    * $P(1) = p$ and $P(0) = 1-p$

2. **Poisson Distribution** $Poisson(\lambda)$
    * *Use Cases:* Any "arrival" process. 
    * Discrete (Attribute)
    * $p(x) = \frac{e^{-\lambda} \lambda^x}{x!} \,\, \forall \,\, x \in X, \,\, X=\{0,1,2,..., \infty\} $
    * $F(x) = \sum_{i=0}^{x}  \frac{e^{-\lambda} \lambda^i}{i!} $


## Basic PDFs
1. **Uniform Distribution** $\mathcal{U}(a,b)$
    * *Use cases*: Niche but good for developing understanding. 
    * Continuous RV
    * $a$ - lower limit or bound, $b$- upper limit or bound
    * $f(x) = \frac{1}{b-a} \,\, \forall \,\, a \leq x \leq b$ ($0$ otherwise)
    * $F(x) = \begin{cases} 0, \,\, \text{if} \,\, x \leq a \\ \frac{x-a}{b-a}, \,\, \text{if} \,\, a \leq x \leq b \\ 1, \,\, \text{if} \,\, x \geq b \end{cases}$ 


2. **Exponential Distribution** $Exponential(\lambda)$ 
    * *Use Cases:* Time to fail, Waiting Time 
    * Variable (continuous)
    * $f(x) = \lambda \exp(-\lambda x) \,\, \forall \,\, x \in X, \,\,X =  [0,\infty) $
    * $F(x) = 1 - \exp(-\lambda x)$









