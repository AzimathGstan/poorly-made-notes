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

$$|(5x-3)-2|\lt\epsilon\implies |5x-5|<\epsilon\implies5|x-1|\lt \epsilon \implies |x-1| \lt \frac{\epsilon}{5}$$ 
Thus we take $\delta=\frac{\epsilon}{5}$

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

## steps
step1: solve $|f(x)-L|\lt\epsilon$ to find an open interval containing $x_0$ on which the inequality holds for all x, $\neq x_0$
> $|f(x)-L \implies -\epsilon \lt f(x)-L\lt\epsilon \implies L - \epsilon \lt f(x) \lt L+\epsilon \implies xxx < xx <xx]$

step2: Find a value of $\delta$ that places $(x_0 - \delta, x_0 + \delta)$ inside $(a,b)$

## Ex: Find $\delta$ algebraically $$ \lim_{x\to 5}\sqrt{x-1}=2$$ find a $\delta\gt 0$ that works for $\epsilon=1$

## Sol:
1. solve $|\sqrt{x-1}-2| \lt \epsilon$ to find an open interval containing $x_0=5$
   $$\begin{align}
   &-1 \lt \sqrt{x-1} -2 \lt 1 \\
   \implies & 1 \lt \sqrt{x-1} \lt 3\\
   \implies & 1 \lt x-1 \lt 9 \\
   \implies & 2 \lt x \lt 10 \\
   \end{align}$$
2.  Find a $\delta\gt 0$  to place $(x_0-\delta, x_0+\delta)$ insides $(a,b)=(2,10)$ 
   Therefore, we take $\delta= 3(O) \text{ or } 5$
   Then $|x-5|\lt\delta\implies|\sqrt{x-1}-2|\lt 1$

## probs:
2-3 1, 7, 11, [15, 17, 31, 33, 57]

# 2-4 One sided-limits
$$ \lim{x\to c}
....
$$
it may still have a one-sided , like right-hand limit $$\lim_{x\to c^+}f(x) = L$$
or left-hand limit $$\lim_{x\to c^-}f(x) = L$$
## Ex: $f(x)=\frac{x}{|x|}$

![](attachs/Pasted%20image%2020240911152015.png)
$$ \lim_{x\to0}f(x) $$ does not exist. But 
$$ \lim_{x\to0^+}f(x) = 1 $$ and 
$$  \lim_{x\to0^-}f(x) = -1 $$
## Thm 6 (One-sided limit theorem)
$$ \lim_{x\to c}f(x) = L $$ 
when 

$$
\begin{align}
&\lim_{x\to c^-}f(x) = L \\
&\lim_{x\to c^+}f(x) = L 
\end{align}
$$ 

![](attachs/Pasted%20image%2020240911152341.png)
> append something from the phone
