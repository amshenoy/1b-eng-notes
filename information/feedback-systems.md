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
