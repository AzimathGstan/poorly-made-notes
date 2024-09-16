# Basic Operation on signals

## Two classes of operations

### On Dependent var $x(t)$
#### Amplitude scaling

$$y(t)=cx(t)$$

$$y[n]=cx[n]$$
#### Addition

$$y(t)=x(t)+v(t)$$

$$y[n]=x[n]+v[n]$$

#### Multiplication

$$y(t)=x(t)v(t)$$

$$y[n]=x[n]v[n]$$

#### Differentiation (continuous only))
$$y(t)=\frac{dx(t)}{dt}$$
#### Integration (continuous only)

$$y(t)=\int x(t)dt$$
### On independent var $t$
#### Time scaling

$$y(t)=x(at)$$

$$y[n]=x[kn]$$
#### Reflection
$$y(t)=x(-t)$$
#### Time shifting
$$y(t)=x(t-t_0)$$

### Example

> TODO
> order of this question
> -> + 3...

...

### Time scaling
#### Continuously: $y(t) = x(at)$ 
- $a \gt 1$, y(t) were compressed
- $0\lt1$ y(t) were expanded
![](attachs/Pasted%20image%2020240916172530.png)
#### Discrete: $y[n]=x[kn]$
> Where $k > 0$ . when $k \gt 1$ the values might be **lost**.

## Reflection
#### Continuously: $y(t)=x(-t)$
#### Discretely: $y[n]=x[-n]$
![](attachs/Pasted%20image%2020240916222859.png)


### Time shifting
#### Continuously: $y(t)=x(t-t_0)$
#### Discretely: $y[n]=x[n-n_0]$

![](attachs/Pasted%20image%2020240916172132.png)

### Precedence Rule
#### Continuously
Time-shifting > time-scaling

$$ v(t)=x(t-b)$$

$$ y(t)=v(at)=x(at-b)$$
####  Discretely

$$ y[n] = x[2n] $$ 
> Note That some values might be **lost** after compression in discrete signal

> Note That It is **IMPORTANT** that it compress based on the original(0) rather the point were it shift to.
## Elementary signals

- Exponential
- Sinusoid
- Step
- Impulse
- Ramp

### Exponential signal

$$x[n]=Br^n=Be^{}$$
![](attachs/Pasted%20image%2020240916223611.png)

#### Continuously $x(t)=Be^{at}$
- $a \gt 0$ exponential growth
- $a \lt 0$ exponential decay
- $a = 0$ constant
#### Discretely $x[n]=Br^n$
- $r \gt 1$ exponential growth
- $0 \lt r \lt 1$ exponential decay
- $r = 1$ constant

### Sinusoid signal $x(t)=Acos(\Omega t+\phi)$ 
- A: amplitude
- $\Omega$: frequency
- $\phi$: phase shift
- Period $T=2\pi/\Omega$
- Frequency $f=1/T=\Omega/2\pi$

#### Continuously

$$ x(t)=Acos(\Omega t+\phi)$$
#### Discrete

$$ x[n]=Acos(\Omega n+\phi)$$
- May not be periodic
- $x[n]$ is periodic if $x[n+N]=Acos(\Omega n + \Omega N + \phi)) = x[n]$ 

> TODO: needs more details 

### Relation between sinusoid and exponential -- Euler's formula

$$ e^{j\theta} = cos(\theta) + jsin(\theta)$$
Consider an exponential signal $Be^{j\omega t}$ where $B = Ae^{j\phi}$
$$ Be^{j\omega t} = Ae^{j\phi}e^{j\omega t} = A(cos(\omega t + \phi) + jsin(\omega t + \phi))$$

$$ s[n] = s[n+N] => cos(2\pi n) = cosj(n + N) $$
> TODO: needs more details
### Step function

#### Discrete

$$
u[n] = 
\begin{cases}
1 & t \geq 0 \\
0 & t \lt 0
\end{cases}
$$

#### Continuously
$$
u(t) = 
\begin{cases}
1 & t \gt 0 \\
0 & t \lt 0
\end{cases}
$$
> TODO: Provide a example from chap1-101

### **Impulse function**
Fundamental signal in signal processing
#### Discrete
![](attachs/Pasted%20image%2020240916225209.png)
#### Continuously 
![](attachs/Pasted%20image%2020240916225234.png)

> Make sure to draw an arrow instead of a line to show the impulse function in continuous signal

- Is an even function
$$\delta(t-t_0) = \delta(t_0-t)$$


