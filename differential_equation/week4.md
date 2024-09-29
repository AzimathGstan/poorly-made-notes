## Example
consider
$$
(x^2+3xy)+(4xy+2x)y'=0
$$
$$\begin{align}
\implies \frac{2M}{2y}=3x \neq \frac{2N}{2x}=??? 
\end{align}$$
??? in phote

## Example
consider
$$
(e^xsin(y)-2x)+(e^xcos(y)+1)y'=0
$$
$$
\frac{\partial M}{\partial y} = e^x cos(y) = \frac{\partial N}{\partial x} = e^x cos(y)
$$
Therefore the given equation is exact.

$$ \begin{cases}
\frac{\partial u}{\partial x} = N = e^x sin(y) - 2x \\
\frac{\partial u}{\partial y} = N = e^x cos(y) + 1
\end{cases}
$$
$$\implies^{\int\partial x}_{\int\partial y} \begin{cases}
\phi = e^xsin(y)-x^2+g(y)\\
\phi = e^xsin(y)+y+h(x)
\end{cases}
$$
$$\begin{align}
&\phi=e^xsin(y)+y-x^2\\
&\implies \phi=C\\
&\implies e^xsin(y)+y-x^2=C
\end{align}
$$

# Intergrating Factors

For not exact D.E., we ca n try ti multiply the equation by a nonzero function $\mu(x,y)$$ to make it exact. The function $$\mu(x,y)$$ is called an integrating factor.

### Example
$$
(y^2-6xy ) + (3xy-6x^2)y'=0
$$
is not exact
let multiply the D.E. with an integrating factor 
$$\mu(x,y) = y \neq 0$$
Then
$$\begin{align}
&(y^3-6x^2y) + (3xy^2 - 6x^2y)y' = 0\\
\implies& \frac{\partial M}{\partial y} = 3y^2-12xy = \frac{\partial N}{\partial x} = 3y^2-12xy \\
\implies &\text{The given D.E. is exact} \\
\implies &\begin{cases}
\frac{\partial \phi}{\partial x} =  y^3-6x^2y \\
\frac{\partial \phi}{\partial y} =  3xy^2-6x^2y
\end{cases}

\end{align}
$$
Therefore
$$
\phi = \int y^3-6x^2y dx = y^3x-2x^3y + g(y)
$$

## Definition
let $M(x,y)dx + N(x,y)$ be defined on a region $R$ of the
plane. Then $\mu(x,y)$ is an interfrating factor for $M+Ng'=0$ if 
$\mu(x,y) \neq 0$ for all $(x,y) in $R$ and $(\mu M)+(\mu N)y'=0$ is exact


## Finding an integrating factor
Since $(\mu M)+( \mu N)y'=0$ is exact
$\implies \frac{\partial (\mu M)}{\partial y} = \frac{\partial (\mu N)}{\partial x}$
Then we can find out the integrating factor 

## Example
$$
(x-xy)-y'=0
$$
Check exactness
$$
M(x,y) = x-xy \quad N(x,y) = -1
$$
$$
\frac{\partial M}{\partial y} = -x \neq \frac{\partial N}{\partial x} = 0
$$
Not exact...

Let multiply the D.E. by an integrating factor $\mu(x,y)$
$$
\implies \mu(x,y)(x-xy) - \mu(x,y)y'=0
$$
Move y' to the right side, and partial each
$$
\begin{align}
\frac{\partial (\mu(x,y) (x-xy))}{\partial y} = \frac{\partial (\mu (x,y)N)}{\partial x}
\end{align}
$$
> is + or - on right side

diff andsimplefy
$$
\begin{align}
\frac{\partial\mu(x-xy)}{\partial y} + \mu(-x) = - \frac{\partial \mu}{\partial x}
\end{align}
$$
Assume $\mu(x,y) = \mu(x)$ so that $\frac{\partial \mu(x,y)}{\partial y} = \frac{\partial \mu(x)}{\partial y} = 0$
$$
\begin{align}
\implies -\mu x = -\frac{\partial \mu}{\partial x}\\
\implies \mu x = \frac{\partial \mu}{\partial x}\\
\end{align}
$$
$$
\begin{align}
\implies \int \frac{1}{\mu}d\mu = \int xdx\\
\implies ln|\mu| = ln|x| + \frac{1}{2}x^2\\
\implies \mu = e^{\frac{1}{2}x^2}x
\end{align}
$$

$$ \begin{align}
\implies& \mu=\pm e^{\frac{1}{2}x^2}\\
\implies& (x-2y)e^{\frac{1}{2}x^2}-e^{\frac{1}{2}x^2}y'=0\\
&\begin{cases}
\frac{\partial \phi}{\partial x} = (x-xy)e^{\frac{x^2}{2}}\\
\frac{\partial \phi}{\partial y} = -e^{\frac{x^2}{2}}
\end{cases}\\
\implies& \phi = (1-y)e^{\frac{x^2}{2}} + e^{\frac{x^2}{ }}\\
\implies& \phi = (1-y)e^ex62...= C\\
\end{align}
$$


## Example 
Consider
$$
\frac{2xy}{y-1}-y'=0
$$
This is separable but not exact
then multiply by an integrating factor
$$\begin{align}
\mu(x,y) = \frac{y-1}{y}, y\neq 0\\
\implies \mu(\frac{2xy}{y-1})-\mu y' = 0\\
\implies 2x - \frac{y-1}{y}y' = 0\\
\end{align}$$
As one can see, it just like separable D.E. 
Therefore separable D.E. is a special case of exact D.E.

## Example
Consider
$$
(y=3)-xy'=0
$$
















