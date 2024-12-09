# Convolution property

For a linear system, we can analyze input output behavior in frequency domain by multiplying transform instead of convolution in time domain.

$$y(t)=h(t)*x(t) \Leftrightarrow Y(f)=H(j\omega)X(j\omega )$$
$$y[n]=h[n]*x[n] \Leftrightarrow Y(e^{j\Omega})=H(e^{j\Omega})X(e^{j\Omega})$$

# Filtering

## Magnitude
Magnitude response is commonly describe in dB$20logx$
And the edge of passband is defined as -3dB or $\frac{1}{\sqrt2}$

## Frequency response
We describe frequency response of a system ratio of input and output

$$ H(j\omega)=\frac{Y(j\omega)}{X(j\omega)}$$
$$ H(e^{j\Omega})=\frac{Y(e^{j\Omega})}{X(e^{j\Omega})}$$

## Recover input
We can recover input signal by inverse transform of frequency response

$$X(j\omega)=H^{-1}(j\omega)Y(j\omega)$$
$$X(e^{j\Omega})=H^{-1}(e^{j\Omega})Y(e^{j\Omega})$$

Such inverse system is known as equalizer.

# Differentiation and Integration Properties

## Differentiation
- Differentiation multiply an $j\omega$ in frequency domain(FT)
- Buffing the high frequency and attenuate(make something smaller) the low frequency
- Destroy DC or constant component

$$ \frac{d}{dt}x(t) \Leftrightarrow j\omega X(j\omega)$$

## Integration
Integration applies only to continuous dependent variable
- Averaging operation
- smoothing
- Attenuate high frequency

$$ \int_{-\infty}^{t}x(\tau)d\tau \Leftrightarrow \frac{1}{j\omega}X(j\omega) + \pi X(j0)\delta(\omega)$$

Notice that we add $\pi X(j0)\delta(\omega)$ for $\omega=0$

# Time & Frequency Shifting

## Time shifting
Time shifting in time domain is equivalent to multiplying by $e^{-j\omega t_0}$ in frequency domain

$$ x(t-t_0) \Leftrightarrow e^{-j\omega t_0}X(j\omega)$$

## Frequency shifting
Frequency shifting in frequency domain is equivalent to multiplying by $e^{j\gamma t}$ in time domain

$$ X(j\omega - \gamma) \Leftrightarrow x(t)e^{j\gamma t}$$

# Inverse FT
Assuming $X(j\omega)$ is expressed as a ration of polynomials in $j\omega$
Then we can find $x(t)$ by partial fraction expansion and inverse FT

$$\sum^{N}_{k=1} \frac{C_k}{(j\omega - d_k)} \Leftrightarrow \sum_{k=1}^N C_k e^{d_kt}$$


# Multiplication Property
Multiplication in Time Domain is equivalent to convolution in frequency domain

$$ x(t)y(t) \Leftrightarrow \frac{1}{2\pi}X(j\omega)*Y(j\omega)$$

# Scaling Property
Scaling in time domain is equivalent to inverse scaling in frequency domain

$$ x(at) \Leftrightarrow \frac{1}{|a|}X(\frac{j\omega}{a})$$

