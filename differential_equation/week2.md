# Direction Fields
## The general first-order differential equation has the form$$F(x, y, y') = 0$$ Rewrite as $$y'=f(x,y)$$
a drawing of the plane, with short line segments of slope $f(x,y)$ drawn at selected point(x,y) is called a direction field.
![](attachs/Pasted%20image%2020240911103737.png)

## Examples
- 1.5 Consider the D.E $$y' = y^2$$ The general solution is $$y=-\frac{1}{x+k}$$![](attachs/Pasted%20image%2020240911104413.png)
- 1.6 Consider the D.E $$y'=sin(x*y)$$![](attachs/Pasted%20image%2020240911105201.png)

# Separable Equation
differential equation is called separable if it can be written as $$y'=A(x)B(y)$$
e.g.$$F(x,y,y')=0 \rightarrow y'=f(x,y)$$
$$ \frac{dy}{dx} = A(x)B(y) \rightarrow \frac{1}{B(y)}dy = A(x)dx \rightarrow \int\frac{1}{B(y)}dy = \int A(x)dx $$
This yields an equation in x,y and a constant of integration. 
This equation implicitly defines the general solution $y(x)$, 
for which may or may not be explicitly solved

### Example
- 1.7 Consider $$y' = \frac{y^2e^-x}{B(y)A(x)} \rightarrow \frac{dy}{dx}=y^2e^{-x} \rightarrow \frac{1}{y^2}dy=e^{-x}dx, y\neq0 \rightarrow \int\frac{1}{y^2}dy=\int e^{-x}dx\rightarrow-\frac{1}{y}=-e^{-x}+C\rightarrow y=\frac{1}{e^{-x}-C}, y\neq0 \text{and singular sol} y=0$$
singular solution can not be generated from $y=\frac{1}{e^x-C}$

### Example 1.8
Consider $$x^2y'=1+y\implies y'=(1+y)\frac{1}{x^2}$$
recall that $y'=\frac{dy}{dx}$ and $y'=A(x)B(y)$, so we can rewrite as 
$$
\frac{dy}{dx}=(1+y)\frac{1}{x^2} \implies \frac{1}{1+y}dy=\frac{1}{x^2}dx
$$
then integrate both side
$$
\int\frac{1}{1+y}dy=\int\frac{1}{x^2}dx \implies ln|1+y|=-\frac{1}{x}+C
$$
then solve for y
$$\begin{align}
&|1+y|=e^{-\frac{1}{x}+C} \\
\implies& |1+y| = e^{-\frac{1}{x}}e^C \\
\implies& |1+y| = Ae^{-\frac{1}{x}}; A=e^C\\
\implies& 1+y = \pm Ae^{-\frac{1}{x}}\\
\implies& 1+y = Be^{-\frac{1}{x}}; B=\pm A\\
\implies& y=-1+Be^{-\frac{1}{x}}\\
\end{align}
\begin{cases}
y=-1+Be^{-\frac{1}{x}} & \text{for } x\neq0\\
y=0 & \text{for } x=0
\end{cases}
$$
> When $x=0$ the solutions need a boundary condition to determine the value of y, here just copied from class ppt

### Example 1.9
Consider $$y'=y^2e^{-x}, y(1)=4$$
$$\begin{align}
&\frac{dy}{dx}=y^2e^{-x}\\
\implies& \frac{1}{y^2}dy=e^{-x}dx\\
\implies& \int\frac{1}{y^2}dy=\int e^{-x}dx\\
\implies& -\frac{1}{y}=-e^{-x}+C\\
\implies& y=\frac{1}{e^{-x}+C}\\
\end{align}$$
idk
$$\begin{cases}
y=\frac{1}{e^{-1}+C}, y\ne0\\ 
y= 0 ? 
\end{cases}$$
then solve for C using the initial condition $y(1)=4$
$$\begin{align}
&4=\frac{1}{e^{-1}+C}\\
\implies& 4(e^{-1}+C)=1\\
\implies& 4e^{-1}+4C=1\\
\implies& 4C=1-4e^{-1}\\
\implies& C=\frac{1-4e^{-1}}{4}\\
\implies& C=\frac{1}{4}-e^{-1}\\
\end{align}$$
>Could be -C here

then plug in C to get the solution
$$\begin{align}
&y=\frac{1}{e^{-x}+\frac{1}{4}-e^{-1}}\\
\implies& y=\frac{1}{e^{-x}+\frac{1}{4}-e^{-1}}\\
\end{align}$$

### Example 1.10
Consider $$y'=y\frac{(x-1)^2}{y+3}, y(3)=-1$$
$$\begin{align}
&\frac{1}{y}y'=\frac{(x-1)^2}{y+3}\\
\implies& \frac{y+3}{y}dy=(x-1)^2dx\\
\implies& \int\frac{y+3}{y}dy=\int(x-1)^2dx\\
\implies& \int(1+\frac{3}{y})dy=\int(x-1)^2dx\\
\implies& y+3ln|y|=\frac{(x-1)^3}{3}+C\\
\end{align}$$
then solve for C using the initial condition $y(3)=-1$
$$
\begin{align}
&-1+3ln|-1|=\frac{(3-1)^3}{3}+C\\
\implies& -1+3ln1=\frac{2^3}{3}+C\\
\implies& -1+0=\frac{8}{3}+C\\
\implies& C=-1-\frac{8}{3}\\
\implies& C=-\frac{11}{3}\\
\end{align}
$$
then plug in C to get the solution

# Linear Differential Equation
A first-order D.E.  is linear if it has the form $$y'(x)+p(x)y(x)=q(x)$$
assume $p(x)$ and $q(x)$ are continuous on an interval $I$ 
$\implies$ Multiply the D.E. by $e^{\int p(x)dx}$ 
$\implies$ $e^{\int p(x)dx}y'(x)+p(x)e^{\int p(x)dx}y(x)=q(x)e^{\int p(x)dx}$ 
$\implies$ $\frac{dx}{dy}(e^{\int p(x)dx}y(x))=q(x)e^{\int p(x)dx}$ 
>$\frac{dx}{dy}$ is the product rule of differentiation  
$\implies$ $\frac{dy}{dx}A(x)B(x)=A'(x)B(x)+A(x)B'(x)$ 

$\implies$ $e^{\int p(x)dx}y(x)=\int q(x)e^{\int p(x)dx}dx+C$ 
$\implies$ $y(x)=e^{-\int p(x)dx}(\int q(x)e^{\int p(x)dx}dx+C)$

### Example 1.14
Consider $$y'+y=sin(x)$$
$$\begin{align}
&p(x)=1, q(x)=sin(x)\\
\implies& y=e^{-\int p(x)dx}\\
\implies& y=e^{-\int 1dx} = e^{x+c} = e^xe^c = Ae^x\\
\end{align}$$
> $A$ is an arbitrary constant, maybe ignore ?

Multiply the D.E. by $e^x$
$$\begin{align}
&e^xy'+e^xy=sin(x)e^x\\
\implies& \frac{dx}{dy}(e^xy)=sin(x)e^x\\
\implies& e^xy=\int sin(x)e^xdx+C\\
\implies& y=e^{-x}(\int sin(x)e^xdx+C)\\
\end{align}$$

### Example 1.15
$$\begin{align}
&y'+\frac{1}{x}y=3x^2, p(x)= \frac{1}{x} \\
\implies& y=e^{\int p(x)dx}=e^{\int \frac{1}{x}dx}=e^{ln|x|}=|x|=\pm x\\
&\text{Multiply the D.E. by } x\\ 
&\implies xy'+y=3x^3\\
&\implies \frac{d}{dy}(xy)=3x^3\\
&\implies xy=\int 3x^3dx+C = \frac{3}{4}x^4+C\\
&\implies y=\frac{3}{4}x^3+\frac{C}{x}\\
\end{align}$$
## Integrals not able to be evaluated
consider the D.E. $$y'+xy=2$$
$$\begin{align}
&p(x)=x, q(x)=2\\
&\implies e^{\int p(x)dx} = e^{\int x dx} = e^{\frac{x^2}{2} }\\
&\text{Multiply the D.E. by } e^{\frac{x^2}{2}}\\
&\implies e^{\frac{x^2}{2}}y'+xe^{\frac{x^2}{2}}y=2e^{\frac{x^2}{2}}\\
&\implies \frac{d}{dx}(e^{\frac{x^2}{2}}y)=2e^{\frac{x^2}{2}}\\
&\implies e^{\frac{x^2}{2}}y=\int 2e^{\frac{x^2}{2}}dx+C\\
&\implies y=e^{-\frac{x^2}{2}}(\int 2e^{\frac{x^2}{2}}dx+C)\\
\end{align}$$










