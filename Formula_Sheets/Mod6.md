# Module 6 - Formula Sheet (3 Sessions) 




## Errors in Hypothesis Testing 
* *p-value* $\leq \alpha$ $\implies$ Reject $H_0$ 
* *Type-I Error*:(Definition) Reject $H_0$ when it is True  
    * $\alpha$ = $p$(*Type-I Error*) 
    * Typically, the $\alpha$ values are provided as 5% or 10%

### Gamma Distribution 
* $f(x) = \frac{1}{\Gamma(\alpha) \beta^{\alpha}}x^{\alpha -1}e^{-\frac{x}{\beta}} \,\, \forall \,\, x \in [0,\infty]$
* Parameters - Shape $\alpha$, scale $\beta$
* Gamma function $\Gamma(\alpha)  = \int_0^\infty t^{\alpha-1}e^{-t}dt$

### 7. Students' t-distribution $t(n-1)$
* $f(x) =\frac{\Gamma(\frac{\nu +1}{2})}{\sqrt{\pi \nu} \Gamma(\frac{\nu}{2})} (1+\frac{x^2}{\nu})^{-\frac{\nu + 1}{2}}$
* $\mu = 0$ and $\sigma^2 = \frac{\nu}{\nu - 2}$
* Variable (continuous), $x \in (-\infty,\infty)$
* $\nu$ is the degrees of freedom
* $n-1$ degrees of freedom

### 8. Chi-squared Distribution $\chi^2(n-1)$
* Variable (continuous) but can only take positive real numbers $x \in [0,\infty)$
* $n$ is the sample size typically
* $n-1$ degrees of freedom

## p-value of Hypothesis Testing ***

### Assuming Normal Distribution of $x$ 
* **Testing on $\mu$** 
    *  Known $\sigma^2$ - "One Sample z-test" $\implies z_{test} = \frac{\bar{x} - \mu_0}{\sigma/\sqrt{n}}$
        * $H_0$: $\mu = \mu_0$; $H_a$: $\mu \neq \mu_0$ $\implies$ Two-sided $\implies$ *p-value* = $2p(Z \geq |z_{test}|)$ 
        * $H_0$: $\mu = \mu_0$; $H_a$: $\mu > \mu_0$ $\implies$ One-sided (Upper Tail Test) $\implies$ *p-value* = $p(Z \geq z_{test})$ 
        * $H_0$: $\mu = \mu_0$; $H_a$: $\mu < \mu_0$ $\implies$ One-sided (Lower Tail Test) $\implies$ *p-value* = $p(Z \leq z_{test})$ 
    * Unknown $\sigma^2$ - "One Sample t-test" $\implies t_{test} = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}$ (remember to use (n-1) degrees of freedom) 
        * $H_0$: $\mu = \mu_0$; $H_a$: $\mu \neq \mu_0$ $\implies$ Two-sided $\implies$ *p-value* = $2p(T \geq |t_{test}|)$ 
        * $H_0$: $\mu = \mu_0$; $H_a$: $\mu > \mu_0$ $\implies$ One-sided (Upper Tail Test) $\implies$ *p-value* = $p(T \geq t_{test})$ 
        * $H_0$: $\mu = \mu_0$; $H_a$: $\mu < \mu_0$ $\implies$ One-sided (Lower Tail Test) $\implies$ *p-value* = $p(T \leq t_{test})$ 
* **Testing on $\sigma^2$**
    * "Chi-squared Test" $\implies \chi_{test}^2 = \frac{(n-1)s^2}{\sigma_0^2}$
    * Two-sided $\implies$ *p-value* $= \min(p(\chi^2 > \chi_{test}^2), p(\chi^2 < \chi_{test}^2)) $
