# Exact D.E.
Any first-order D.E. that can be written in the form of 
$$ \begin {align}
&y' = f(x,y) \\ 
\implies& -f(x,y)+y' = 0\\
\implies& M(x,y)+N(x,y)y'=0\\
\implies& 
\begin{cases}
M(x,y) = -f(x,y)\\
N(x,y) = 1
\end{cases}

\end {align} $$

If there exists a function $\phi(x,y)$ such that 
$$ \begin {align}
&\frac{\partial \phi}{\partial y} = M(x,y)\\
&\frac{\partial \phi}{\partial x} = N(x,y)
\end {align} $$
And $\frac{d}{dx}\phi(x,y) = 0$, which implies that ...
then the D.E.'s solution is $\phi(x,y) = C$ where $C$ is a constant.
> $\frac{\partial \phi}{\partial y} + \frac{\partial \phi}{\partial x}\frac{dy}{dx} = 0 \implies \frac{\partial \phi}{\partial y} + \frac{\partial \phi}{\partial x}\frac{\partial y}{\partial x} = 0$ 

## Ex
Consider the D.E. 
$$
y'=\frac{2xy^3+2}{3x^2y^2+8e^{4y}}
$$
Which is neither separable nor linear. 
Rewrite the D.E. as
$$ \begin{align}
&(3x^2y^2+8e^{4y})y'+(2xy^3+2)=0\\
&\implies M(x,y)=3x^2y^2+8e^{4y}\\
&\implies N(x,y)=2xy^3+2

\end{align} $$
Since there exists a function $\phi(x,y)=x^2y^3+2x+2e^{4y}$such that 
$$ \begin{align}
&\frac{\partial \phi}{\partial y} = 2xy^3+2 = M(x,y)\\
&\frac{\partial \phi}{\partial x} = 3x^2y^2+8e^{4y}= N(x,y)
\end{align} $$
Then the solution to the D.E. is $\phi(x,y)=C$ where $C$ is a constant.
$$
x^2y^3+2x+2e^{4y}=C
$$

> some checks here


## Potential Functions
a function $\phi(x,y)$ is called a potential function for the D.E. $M(x,y)+N(x,y)y'=0$ on a region R of the plane
if for each $(x,y)$ in the $R$
$$
\frac{\partial \phi}{\partial x} = M(x,y) \text{ and } \frac{\partial \phi}{\partial y} = N(x,y)
$$

## Exact Differential Equation
when a potential function exists on a region $R$ for the D.E.
$M+Ny'=0$ then the D.E. is called an exact D.E. then this equation is said to be exect on $R$ 
$\phi(x,y)$ exists $implies$ the D.E. is exact.

## How to find potential function
$$
M+Ny'=(2xy^3+2)+(3x^2y^2+8e^{4y})y'=0
$$
assume that D.E. is exact $\implies$ $\phi(x,y)$ exists
$\implies$ $\frac{\partial \phi}{\partial x}= M = 2xy^3+2$ and $\frac{\partial \phi}{\partial y} =N= 3x^2y^2+8e^{4y}$

$$
\begin{align}
\frac{\partial \phi}{\partial x} &= 2xy^3+2\\
\phi(x,y) &= \int 2xy^3+2 dx = x^2y^3+2x+h(y)\\
\frac{\partial \phi}{\partial y} &= 3x^2y^2+8e^{4y} + h'(y)\\
\frac{\partial}{\partial y}(x^2y^3+2x+h(y)) &= 3x^2y^2+h'(y) = 3x^2y^2+8e^{4y}\\
\implies h'(y) &= 8e^{4y}\\
\implies h(y) &= 2e^{4y}+C
\end{align}
$$

$$ \begin{align}
\frac{\partial \phi}{\partial y} &= 3x^2y^2+8e^{4y} = N\\
\frac{\partial \phi}{\partial x} &= 2xy^3+2 = M \\
N \xrightarrow{\int} \phi(x,y) &= x^2y^3+2e^{4y}+h(x) \\
\xrightarrow{\frac{\partial}{\partial x}}& 2xy^3+0+h'(x)\\
\end{align}$$
then $h'(x)=2$ $\implies$ $h(x)=2x+C$, finally $\phi(x,y)=x^2y^3+2e^{4y}+2x$
Then because $\frac{\partial \phi}{\partial x} = M$ and $\frac{\partial \phi}{\partial y} = N$, and $M+Ny'=0$ , then $\phi$ should be some sort of constant.  therefore $x^2y^3+2e^{4y}+2x=C$


### Ex
Consider $y+y'=0$
assume the D.E. is exact $\implies$ $\phi(x,y)$ exists
$$\begin{cases}
M(x,y) = y\\
N(x,y) = 1
\end{cases}$$
$$
\begin{align}
\frac{\partial \phi}{\partial x} &= y\\
\phi(x,y) &= \int y dx = xy+h(y)\\
\frac{\partial \phi}{\partial y} &= x+h'(y)\\
h'(y) &= -x + y\\ 
\text{impossible ?}
\end{align}
$$

## Test for exactness
Suppose se $M(x,y)$ and $N(x,y)$ , $\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$ are continuous for all $(x,y)$ in a rectangle $R$ is t he plane, then the D.E. $M(x,y)+N(x,y)y'=0$ is exact if and only if $\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$ 

#### proof ?
If $M+Ny'=0$ is exact, then there is a potential function $\phi$ such that $\frac{\partial \phi}{\partial x} = M$ and $\frac{\partial \phi}{\partial y} = N$ 
$$
\implies \frac{\partial M}{\partial y} =\frac{\partial}{\partial y} \frac{\partial \phi}{\partial x} = \frac{\partial}{\partial x} \frac{\partial \phi}{\partial y} = \frac{\partial N}{\partial x}
$$

$$\begin{align}
&\phi(x,y) = \int^{x}_{x_0} M(\xi, y_0 ) d\xi = \int^y_{y_0} N(x, \eta) d\eta\\
&\frac{\partial \phi}{\partial y} = N(x,y) \text{ will be automatically satisfied}\\
&\implies \frac{\partial}{\partial x}\int^x_{x_0} M(\xi, y_0)d\xi + \frac{\partial}{\partial y}\int^y_{y_0} N(x, \eta) d\eta\\
&= M(x,y_0)+\int^y_{y_0} \frac{\partial}{\partial x} N(x,\eta) d\eta \\
&= M(x,y_0)+\int^y_{y_0} \frac{\partial}{\partial \eta} M(x,\eta) d\eta \\
&= M(x,y_0)+M(x,y)-M(x,y_0) = M(x,y)

\end{align}$$



















	
