## Mini Project 2 - Atomic Diffusion Process
*Check Canvas for Deadlines and Office Hours*

**The necessary Python code is available [here](https://colab.research.google.com/drive/1Xa7q9WCV04prodgW6G-1MeYrbnfujNcH?usp=sharing).** 

An atomic diffusion process looks [like this](https://en.wikipedia.org/wiki/File:Chemical_surface_diffusion_slow.gif). Imagine a single atom sitting on a lattice site in a crystal. Every $\tau$ seconds, it gains enough thermal energy to jump to an adjacent site at distance $a$, i.e., jump to $(current position + a)$ or $(current position - a)$.



### Task 1: 1D "Drunkard's Walk" 
 In a simple 1D model, assume that the atom can move either left or right with equal probability ($p = 0.5$). If there are $k$-particles all starting at $x = 0$ at time $t = 0$, derive the $E[X]$ and $Var[X]$ of positions of these $k$ particles after $n \tau$ seconds. Fill in the code with ($E[X]$ and $Var[X]$) in the code at this line (do not modify anything else): 
```
E_x =   #Fill in here
V_x =   #Fill in here
```
If the appropriate values are entered, the code will run. Check for the saved .gif file (instructions below)

### Task 2: 3D Squared Displacement
If the atoms can move to adjacent sites in 3D (jump $+a$ or $-a$ in any of the three directions with equally likely probabilities), what is the expected value and variance of squared displacement $r^2$? Note the general definition of displacement is $r = \sqrt{x^2 + y^2 + z^2}$. It may be helpful to start thinking in 1D then move to 3D.

```
E_r2 =  # Fill-in here
V_r2 =  # Fill-in here
```


### Task 3: Manufacturing Scenario: Carbon Diffusing in Body Centered Cubic (BCC) Iron
Arrhenius law provides the relationship to relate temperature (thermal energy) to$\tau$ as 
$$\frac{1}{\tau} = \nu_0 \exp(-\frac{Q}{k_BT})$$ 

where $T$ is the temperature. It is known that attempt to jump frequency $\nu_0 = 10^{13} Hz$ for carbon in BCC iron, activation energy $Q = 0.83 ev$, and Boltzmann constant $k_B = 8.617 \times 10^{-5} ev/K$.  

If the expected value from the Task 2 in 3D equals $6D(n\tau)$, find the diffusion coefficient $D$ assuming that the step size $a = 0.2nm$ at *(1)* room temperature ($300K$) and while *(2)* heat treatment ($1000K$).  


## Deliverables
1. In a single pdf file, include
    * Derivations of Task 1 and Task 2. (handwritten is okay)
    * Task 1 and Task 2 answering whether you see a match with blue line and the histogram? Why or why not?
    * Diffusion coefficient values from Task 3.
2. .gif files from Task 1 and Task 2. 

## Tips for Python in Google Colab

1. You need to know basic mathematical operations in Python, i.e., $+$,$-$, $*$ and $/$.
2. You will find the save '.gif' files usually if you click the folder button on the left sidebar. 

<img src="./Colab_sidebar.png" alt="A simple flow chart" width="50" height="100">
