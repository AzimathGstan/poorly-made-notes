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

	order of this question
	-> + 3...

...

### Time scaling
#### Continuously: $y(t) = x(at)$ 
- $a \gt 1$, y(t) were compressed
- $0\lt1$ y(t) were expanded
![](attachs/Pasted%20image%2020240916172530.png)
#### Discrete: $y[n]=x[kn]$
Where $k > 0$ . when $k \gt 1$ the values might be lost.

## Reflection
> TODO

### Time shifting
#### Continuously: $y(t)=x(t-t_0)$
#### Discretely: $y[n]=x[n-n_0]$

![](attachs/Pasted%20image%2020240916172132.png)

### Precedence Rule

time-shifting -> time-scaling

$$ v(t)=x(t-b)$$   
$$ y(t)=v(at)=x(at-b)$$

	Note That It is IMPORTANT that it compress based on the original(0) rather the point were it shift to. That so called precedence rule
	

when comes to discrete  
$$ y[n] = x[2n] $$ its important to know that some sample that were not integer will be discarded

## Elementary signals

- Exponential
- Sinusoid
- Step
- Impulse
- Ramp

#### Exponential signal			
$$x[n]=Br^n=Be^{}$$
		Fill this out according to the ppt

for continusly
for descrete $e^{\Omega n}$

### Sinusoid signal

#### Discrete
$$ x[n]=Acos(\Omega n+\phi)$$
- May not be periodic
- $x[n]$ is periodic if $x[n+N]=Acos(\Omega n + \Omega N + \phi)) = x[n]$ 
	sin(t) = 2pi
	sin(5 * pi * n) = 2/5

The m in the ppt might need to be found by oneself
===ask this ? === 

### relation between sinusoid and exponential 
the eular formuler

$$ s[n] = s[n+N] => cos(2\pi n) = cosj(n + N) $$

### step function
> Finishing this from ppt

### impulse function
#### Discrete
important for discrete.
Any Discrete function can be describe by scaling or shifting impulse function
> TODO pic
#### Continuously 

===make sure draw an arrow upward instead of drawing a circle or a line with 1===
>TODO pic

- Is an even function
- its shifting:
- its time-scaling --notice that u might need add abs:
> todo ppt, notice the importance of the shifting property

$$\delta(t-t_0) = \delta(t_0-t)$$
> maybe a pic ?
> 


