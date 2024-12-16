# Parseval Relationships

## FT

$$ \int_{-\infty}^{\infty} |x(t)|^2 dt = \frac{1}{2\pi}\int_{-\infty}^{\infty} |X(\omega)|^2 d\omega $$

## FS 

$$ \frac{1}{T} \int^T_0 |x(t)|^2 dt = \sum_{n=-\infty}^{\infty} |X[k]|^2 $$

## DTFT

$$\sum_{n=-\infty}^{\infty} |X[n]|^2 =
\frac{1}{2\pi} \int_{-\pi}^{\pi} |x(e^{j\Omega})|^2 d\Omega $$

## DTFS

$$ \frac{1}{N} \sum_{n=0}^{N-1} |x[n]|^2 = \sum_{k=0}^{N-1} |X[k]|^2 $$

# Time-bandwidth product

## Time Duration

$$ T_d = \frac{\int^\infty_{-\infty}t^2|x(t)|^2dt}{\int^\infty_{-\infty}|x(t)|^2dt}^{1/2} $$

# Effective Bandwidth

$$ B_e = \frac{\int^\infty_{-\infty}\omega^2|X(\omega)|^2d\omega}{\int^\infty_{-\infty}|X(\omega)|^2d\omega}^{1/2} $$

# Time-bandwidth product

$$ T_dB_w \geq \frac{1}{2} $$

# Duality

## FT

$$ x(t) \rightarrow X(j\omega) \rightarrow X(jt) \rightarrow 2\pi x(-\omega)$$

## DTFS

$$ x[n] \rightarrow X[k] \rightarrow X[-n] \rightarrow \frac{1}{N} x[-k] $$

## DTFT-FS

$$ x[n] \rightarrow_{DTFT} X(e^{j\Omega}) \rightarrow X(e^{jt}) \rightarrow_{FS} x[-n] $$
