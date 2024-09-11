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
