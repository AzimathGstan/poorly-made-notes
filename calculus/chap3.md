# Differentiate 

## Def
Slope m = 
$$
\lim_{h \to 0} \frac{f(x+h) - f(x)}{h}
$$
or 
$$
\lim_{x \to a} \frac{f(x) - f(a)}{x-a}
$$

called $f'$

## Ex: $y=|x|$ is not differentiable at $x=0$
$$
\lim_{h \to 0^+} \frac{|h| - 0}{h} = \lim_{h \to 0^+} \frac{h}{h} = 1
$$
$$
\lim_{h \to 0} \frac{|h| - 0}{h} = \lim_{h \to 0^-} \frac{-h}{h} = -1
$$

Therefore A differentiable function must be continuous
But a continuous function is not necessarily differentiable

pf: $f'(x)$ exists $\implies \lim_{h\to c} f'(c)$ exists

If the differential result in $\pm \infty$, then the function is not differentiable
But its tegent line is vertical
