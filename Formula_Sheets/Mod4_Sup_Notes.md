# Module 4 Supplementary Notes (Optional)
Derivation of two key results
1. For **any** random variable
    $$ \mathbb{E}[X_1 + X_2 + \cdots + X_n] = \mathbb{E}_1[X_1] + \mathbb{E}_2[X_2] + \cdots +  \mathbb{E}_n[X_n]$$ 
2. For **independent** random variables
    $$ \mathbb{E}[X_1X_2] = \mathbb{E}_1[X_1]\mathbb{E}_2[X_2]$$

## 1. Expected Value of Sum of Random Variables
### Marginal Distribution (Definition)

$$f_1(x_1) = \int_{-\infty}^{\infty} f_{12}(x_1,x_2) dx_2 $$
$$f_2(x_2) = \int_{-\infty}^{\infty} f_{12}(x_1,x_2) dx_1 $$

---
### Expected Value of Sum of Two Random Variables
$$ T = X_1 + X_2$$

$$ \mathbb{E}[T] = \mathbb{E}_{12}[X_1 + X_2] = \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} (x_1 + x_2) f_{12}(x_1, x_2) dx_1dx_2$$

$$  = \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} x_1 f_{12}(x_1, x_2) dx_1dx_2 + \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} x_2 f_{12}(x_1, x_2) dx_1dx_2$$

$$  = \underbrace{\int_{-\infty}^{\infty} \int_{-\infty}^{\infty}}_{swap}  x_1 f_{12}(x_1, x_2) \underbrace{dx_2dx_1}_{swap} + \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} x_2 f_{12}(x_1, x_2) dx_1dx_2$$

$$  = \int_{-\infty}^{\infty} x_1\Big (\int_{-\infty}^{\infty}  f_{12}(x_1, x_2) dx_2 \Big)dx_1 + \int_{-\infty}^{\infty} \Big( x_2 \int_{-\infty}^{\infty} f_{12}(x_1, x_2) dx_1 \big) dx_2$$

$$  = \underbrace{\int_{-\infty}^{\infty} x_1 f_1(x_1) dx_1}_{\mathbb{E}_1[X_1]} + \underbrace{\int_{-\infty}^{\infty} x_2 f_2(x_2) dx_2}_{\mathbb{E}_2[X_2]} $$
$$\implies \mathbb{E}_{12}[X_1 + X_2] = \mathbb{E}_{1}[X_1] + E_2[X_2]$$


---
### Expected Value of Sum of $n$ Random Variables
$$ \mathbb{E}[T] = \mathbb{E}[X_1 + X_2 + \cdots + X_n] = \int \int \cdots \int (x_1 + x_2 + \cdots x_n) f(x_1, x_2, \cdots x_n) dx_1dx_2 \cdots dx_n$$    

$$ = \int \int \cdots \int (x_1) f(x_1, x_2, \cdots x_n) dx_1dx_2 \cdots dx_n  +  \int \int \cdots \int (x_2) f(x_1, x_2, \cdots x_n) dx_1dx_2 \cdots dx_n + \cdots +   \int \int \cdots \int (x_n) f(x_1, x_2, \cdots x_n) dx_1dx_2 \cdots dx_n + \cdots$$

$$ = \mathbb{E}_1[X_1] + \mathbb{E}_2[X_2] + \cdots +  \mathbb{E}_n[X_n]$$


## 2. Expected Value of Product of RVs

$$ \mathbb{E}[X_1X_2] = \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} x_1x_2 f_{12}(x_1, x_2) dx_1dx_2 = \int_{-\infty}^{\infty} \Big(\int_{-\infty}^{\infty} x_1x_2 f_{12}(x_1, x_2) dx_1 \Big) dx_2 $$

$$ = \int_{-\infty}^{\infty} x_2 \Big(\int_{-\infty}^{\infty} x_1 f_{12}(x_1, x_2) dx_1 \Big) dx_2 $$

(if independent 
$f_{12}(X_1,X_2) = f_1(X_1) f_2(X_2)$)
$$ = \int_{-\infty}^{\infty} x_2 \Big(\int_{-\infty}^{\infty} x_1 f_{1}(x_1) f_2(x_2) dx_1 \Big) dx_2 $$

$$ = \int_{-\infty}^{\infty} x_2 f_2(x_2) \underbrace{\Big(\int_{-\infty}^{\infty} x_1 f_{1}(x_1)  dx_1 \Big)}_{\mathbb{E}_1[X_1]} dx_2 $$
$$ = \int_{-\infty}^{\infty} x_2 f_2(x_2) \mathbb{E}_1[X_1] dx_2 $$
$$ = \mathbb{E}_1[X_1]\int_{-\infty}^{\infty} x_2 f_2(x_2)  dx_2 $$
$$ = \mathbb{E}_1[X_1]\mathbb{E}_2[X_2]$$


<!-- ### If Independent RVs

$$P_{12}(X_1,X_2) = P_1(X_1) P_2(X_2)$$ -->


---

<!-- ---
 $$   = \int_{-\infty}^{\infty} \Big(\int_{-\infty}^{\infty} x_1 f_{12}(x_1, x_2) dx_1 + \int_{-\infty}^{\infty} x_2 f_{12}(x_1, x_2) dx_1 \Big) dx_2$$  

(*Wrong route*) If independent
$$   = \int_{-\infty}^{\infty} \Big(\int_{-\infty}^{\infty} x_1 f_1(x_1)f_2(x_2) dx_1 + \int_{-\infty}^{\infty} x_2 f_1(x_1)f_2(x_2) dx_1 \Big) dx_2$$  


$$   = \int_{-\infty}^{\infty} \Big(f_2(x_2) \int_{-\infty}^{\infty} x_1 f_1(x_1) dx_1 + x_2 f_2(x_2) \int_{-\infty}^{\infty}  f_1(x_1) dx_1 \Big) dx_2$$  


$$   = \int_{-\infty}^{\infty} \Big(f_2(x_2) \mathbb{E}_1[X_1] + x_2 f_2(x_2) (1) \Big) dx_2$$  
$$   = \int_{-\infty}^{\infty} f_2(x_2) \mathbb{E}_1[X_1]dx_2 +  \int_{-\infty}^{\infty} x_2 f_2(x_2) dx_2$$  
$$   =  \mathbb{E}_1[X_1] \int_{-\infty}^{\infty} f_{X_2}(x_2) dx_2 + \mathbb{E}_2[X_2]$$  
$$   =  \mathbb{E}_1[X_1] (1) + \mathbb{E}_2[X_2] =  \mathbb{E}_1[X_1] + \mathbb{E}_2[X_2] $$  

---

$$ \mathbb{E}[T] = \mathbb{E}_{12}[X_1 + X_2] = \int_{-\infty}^{\infty} \Big(\int_{-\infty}^{\infty} (x_1 + x_2) f_{12}(x_1, x_2) dx_1\Big)
---
$$ T = X_1 + X_2 + X_3 + \cdots + X_n$$ -->

