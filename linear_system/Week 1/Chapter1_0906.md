# Signal Type

## Continuous-time signal $x(t)$
Defined across all time $t$ 
## Discrete-time signal $x[n]$
Defined only at discrete times $n$
**$n$ needs to be an positive integer.**
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
When we facing $sin(n)$ or $cos(n)$, to be able to achieve periodic signal, **$n$ must be an integer multiple of $2\pi$**. Therefore we can find an positive integer $N$ to proof the periodicity of $sin(n)$ or $cos(n)$.
Then the fundamental angular frequency is $\Omega = \frac{2\pi}{N}$.
## Non-Periodic signal
![](attachs/Pasted%20image%2020240909225626.png)

## Energy and Power of a signal

### Continuous-time signal
#### Insta-power
$$ p(t) = |x(t)|^2 $$
#### Total energy
$$ E = \int_{-\infty}^{\infty} |x(t)|^2 dt $$
#### Average power
$$ P = \lim_{T\to\infty} \frac{1}{T} \int_{-T/2}^{T/2} |x(t)|^2 dt $$

### Discrete-time signal