# FT - Fourier Transform

The Fourier Transform(FT) representation of aperiodic signal $x(t)$ is given by

$$
x(t)=\frac{1}{2\pi}\int^{\infty}_{-\infty}X(j\omega)e^{j\omega t}d\omega
$$

Where $X(j\omega)$ is the FT coefficients given by

$$
X(j\omega)=\int^{\infty}_{-\infty}x(t)e^{-j\omega t}dt
$$

These are the FT pair.

Dirichlet Condition: $x(t)$ is
- x(t) is absolutely integrable $\int^\infty_\infty|x(t)|dt<\infty$ 
- x(t) has a finite number of maxima and minima in any finite interval
- x(t) has a finite number of discontinuities in any finite interval

> Add examples

# Properties of Fourier Representations

## Time Domain Periodic Signals
- Series representation
- Signal are weighted sum of complex sinusoids (NOTE: In PPT it state that they has same period. But I don't think that harmonics have the same period as the fundamental frequency)
- We can describe the periodic signal with a finite(__Discrete__) number of harmonics(__Frequencies__).
- Such set of Frequencies are describe as $X[k]$

## Time Domain Aperiodic Signals
- Weight Integral of complexes over Frequencies representation
- We can describe the aperiodic signal with an infinite(__Continuous__) number of frequencies.

## Discrete Time Signals
Has a Periodic Frequency Domain as Discrete Signal are made up of harmonics of $2\pi N$

## Continuous Time Signals
Has a Aperiodic Frequency Domain as Continuous Signal can be made up of any frequencies which are distinct to each other.

## Summary
Representations which is Discrete(Cont.) in one domain are Periodic(Aperiodic) in the other domain.


![](attachs/Pasted%20image%2020241202214951.png)

# Symmetry Properties
## when $x(t)$ is real

$$ X^\*(j\omega)=(\int^\infty_{-\infty} x(t)e^{-j\omega t}dt)^\* = \int^\infty_{-\infty} x^\*(t)e^{-j(-\omega)t}dt $$

$x(t) = x^*(t)$

Then

$X^*(j\omega) = X(-j\omega)$

And

$\text{Re}\{X(j\omega)\} = \text{Re}\{X(-j\omega)\}$ which real part is even

$\text{Im}\{X(j\omega)\} = -\text{Im}\{X(-j\omega)\}$ which imaginary part is odd

### Even Signal
Has a real and even Frequency Domain representation

### Odd Signal
Has a imaginary and odd Frequency Domain representation

![](attachs/Pasted%20image%2020241202224308.png)
> Simulation from gnuradio. Where Blue is real and Red is imaginary.

## when $x(t)$ is imaginary

### Even Signal
Has a imaginary and even Frequency Domain representation

### Odd Signal
Has a real and odd Frequency Domain representation
![](attachs/Pasted%20image%2020241202224619.png)
> Simulation from gnuradio. Where Blue is real and Red is imaginary.

> Add examples