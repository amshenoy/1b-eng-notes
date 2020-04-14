# Feedback Control Systems

## Block Diagram Example


## Definitions

### <font color="#00f">Feedforward</font> Transfer Function
### $ F(s) = ABC $ - Product of all blocks in forward line from $ \bar{x} \to \bar{y}$

### <font color="#00f">Feedback</font> Transfer Function
### $ G(s) = D $ - Product of all blocks in feedback line from $ \bar{y} \to \bar{x}$

</br></br>

### <font color="#00f">Loop</font> Transfer Function (<font color="#0b0">Return Ratio</font>)
### $ L(s) = ABCD = F(s) G(s) $ - Product of all blocks in loop

### <font color="#00f">Sensitivity</font> Transfer Function 
### $ S(s) = \dfrac{1}{1+L(s)} = \dfrac{1}{1 + F(s) G(s)} $

### <font color="#00f">Complementary Sensitivity</font> Transfer Function
### $ T(s) = \dfrac{L(s)}{1+L(s)} = \dfrac{F(s) G(s)}{1 + F(s) G(s)} = L(s) S(s) $

#### Note*: S(s) + T(s) = 1; Ideally we want $ S(s) \approx 0 $ 
</br></br>

### <font color="#00f">Closed-Loop</font> Transfer Function (<font color="#0b0">Full System</font>)
### $ H(s) = \dfrac{F(s)}{1+L(s)} = \dfrac{F(s)}{1 + F(s) G(s)} = F(s) S(s) $

</br></br>

### <font color="#00f">Steady State Gain</font> (<font color="#0b0">Final Value Step Response</font>)

$ SSG = \dfrac{\bar{y}}{\bar{x}}|_{s=0} = H(0) $

### <font color="#00f">Steady State Error</font>

$ SSE = 1 - \dfrac{\bar{y}}{\bar{x}}|_{s=0} = 1 - H(0) \qquad (= 1 - SSG) $

## Disturbance Rejection

We can add a <font color="#36f">controller $ K(s) $</font> transfer function  to the input of the <font color="#36f">plant $ H(s) $</font> transfer function (the system that needs to be controlled). Consider that the plant has some added <font color="#36f">input disturbance $ \bar{d_{i}} $</font> and some added <font color="#36f">output disturbance $ \bar{d_{o}} $</font>.

### Block Diagram

</br>

$$ \bar{y} = \dfrac{HK}{1+HK} \bar{x} + \dfrac{H}{1+HK} \bar{d_{i}} + \dfrac{1}{1+HK} \bar{d_{o}} $$

In this case, the loop transfer function is $ L(s) = HK $:

$$ \bar{y} = \dfrac{L}{1+L} \bar{x} + \dfrac{H}{1+HK} \bar{d_{i}} + \dfrac{1}{1+L} \bar{d_{o}} $$
$$ \therefore \bar{y} = \color{blue}T \ \bar{x} + \dfrac{H}{1+HK} \bar{d_{i}} + \color{blue}S \ \bar{d_{o}} $$

Here we can see how the sensitivity and complementary sensitivity transfer functions affect the output signal. Hence we require $ S \approx 0 $ to minimise the effects of the output disturbance given that there is no input disturbance ($ \bar{d_{i}} = 0 $).

### PID Controller






