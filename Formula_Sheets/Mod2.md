# Module 2 - Formula Sheet (3 sessions)
(Chapter 2 in Textbook)
May be useful to refer [mathematical notations](https://m2m-famu-fsu.github.io/Prob_EGN3443/Notations.html)

## Definitions
* Events - Subset of Sample Space $A \subseteq \Omega$ or $A \in 2^{\Omega}$
* Probability ($p(A)$) - Every event has an associated probability
    * **Axioms of Probability**
        1. $p(\Omega) = 1$
        2. For any event A, $p(A) \geq 0$
        3. If $A_i$ are disjoint (mutually exclusive) events, $p(\cup_{i=1}^{\infty} A_i) = \sum_{i=1}^{\infty} p(A_i)$
* Two events are independent $\implies P(A \cap B) = P(A).P(B) $
* Exhaustive Events  $\cup_{i=1}^{k} A_i = \Omega$ 
## Probability Relations
* $p(A|B) = \frac{p(A \cap B)}{p(B)} \Leftrightarrow P(A\cap B) = P(A|B).P(B)$ 
* $p(A \cup B) = p(A) + p(B) - P(A \cap B)$
* $p(A \cup B \cup C) = p(A) + p(B) + p(C) - P(A \cap B) - P(B \cap C) - P(A \cap C) +  P(A \cap B \cap C)$
* **Law of Total Probability**
    If $A_1,...,A_k$ are mutually exlusive and exhaustive events. 
    $P(B) = \sum_{i=1}^{k}P(B|A_i)p(A_i)$
* **Bayes' Theorem**
    If $A_1,...,A_k$ are mutually exlusive and exhaustive events. 
    $P(A_j|B) = \frac{P(B|A_j)P(A_j)}{\sum_{i=1}^{k}P(B|A_i)p(A_i)}$

## Basic Mathematics
### Permutations and Combinations
* $^nC_r =$ $n\choose r$ $= \frac{n!}{r! \times (n-r)!}$
* $^nP_r =$ $n\choose r$ $\times r!= \frac{n!}{(n-r)!}$

### DeMorgan's Laws
  * $(A \cup B)' = A' \cap B' $
  * $(A \cap B)' = A' \cup B' $ 








