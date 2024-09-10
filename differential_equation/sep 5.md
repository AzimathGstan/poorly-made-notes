# Preliminary Concepts

## Differetial Equation

* Definition
    a differentia; equation is an equation that contains one or more derivatives
    - $y''(x) + y(x) = 4sin(3x)$
    - $\frac{d^4\omega(t)}{dt^4} - (\omega(t))^2 = e^-t$

    Those are called ordinary differential equation because they involve only 
    totally derivativs

    > O.D.E -- Ordinary differential equations

    They express relationships involving rates of change.
    The order of a differential equation is the order of its hightest derivatives 

* Solution Demo
    a solutuon of a D.E is any function that satisfies\
    $y''(x) + 4y = 0 \stackrel{y=sin(2x)}{\longrightarrow} -4sin(2x)+4sin(2x) = 0$\
    $y' = \frac{y}{x} + 1 \stackrel{y = xln(x)-x}{\longrightarrow}$
    $ln(x) + x\frac{1}{x} -1 = ln(x)$

    he solve that by a predefined answer, 
    Let learn how to get that answer in later if the class
    
* General and particular solutions
    * General solutions
        The most general form of a first-order D.E. is
        $F(x,y,y') = 0$
        $y' - y^2 - e^y = 0$

        example ?\
        $y' = 2 \stackrel{\int}{\longrightarrow} y = 2x + C$\
        $y' - cos(x) = 0$
    
        a solution of the first-ordere D.E is $y(x) = \phi(x)$\
        $F(x, \phi(x), \phi'(x)) = 0$\
        $\phi(x)$ satisfise the D.E. $F(x, \phi(x), \phi'(x)) = 0$

        example \
        $y' + y = = 2 \stackrel{\phi(x)=2+ke^-x}{\longrightarrow}$ 

    so called general solution, which envolved one variable

    * Particular Solution
        - $C=-1, \phi(x)=xln(x)-x$ particular solution
        - $C=0, \phi(x)=xln(x)$ the other particular solution
        - $C=1 \phi(x)=xln(x)+x$ another particular soltion
        - BLANK INTENTIONALLY\
    * Explicitly and Implicitly Defined solutions

        Sometimes we can write a solution explicitly giving y as a function of x\
        $y'= -y \stackrel{y = ke^-x}{\longrightarrow} y = ke^-x$

    * Implicitly Solution

        Considier the D.E.\
        $y'= - \frac{2xy^3 + 2}{3x^2 y^3 + 8e^4y}$

        We claim that the general solution is the function $y(x)$\
        implictly defined by the equation\
        $x^2y^3 + 2x + 2e^{4y} = k$

        > There are no clearly $y$ equal to something.
        > Too check if is a solution, we can integral both side of the solution
        > $y = \int x^2y^3 + 2x + 2e^{4y} \stackrel{y = \int k}{\longrightarrow}$
        > $(3x^2y^3 + 8e^{4y})y' = -(x + 2xy^3) \longrightarrow y' = -\frac{2xy^3 + 2}{3x^2y^3 + 8e^{4y}}$

* Integral Curves
    * Definition

        A graph of a solition of a first-order D.E is called an 
        intergral curves of the equation
    * Example

        Consider the D.E. $y' + y = 2$
        The genenral solution is $y=2+ke^{-x}$

* Initial Value Problem
    - Definition

        a first-order initial value problem has the form $F(x, y, y') = 0, y(x_0)=y_0$\
        The condition $y(x_0)=y_0$ is called an initial condition.
    - Example 1.4

        Consider the inital value problem $y'+y=2$, $y(1) = -5$
        The general solution is $y=2+ke^{-x}$
        $\rightarrow y(1) = 2 +ke^{-1} = -5 \rightarrow k = -7e$
        $\rightarrow y = 2-7ee^{-x} = 2-7e^{-(x-1)}$



