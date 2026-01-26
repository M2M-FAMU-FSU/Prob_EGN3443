# Coffee Discussion (Instruction Material)
### **Intro/Module 1: Session \#1** (in prep)
Have you faced issues with parking or seen cars parked on grass at COE? How can you design the number of parking spots necessary?

### **Module 2 (Session \#5)** 
You are designing a bridge. A structural engineer asks you, will the bridge fail? There are some known causes (listed below). 
* Dead loads (the bridge structure itself) 
* Live loads (moving vehicles/people) 
* Winds
* Rain 
* Snow
* Heat
* Earthquakes 
    
**Prompts**
* How will you answer? 
<span style = "color: red"> The answer is never binary (yes or no). Change the question to "how likely" the bridge will fail. We need to quantify as probability - specifically, in terms of time/days per year/decade/century that the authorities can understand.    </style>
* Describe all the information you need (which may be available or collectable) \& how will you make sense of that information?
<span style = "color: red"> 
        *Two types on information (Are there more?)* 
        * How likely (probability) the bridge will fail with each associated cases.
        * How likely (probability) the loading itself can occur (over time)?    </style>
* How will you give a mathematical form to this? 
<span style = "color: red"> 
        * Sample Space: $ \Omega = \{0, 1\}$ with $0$ indicating that the bridge fails. 
        * Event (subset of sample space): Only four ($2^2$) possible events $\{\}, \{0\}, \{1\}, \{0,1\}$
        * Can you answer the question with the given information using this mathematical form? 
    <br> 
        * Sample Space: $\{ a-failure, b-failure,..., f-failure \}$. 
        * Event (subset of sample space): $2^6 = 64$ possible events - each denoting 
        * Can you find the probability with the given information? 
        * Can you answer the question with the given information using this mathematical form?
    <br>
        * Sample Space: $\{ a-occurs, b-occurs,..., f-occurs, bridge fails\}$.
        * Event (subset of sample space): $2^7 = 128$ possible events - half of those "events" include bridge failing!
        * Can you find the probability with the given information?
        * Define Events - We need to find $p(\{bridgefails\}) = ?$
            We can use information
            * $p(\{bridgefails\}|\{a-occurs\}), p(\{bridgefails\}|\{b-occurs\}),$ etc.
            * $p(a-occurs),p(b-occurs),...,$
    <br>
    * Sample Space: All time from now or $(0,\infty)$
        * Event (subset of sample space): $2^\infty$
        * Define Events: a-occurs, b-occurs, bridgefails, etc. 
        * We need to find $p(bridgefails) = ?$
        * We can ask for information such as
            * $p(bridgefails|a-occurs), p(bridgefails|b-occurs),$ etc.
            * $p(a-occurs),p(b-occurs),...,$
        * We can also think about events occuring together (two events,three events,..., seven events) - find appropriate 'combinatorial' probability. 
        * We can use interdependencies, mutually exclusive events, etc. 
    </style>
