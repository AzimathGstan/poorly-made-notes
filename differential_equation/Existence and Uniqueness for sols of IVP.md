## Example
Consider the IVP
$$ y'=2y^{\frac{1}{2}};  y(0)=-1 $$
$$
\begin{aligned}
\implies \frac{dy}{dx}&=2y^{\frac{1}{2}}\\
\implies \frac{dy}{y^{\frac{1}{2}}}&=2dx\\
\implies \int y^{-\frac{1}{2}}dy&=\int 2dx\\
\implies 2y^{\frac{1}{2}}&=2x+c\\
\implies y^{\frac{1}{2}}&=x+c\\
\implies y&=(x+c)^2
\end{aligned}
$$
then we plug IC to find $c=-1$ $y(0)=(0+c)^2=-1$ which is impossible, so there is no solution to the IVP.
> complex ?


## Example 2
Consider the IVP
$$
y'=2y^{\frac{1}{2}};  y(2)=0
$$
One solution is $y=0$ for all 0 and $y=x^2$ for $x>0$. But the solution is not unique.

## Theorem
Let $f$ and $\frac{\partial f}{\partial y}$ be continuous for all $(x, y)$ in a closed rectangle $R$ of the $xy$-plane centered at $(x_0, y_0)$. Then there exists a positive number $h$ such that the ivp $y'=f(x, y); y(x_0)=y_0$ has a unique solution over (x_0-h, x_0+h)

### Example
Consider the IVP
$$ y'=y^2; y(0)=n $$
The solution is $y(x)=-\frac{1}{x+\frac{1}{n}}$
which is not continuous at $x=-\frac{1}{n}$, so the theorem does not apply.
which us valid on $(0-\frac{1}{n}, 0+\frac{1}{n}$ for x since f and $\frac{\partial f}{\partial y}$ are continuous on this interval.










