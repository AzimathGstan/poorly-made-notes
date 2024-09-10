## functions
- Trigonalmetric Functions : $sin(x) cos(x) tan(x)$
- Exponential Functions : $f(x)=a^x$\
=> domain: $(-\infty, +\infty)$\
=> range: $(0, +\infty)$

- Logarithmic Functions : $f(x)=log_a(x)$ where $a>0, a\neq 1$\
=> domain: $(-\infty, +\infty)$\
-> range: $(-\infty, +\infty)$

### questions? 
1-1: 3, 5, 7, 25, 35, 45, 51

> For training purpose, maybe will be included in next exam.

# 1-2 Combining Functions
## shifting and scaling functions
If $f(x)$, $g(x)$ are functions, then for every $x\in D(f) \cap D(g)$, 
the following functions are defined:

- $f(x)+g(x)$
- $f(x)-g(x)$
- $f(x)*g(x)$
- $f(x)/g(x)$

> Notice that Domain change after these operations,
> Thus these are the new functions.
> D stand for domain
> R stand for range

### Example
$f(x)=\sqrt{x}, g(x)=\sqrt{1-x}$

$D(f)=[0, +\infty) , D(g)=(-\infty, 1]$

$(f+g)(x)=f(x)+g(x)=\sqrt{x}+\sqrt{1-x}$, Domain: $[0, 1]$

$(f/g)(x)=\frac{\sqrt{x}}{\sqrt{1-x}}$, Domain: $[0, 1)$

## Composite Functions
If $f(x), g(x)$ are functions, the composite function
$f \circ g(x) = f(g(x))$ 
The domain of $f \circ g$ consists of x in $D(g)$ for 
which $g(x)$ lies in the domain of f

### diagram of 

$f\circ g$

![$f \circ g$](./composite.png)

### example 
$y=\sqrt{1-x^2}$ => Take f(x)=$\sqrt{x}$, $g(x)=1-x^2$
=> f(g(x))=$\sqrt{1-x^2}$
=> Domain: $[-1, 1]$
-> Range: $[0, 1]$

## Shift formaulas 
- Vertical shift: \
    $y=f(x)+c$ => shift c units up
- Horizontal shift: \
    $y=f(x+c)$ => shift c units left
- Vertical scaling: \
    $y=cf(x)$, if ($c >  1$) => stretch vertically by a factor of c \
    $y=\frac{f(x)}{c}$, if ($c > 1$) => compress vertically by a factor of c \
- Horizontal scaling: \
- $y=f(cx)$, if ($c > 1$) => compress horizontally by a factor of c \
- $y=f(\frac{x}{c})$, if ($c > 1$) => stretch horizontally by a factor of c

## reflection
- $y=-f(x)$ => reflect across x-axis
- $y=f(-x)$ => reflect across y-axis

## Example
$f(x)=x^4 - 4x^3 + 10$ =>\
Compress $f(x)$ horizontally by a factor of 2, 
follow by a reflection across the y-axis

whats the new function ?\
ANS: $f(-2x) = (-2x)^4 -4(-2x)^3 + 10$
$= -16x^4 + 32x^3 + 10$

# 1-3 Trigonometric Functions

## degrees vs radians
($\pi$ = 180 deg, 2$\pi$ = 360 deg)

## functions
- $sin(\theta) = \frac{y}{r}$
- $cos(\theta) = \frac{x}{r}$
- $tan(\theta) = \frac{y}{x}$

## trigonometric identities
- $sin^2(\theta) + cos^2(\theta) = 1$
- $tan(\theta) = \frac{sin(\theta)}{cos(\theta)}$
- $cot(\theta) = \frac{cos(\theta)}{sin(\theta)}$
- $sec(\theta) = \frac{1}{cos(\theta)}$
- $csc(\theta) = \frac{1}{sin(\theta)}$
- $tan(\theta) = \frac{sin(\theta)}{cos(\theta)}$
- $cot(\theta) = \frac{cos(\theta)}{sin(\theta)}$

## definition of periodic functions
$f(x)$ is periodic if there is a positive P such that 
$f(x+P) = f(x), \forall x$

> $\forall$ stands for "for all"

The smallest such valve of P is the period of $f(x)$

### Example
- $f(x) = sin(x)$, $p = 2\pi$ 
- $f(x)=cos(x)$, $p=2\pi$
- $f(x)=tan(x)$, $p=\pi$

$f(x)=tan(x)$ is an **odd** functions

## more trigonometric identities
Addition: $cos(A+B)=cosAcosB-sinAsinB$

$cos^2(\theta) = \frac{1+cos(2\theta)}{2}$

## the law of consines

$c^2 = a^2 + b^2 - 2abcos(\theta_C)$

## Transformation of graph

Given $y=f(x)$ $y=af(b(x+c))+d$\
Ex: $f(x)=Asin[\frac{2\pi}{B}(x-c)] + D$


# Chap2 Limits and Continuity 

## 2-1: Rates of change and tangents to curve
Average rate of change of $f(x)$ over ab interval $[x_1, x_2]$ is \
=> $\frac{\Delta y}{\Delta x} = \frac{f(x_1)-f(x_2)}{x_1-x_2}$\
=> $\frac{f(x_1+h) - f(x_1)}{h}$






