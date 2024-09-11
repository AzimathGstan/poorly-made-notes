let $f(x)$ be defined on an open interval (containing $x_0$), except for possibly at $x_0$. 
If for every number $\epsilon \gt 0$, there exist a number $\delta \gt 0$, such that for all $x$, 
$$0 \lt |x - x_0| \lt \delta \implies |f(x) - L| \lt \epsilon \implies \lim_{x\to x_0}f(x)=L$$
> $|f(x) - f(x_0)| \lt \epsilon$ can be seen as  $x_0-\delta \lt x \lt x_0+\delta$.
>$|f(x) - L| \lt \epsilon$ can be seen as $L-\epsilon \lt f(x) \lt L+\epsilon$
![](attachs/Pasted%20image%2020240911133928.png)

$$\forall\epsilon\gt 0, \exists\delta \gt 0 \mid \forall x, 0 \lt |x-x_0|\lt \delta\implies |f(x)-L| \lt \epsilon \implies \lim_{x\to x_0}f(x)=L$$
> $\forall$ - for all
> $\exists$ - exists

### Ex: Show that $$ \lim_{x\to 1}(5x-3)=2$$ by using the precise definition

$$
\forall\epsilon \gt 0, \exists x,
\forall x, 0 < |x-x_0| < \delta \implies |f(x)-L| < \epsilon
$$
$$x_0=1, f(x)=5x-3, L=2$$
$$ \forall\epsilon\gt 0, \exists\delta(...\epsilon), s.t. \forall x, 0 \lt |x-x_0| \lt \delta \implies |f(x)-L| \lt \epsilon
$$
$$|(5x-3)-2|\lt\epsilon\implies |5x-5|<\epsilon\implies5|x-1|\lt \epsilon \implies |x-1| \lt \frac{\epsilon}{5}$$ Thus we take $\delta=\frac{\epsilon}{5}$
$$ \forall\epsilon\gt 0, \exists\delta=\frac{\epsilon}{5}$$
when $$\begin{align} 
&0\lt|x-1|\lt\delta=\frac{\epsilon}{5} \implies \\
&|x-1|\lt \frac{\epsilon}{5}\implies \\
&5|x-1|\lt\epsilon\implies \\
&|5x-5|\lt\epsilon\implies \\
&|(5x-3)-2|\lt\epsilon \implies\\
&|f(x)-2|\lt\epsilon \implies\\
&|f(x)-L|\lt\epsilon \implies\\
&\lim_{x\to1}(5x-3)=2
\end{align}$$
> It forms $f(x)-L$ in the end. where L is the limit











