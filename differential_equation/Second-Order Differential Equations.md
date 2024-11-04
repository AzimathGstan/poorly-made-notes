An equation that contains a second derivative but no higher.
$$
F(x, y, y', y'') = 0
$$
For example
$$
\begin{aligned}
y''=x^3\\
xy''-cos(y)=e^x\\
y''-4xy'+y=2
\end{aligned}
$$

a function $\phi'(x)$ that satisfies the differential equation
$$
\implies F(x, \phi(x), \phi'(x), \phi''(x)) = 0
$$

For example...


# Def
$$
R(x)y''+P(x)y'+Q(x)y=F(x)
$$
and s(x) is a solution to the homogeneous equationonsider the linear second-order = D.E.


# Solution

## Particular Solution
$$  y''+p(x)y'+g(x)y=f(x) $$
### Theorem
Let $p, g, f$ be continuou. Let $x_0$ be a point in the solution domain. Let $A, B$ be real numbers. The IVP
$$
y''+p(x)y'+g(x)y=f(x); y(x_0)=A, y'(x_0)=B
$$
Then $y$ has a unique solution on some interval containing $x_0$ 

## Homogeneous Solution
$$ y''+p(x)y'+g(x)y=0 $$
When $f(x)=0$
$y''+p(x)y'+g(x)y=0$ is called the homogeneous equation.

Let $y_1(x)$ and $y_2(x)$ be two linearly independent solutions to the homogeneous equation. Then 
$$
y_h(x)=c_1y_1(x)+c_2y_2(x)
$$
is also a solution to the homogeneous equation.
#### proof
Substitute $y_h(x)$ back into the homogeneous equation
$$
\begin{aligned}
y_h''+p(x)y_h'+g(x)y_h&=0\\
c_1y_1''+c_2y_2''+p(x)(c_1y_1'+c_2y_2')+g(x)(c_1y_1+c_2y_2)&=0\\
c_1(y_1''+p(x)y_1'+g(x)y_1)+c_2(y_2''+p(x)y_2'+g(x)y_2)&=0\\
c_1(0)+c_2(0)&=0
\end{aligned}
$$


























