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
DTFS representation of periodic signal $x[n]$ with period $N$ and fundamental frequency $\Omega_0=2\pi/N$ is given by

$$ x[n]=\sum^{N-1}_{k=0}X[k]e^{jk\Omega_0n}$$
  
  Where $X[k]$ is the DTFS coefficients given by

$$ X[k]=\frac{1}{N}\sum^{N-1}_{n=0}x[n]e^{-jk\Omega_0n}$$
Which $X[k]$ is a frequency-domain representation of the signal $x[n]$.

> TODO add some examples start from ptt 40, 41
# FS - Fourier Series 
FS representation of a periodic signal $x(t)$ with period $T$ and fundamental frequency $\omega_0=2\pi/T$ is given by

$$ x(t)=\sum^{\infty}_{k=-\infty}X[k]e^{jk\omega_0t}$$

Where $X[k]$ is the FS coefficients given by

$$ X[k]=\frac{1}{T}\int^{T/2}_{-T/2}x(t)e^{-jk\omega_0t}dt$$

or 

$$ X[k]=\frac{1}{T}\int^{T}_{0}x(t)e^{-jk\omega_0t}dt$$

depend on the situation.

Which $X[k]$ is a frequency-domain representation of the signal $x(t)$.

> TODO add some example start from ptt 67

# DTFT - Discrete Time Fourier Transform

# FT - Fourier Transform
