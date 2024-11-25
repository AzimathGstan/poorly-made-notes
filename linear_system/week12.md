# Ranges
## Time-Domain-Periodic Signal
For Time-Domain-Periodic signals we can add the Fourier Series of Harmonics 
$k\Omega_0$(for Discrete)or $k\omega_0$(for Continuously) to get it.
Then for Frequency-Domain-Periodic signals we can add

$$\hat{x}[n]=\sum^{N-1}_{k=0}A[k]e^{jk\Omega_0n}$$

For Non-Frequency-Domain-Periodic signal we

$$ \hat{x}[n]=\sum^{\infty}_{k=-\infty}A[k]e^{j\Omega_0n}$$

## Time-Domain-Aperiodic Signal
For Time-Domain-Aperiodic signals we use the Discrete Time Fourier Transform(DTFT) or the Fourier Transform(FT).
Unlike the Fourier Series, we can combine not only the harmonics but any frequency to get the signal. We detonate that as $\Omega$(for Discrete) or $\omega$(for Continuously).

For Frequency-Domain-Periodic signals we describe it as:

$$ \hat{x}(n)=\frac{1}{2\pi}\int^\pi_{-\pi}X(e^{j\omega})e^{j\omega n}d\omega$$

For Non-Frequency-Domain-Periodic signal we describe it as:

$$ \hat{x}(n)=\frac{1}{2\pi}\int^\infty_{-\infty}X(e^{j\omega})e^{j\omega n}d\omega$$

# DTFS - Discrte Time Fourier Series

# FS - Fourier Series 

# DTFT - Discrete Time Fourier Transform

# FT - Fourier Transform
