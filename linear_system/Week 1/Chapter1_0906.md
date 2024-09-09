# Signal Type

## Continuous-time signal $x(t)$
Defined across all time $t$ 
## Discrete-time signal $x[n]$
Defined only at discrete times $n$
**$n$ needs to be an integer.**
## Even signal
$$ x(t) = x(-t) $$

Can be describe as **mirror across y-axis**.
## Odd signal
$$ x(t) = -x(t) $$

Can be describe as **rotate 180 degree around origin**.

## Quick distinguishing

![](attachs/Pasted%20image%2020240909223401.png)
## Even-Odd decomposition
Define 

$$ x(t)=x_e(t)+x_o(t)$$

Where $x_e$ is even part, $x_o$ is odd part, then 

$$ \begin{cases} 
x_e(t) = \frac{1}{2}[x(t)+x(-t)] \\ 
x_o(t) = \frac{1}{2}[x(t)-x(-t)] 
\end{cases} 
$$ 

## Periodic signal
### Continuous-time signal
For continuous-time signal $x(t)$, if there exists a $T$ such that

$$ x(t) = x(t+T) $$

Where the smallest possible $T$ is being called as "The Fundamental period"
### Discrete-time signal
For discrete-time signal $x[n]$, if there exists a $N$ such that

$$ x[n] = x[n+N] $$

Where the smallest possible $N$ is being called as "The Fundamental period"
**$N$ is also need to be an integer.**
## Non-Periodic signal

> Some picture here.
