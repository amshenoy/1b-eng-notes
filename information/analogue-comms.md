# Analogue Communications

**Analogue Communication Process**

Modulation $ \rightarrow $ Transmission $ \rightarrow $ Demodulation $ \rightarrow $ Analogue-Digital Converter 

We are not going to cover the transmission process in this topic as this is an electronics problem however we will be looking at the process of modulation, demodulation and the AD conversion.

## Analogue Modulation

The process of transmitting a low frequency analogue (wave) signal over a higher frequency signal (higher energy therefore higher distance transmission).

The **baseband/modulating** signal is the **"message"** signal and the **carrier/envelope** signal is the **"encoder"** signal.

### Amplitude Modulation (AM)
$$ AM(t) = ( \ A_{\text{carrier}} + \text{Baseband}(t) \ ) \cdot \text{Carrier}(t) $$
Modulation Index: $ m = \dfrac{A_{\text{Baseband}}}{A_{\text{Carrier}}} \qquad m < 1 $ is desirable
 
Example Signal:
$$
\begin{align*} 
s(t) &= (A_{c} + A_{m}\cos(2\pi f_{m}t)) \cdot \cos(2\pi f_{c}t) \\
&= A_{c} \ (1 + m\cos(2\pi f_{m}t)) \cdot \cos(2\pi f_{c}t) 
\end{align*}
$$

#### Improvements
We can reduce the power consumption and increase the number of channels available for data transmission by using a single sideband transmission. AM transmission by default uses double sideband transmission.

$$ \small \text{Channels Available} = \dfrac{\text{Transmission Bandwidth}}{\text{Available Bandwidth}}  $$ 
##### Double Sideband (DSB)
Transmission Bandwidth: $ 2 f_{m} + f_{g} $

##### Single Sideband (SSB)
Transmission Bandwidth: $ f_{m} + f_{g} $

### Frequency Modulation (FM)

Let $ x(t) = a_{m} cos(2 \pi f_{m} t) $

Applying frequency modulation to $ x(t) $:
$$ FM(t) = A_{c} \cos(2 \pi f_{c} t + m \sin(2 \pi f_{m} t)) $$
Modulation Index: $ m = \dfrac{(\Delta f)_{\text{peak}}}{f_{m}} \qquad m < 1 $ is desirable

Transmission Bandwidth: $ 2 \Big( (\Delta f)_{\text{peak}} + f_{m} \Big) \qquad (Carson's Rule) $


## Analogue Demodulation




## Analogue-Digital Converter (ADC)

### Nyquist's Sampling Theorem
$$ f_{\text{sampling}} \geqslant 2 f_{max} $$

### Binary Data

$$
\begin{align*}
\text{Bit Rate} &= (\text{Bits per Sample}) * (\text{Samples per Second}) \\
 &= (\text{Sample Resolution}) * (\text{Sample Rate})
\end{align*}
$$

### Quantisation Noise





