# Homogeneous Differential Equations


## Example
let say $\frac{dx(t)}{dt}=x'=-vcos(\alpha)$, and $\frac{dy(t)}{dt}=y'=S-vsin(\alpha)$
Then 
$$\frac{dy}{dx}=\frac{dy/dt}{dx/dt}
=\frac{S-vsin(\alpha)}{-vcos(\alpha)}
=-\frac{S}{v}sec(\alpha)+tan(\alpha)
$$

Then we can solve this differential equation by integrating both sides:
$$\int dy = \int (-\frac{S}{v}sec(\alpha)+tan(\alpha))dx$$
$$y=-\frac{S}{v}sec(\alpha)x+ln|cos(\alpha)|$$

# Bernoulli Differential Equations

## Example
Let say we have a differential equation of the form:
$$\frac{dy}{dx}+P(x)y=Q(x)y^n$$
Then we can solve this differential equation by making a substitution $v=y^{1-n}$, then we have:
$$\frac{dv}{dx}=(1-n)y^{-n}\frac{dy}{dx}$$
$$\frac{dv}{dx}=(1-n)y^{-n}(P(x)y+Q(x)y^n)$$
$$\frac{dv}{dx}=(1-n)P(x)y^{1-n}+(1-n)Q(x)$$
$$\frac{dv}{dx}=(1-n)P(x)v+(1-n)Q(x)$$

Now we have a first order linear differential equation, we can solve this by using the integrating factor method.

# Riccati Differential Equations
> adding foreword

## Example
Consider the Riccati D.E. $y'=\frac{1}{x}y^2+\frac{1}{x}y-\frac{2}{x}$

1. Find one simple solution as $s(x)=1$
2. Use the change of variable $y(x)=s(x)+\frac{1}{z}=1+\frac{1}{z}$ to find the general solution of the Riccati D.E.

$$
\begin{aligned}
\implies -\frac{1}{z^2}z'...
\end{aligned}
$$
> adding from pic