## Causality
causal when present value of the output signal depends only on present or past value of input signal.

##### Example:

$$ y[n]=x[n-1]+x[n]+x[n+1] $$

which required future value of input signal, so it is not causal.

## Invertibility
A system is invertible if input signal can be recovered from output signal'.
In mathematical terms 

$$
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
### Ex:
#### Time Invariance
Consider a inductor that is

$$
y_1(t) = \frac{1}{L}\int_{-\infty}^{t}x_1(\tau)d\tau
$$

Then we try to shift the input of the system $y_2$  by changing the $t$ in x to $t-t_0$

$$
y_2(t) = \frac{1}{L}\int_{-\infty}^{t}x_2(\tau-t_0)d\tau
$$

while we delay whole system $y_1$ by $t_0$.

$$
y_1(t-t_0) = \frac{1}{L}\int_{-\infty}^{t-t_0}x_1(\tau-t_0)d\tau
$$

Then we can see that $x_2(\tau-t_0) = x_1(\tau-t_0)$, so the system is time invariant.
> Still there are some question that whether $\int_{-\infty}^{t}x_1(\tau)d\tau = \int_{-\infty}^{t-t_0}x_1(\tau)d\tau$ differ or not, might better to check it.



#### Time variance
Consider an thermistor that is

$$
y_1(t) = \frac{x_1(t)}{R(t)}
$$

Then we try to shift the input of the system $y_2$  by changing the $t$ in x to $t-t_0$


$$
y_2(t) = \frac{x_2(t-t_0)}{R(t)}
$$

while we delay whole system $y_1$ by $t_0$.

$$
y_1(t-t_0) = \frac{x_1(t-t_0)}{R(t-t_0)}
$$

Then we can see that $R(t-t_0) \neq R(t)$, so the system is not time invariant.
> The key of checking time variance is to plug $t-t_0$ into $t$ and see to see if its equal to the original system.



## Linearity
One can break the input signal into multiple signal, then apply the system to each signal and sum them up to get the output signal. Which will be the same as applying the system to the original signal.
Therefore it need to be satisfied by two properties:
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
### Checking Linearity
Consider $y(t)=x(t)x(t-1)$, then i can plug $x(t)=\sum_{i=1}^{N}a_ix_i(t)$ into the system to see if it satisfy the linearity.

$$ 
\begin{align}
y(t)=&\sum_{i=1}^{N}a_ix_i(t)\sum_{i=1}^{N}a_jx_j(t-1) \\
=&\sum_{i=1}^{N}\sum_{j=1}^{N}a_ia_jx_i(t)x_j(t-1) \\
\neq &\sum_{i=1}^{N}a_iy_i(t)
\end{align}
$$

Therefore the system is not linear.

> Maybe add more example ?

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
assume 

$$
y_i[n]=H\{x_i[n]\}
$$

then let 

$$
x[n] = \sum_{i=1}^{N}a_ix_i[n]$$

plug in and check if it 

$$
y[n] = \sum_{i=1}^{N}a_iy_i[n]
$$
### Noise:
Signal that you don't want.















