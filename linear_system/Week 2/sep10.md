## Interesting question from the class

$$ \begin{align} &f(t)\delta(t-t_1)\delta(t-t_2)\\ &\delta^2(t-t_1)\rightarrow \delta(t-t_1) \text{ if } t_1=t_2 \\ &0 \text{ when }t_1 \neq t_2 \end{align}$$

> 09/16 Update: It seems like that $\delta^2$ is not a valid operation. 

## Ramp Function $$ r(t) = tu(t) $$ 
## System as interconnection of operation

> add something here
# System
## properties of systems

- Stability
- Memory
- Causality
- Invertibillity
- Time invariance
- Linearity
## stability
### BIBO (bounded-input bounded-output)
Assume
$$ |x[n]| < M_0 < \infty$$
here $M_0$
then use abs to check

$$  |y[n] |=[r^nx[n]=|r^n|*|x[n] $$


## Memory
Output depends on non-present (e.g. past or future) called memory.

$$ (x[n-1]+x[n]+x[n+1]) $$
is a  memory system, as it depends on past($x[n-1]$)  and future($x[n+1]$).
