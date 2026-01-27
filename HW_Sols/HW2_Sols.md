# Homework 2 Solutions  (Under Construction)
*Check Due Date and Office Hours on Canvas* 


[Textbook is here.](https://www.stat.purdue.edu/~qfsong/teaching/511/probability_and_statistics_for_engineering_and_the_sciences.pdf)

1. <span style = color:red> Verify De Morgan's Laws through venn diagrams. For each law, draw two diagrams for each side of inequality (totaling eight diagrams). Each diagram will correspond to one operation ($\cup$,$'$, or $\cap$). Use shading or color to differeniate sets ($A$,$A'$,$B$,$B'$) from each other. 
    * **Law 1**: $(A \cup B)' = A' \cap B' $
    * **Law 2**: $(A \cap B)' = A' \cup B' $ 
</style>

<br>

2. (Events) Textbook Section 2.1 \#1 (Textbook notation for sample notation is $\mathcal{S}$)
    a. $\Omega = \{1324,3124,1342,3142,2314,3214,2341,3241,
                    1423,4123,1432,4132,2413,4213,2431,4231\}$ 

    b. $A = \{1324, 1342, 1423, 1432\}$
    c.  $B = \{2314, 2341, 2413, 2431, 3214, 3241,4213,4231 \}$
    d. $A \cup B = \{1324, 1342, 1423, 1432, 2314, 2341, 2413, 2431, 3214, 3241,4213,4231 \}$
        $A \cap B = \{ \}$ (Null set because either 1 or 2, not both, can get into the championship)
        $A' = \{3124,3142,2314,3214,2341,3241,4123,4132,2413,4213,2431,4231\}$

<br>

3. (Events) Textbook Section 2.1 \#3
    Though not asked, it is a good idea to first write down all possible outcomes (aka Sample Space)
    $\Omega = \{SSS,SSF,SFS,FSS, SFF, FSF, FFS, FFF\}$ ($2^3$ possible outcomes)
    a.  $A = \{SSF,SFS,FSS\}$
    b. $B = \{SSS,SSF,SFS,FSS\}$
    c. $C = \{SSS,SSF,SFS\}$ 
    d. $C' = \{FSS, SFF, FSF, FFS, FFF\}$
        $A\cup C = \{SSF,SFS,FSS, SFF, FSF, FFS, FFF\}$
        $A\cap C = \{FSS\}$
        $B\cup C = \{SSS,SSF,SFS,FSS, SFF, FSF, FFS, FFF\}$
        $B\cap C = \{FSS\}$

<br>

4. (Events, Independence, Disjointness) Textbook Section 2.2 \#17
    a. There is a possibility (an outcome in Sample Space) that the next request is neither SPSS or SAS. 
    b. $P(A') = 1 - 0.3 = 0.7$
    c. $P(A \cup B) =  P(A) + P(B) - P(A\cap B) = 0.3 + 0.5 - 0 = 0.8$ ($P(A\cap B) = 0$ assumed because the request cannot be involving SPSS and SAS at the same time, also otherwise we cannot calculate the values)
    d. Use DeMorgan's Laws (and first axiom of probability)
        $P(A' \cap B') = P((A \cup B)') = 1 - P(A\cup B) = 0.2 $ 

<br>

5. (Probability) Textbook Section 2.2 \#23
   15 ($=$ $^6C_2$) equally likely outcomes
   a. $\frac{^2C_2}{^6C_2}$
   b. $\frac{^4C_2}{^6C_2}$
   c. $\frac{^4C_2 + 4}{^6C_2}$
   d. $\frac{4\times2}{^6C_2}$

<br>

6. (Probability/Counting) Textbook Section 2.3 \#40
    a. $\frac{12!}{3^4}$
    b. (Assuming all outcomes are equally likely)
     $\frac{4!}{\frac{12!}{3^4}}$ 

<br>

7. We have a deck of randomly shuffled typical playing cards (if you do not know about cards, please check online). 
    * If we choose one card at random, 
        * $\Omega = $ All single cards. $n(\Omega) = 52$ 
        * $\frac{26}{52}$
    * If we choose two cards together randomly,
        * $\Omega = $ All combinations of different cards. $n(\Omega) =$ $ 52 \choose 2$ 
        * $\frac{26 \choose 2}{52 \choose 2}$
        * $\frac{26 \choose 1 }{52 \choose 2} \times \frac{26 \choose 1 }{52 \choose 2}$
    * If we choose two cards one-after-another after replacing the card
        * $\Omega = $ All combinations including choosing the same card twice, $n(\Omega) =$ $ 52\times52$ 
        * $\frac{26 \times 26}{52 \times 52}$
        * $\frac{26 \times 26}{52 \times 52}$


8. (A classical problem) 
*You need to apply Bayes' Theorem*
Let $A$ denote the event that I have COVID-19 $\implies$ $A'$ is the event that I do not have COVID-19. $A$ and $A'$ form mutually exlusive and exhaustive events such that $P(A) + P(A') = 1$. 
Let $B$ denote the event that I tested positive. We need to find $P(A|B)$

$$P(A|B) = \frac{P(B|A)P(A)}{P(B|A)P(A) + P(B|A')P(A')}$$

$$P(A) = 0.1 \implies P(A') = 0.9$$

$$P(B|A) = 0.99, P(B|A') = 0.02$$

$$\implies P(A|B) = \frac{0.99 \times 0.1 }{0.99 \times 0.1 + 0.02 \times 0.9} = 84.6\%$$ *(surprising?)*

<br>

9. Textbook Section 2.4 \#60
(Another application of Bayes' Theorem) 
We are only talking about light aircraft, so you do not need to be thinking about other aircrafts (for example, you do not need to worry about $P(Discovered|NotLightAircraft)$)

Given light aircraft,
$P(Discovered) = 0.7$
$P(YesLocator|Discovered) = 0.6$
$P(NoLocator|NotDiscovered) = 0.9$


a. $$P(NotDiscovered|YesLocator) = \frac{P(YesLocator|NotDiscovered)P(NotDiscovered)}{P(YesLocator|NotDiscovered)P(NotDiscovered) + P(YesLocator|Discovered)P(Discovered)}$$


* $P(YesLocator|NotDiscovered) = 1 - 0.9 = 0.1$
* $P(NotDiscovered) = 1 - 0.7 = 0.3$

$$P(NotDiscovered|YesLocator) = \frac{0.1\times0.3}{0.1\times0.3 + 0.6 \times 0.7} = \frac{3}{45} = \frac{1}{15}$$

<br>
10. <span style = color:red> Textbook Section 2.4 \#63 (b), (c), (d) and (e). (You may read about tree diagram in (a) if you are curious) 
</style>

<br>

11.<span style = color:red>  Textbook Section 2.5 \#80
    * Additionally, write the definitions of sample space and events, that help you formulate this problem to calculate the probability values? Draw a relevant Venn diagram, if possible. 
</style>

12. Car manufacturing can be considered an assembly of 500 independent components. If 99.9\% of cars needs to be defect-free, 
    * If $p$ is the required probability $(1-p)^{500} = 0.999 \implies (1-p) \approx 0.999998 \implies p = 0.000002 = 2 ppm$
    * Write the definitions of sample space and events, that help you formulate this problem to calculate the probability of defective cars? Draw a relevant Venn diagram, if possible. 

