# Basic Operation on signals

## Two classes of operations

- On Dependent variables e.g $x(t)$
	- Amplitude scaling
	
	  $$\begin{align}
		  &y(t) = cx(t)\\
		  &y[n] = cx[n] \\
		  \end{align}$$ 
	- Addition
    $$\begin{align}
      &y(t) = x(t) + v(t)\\
      &y[n] = x[n] + v[n] \\
      \end{align}$$ 
	
	- Multiplication
    $$\begin{align}
      &y(t) = x(t)v(t)\\
      &y[n] = x[n]v[n] \\
      \end{align}$$ 
	
	- Differentiation -- for continuous only
	
	- Integration -- for continuous only
- On independent variables e.g. $t$ 
	- Time scaling
	- Reflection
	- Time shifting

### Example

	order of this question
	-> + 3...

...

### Time scaling
#### Continuously: $y(t) = x(at)$ 
- $a \gt 1$, y(t) were compressed
- $0\lt1$ y(t) were expanded

		Perhaps adding some figure here 

#### Discrete: ... $a \gt 1$
		sample might be lose after compress

### Time shifting
#### Continuously: $y(t)=x(t-t_0)$
#### Discretely: ...

		perhaps import some figure from ppt


### Precedence Rule

time-shifting -> time-scaling

$$ v(t)=x(t-b)$$	$$ y(t)=v(at)=x(at-b)$$

	Note That It is IMPORTANT that it compress based on the original(0) rather the point were it shift to. That so called precedence rule
	

when comes to discrete $$ y[n] = x[2n] $$ its important to know that some sample that were not integer will be discarded

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


