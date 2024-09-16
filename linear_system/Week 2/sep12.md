## Causality
causal when present value of the output signal depends only on present or past value of input signal.

##### Example:
$$ y[n]=x[n-1]+x[n]+x[n+1] $$
which required future value of input signal, so it is not causal.

## Invertibility
A system is invertible if input signal can be recovered from output signal'.
In mathematical terms $$
H^{inv}\{H\{x[n]\}\}=x[n]
$$
caveat:
- It must be one-to-one mapping between input and output signal.

## Time Invariance
Time invariance means that the system responds identically to the same input signal no matter when

math term: 

$$ \begin{align}
&x(t) \rightarrow y(t)\\ 
&x(t-\tau) \rightarrow y(t-\tau)
\end{align}
$$
##### Ex:
>from ppt chap1-132
>**make input $\tau$ as $t-t_0$**

## Linearity
### Superposition(Additivity $+$ )
$$ \begin{align}
\text{If  }  &x_1(t) \xrightarrow[]{H} y_1(t) \text{ and } x_2(t) \rightarrow y_2(t) \\
\text{ then } &x_1(t)+x_2(t) \xrightarrow[]{H} y_1(t)+y_2(t)
\end{align}
$$

### Homogeneity(Scaling $\times$)
	$$\begin{align}
	\text{If }  x(t) &\xrightarrow[]{H} y(t) \\
	\text{ then } ax(t) &\xrightarrow[]{H} ay(t)
	
	\end{align}$$
	
#### Ex: 

$$ y[n]=nx[n] $$
steps: 
1. let a new signal $x[n]2$
> TODO

## Review 
### Stability
Assume $|x[n]| \leq M_x \lt \infty$ then $|y[n]| \leq M_y \lt \infty$.

### Memory
$y[n]$ is a function of $x[n+k]$ where $k$ is a constant that $\neq 0$.

### Causality
$y[n]$ is a function of $x[n-k]$ where $k$ is a constant that $\gt 0$.

### Invertibility
Find out $H^{inv}$ such that $H^{inv}\{H\{x[n]\}\}=x[n]$.

### Time Invariance
assume $y[n] = H\{x[n]\}$
let input: $x[n-n_0]$ then shall output be: $y[n-n_0]$

## Linearity: 
assume $$
y_i[n]=H\{x_i[n]\}
$$
then let 
$$
x[n] = \sum_{i=1}^{N}a_ix_i[n]$$
plug in and check if it 
$$
y[n] = \sum_{i=1}^{N}a_iy_i[n]
$$
> TODO: EXAMPLE
### Noise:
Signal that you don't want.















