# Linear Control Systems

## Overview
In this topic we will be focusing on Linear Time-Invariant (LTI) systems.

Given a real-life system, we can attempt to find a linear differential equation in the form $ a_{0}(t) \ y(t) + a_{1}(t) \ \frac{dy(t)}{dt} + ... + a_{n}(t) \ \frac{d^{n}y(t)}{dt} = b(t)$ where $ a_{i}(t) $ and $ b(t) $ are differentiable functions.

We can apply the Laplace transform to the found differential equation to convert it into an equivalent function in the s-domain.

This can also be written as a combination of linear operators (multiplication and addition) applied to a combination of functions in the s-domain. This is better represented as a block diagram of transfer functions consisting of linear operators.

We can then use this to analyse the response of the system to a certain input signal.

### Laplace Transform
$$ F(s) = \mathcal{L}\{f(t)\} = \int_{0^{-}}^{\infty} f(t) e^{-st} dt $$

#### Identities

##### Linearity
$$ \mathcal{L}\{a f_{1}(t) + b f_{2}(t)\} = a \mathcal{L}\{f_{1}(t)\} + b \mathcal{L}\{f_{2}(t)\} $$

##### Initial Value Theorem
$$ lim_{s \to \infty} \ (s F(s)) = f(0)$$

##### Final Value Theorem
$$ lim_{s \to 0} \ (s F(s)) = f(\infty)$$

##### Convolution Identity
$$ \mathcal{L}\{ \ f(t) * g(t) \ \} = \mathcal{L}\{f(t)\} \enspace \mathcal{L}\{g(t)\} = F(s) G(s)$$

### Block Diagrams

#### Linear System Definition
Consider an input signal x(t) into a system $ \mathcal{H} $ such that the output is y(t). For $ \mathcal{H} $ to be a linear system, the following must be true for any constants $ \alpha $ and $ \beta $:
$$ \mathcal{H} \{ \alpha \ x_{1}(t) + \beta \ x_{2}(t) \} = \alpha \ \mathcal{H} \{ x_{1}(t) \} + \beta \ \mathcal{H} \{ x_{2}(t) \} = \alpha \ y_{1}(t) + \beta \ y_{2}(t) $$



### System Response

Consider a LTI system that has the function $ g(t) $ meaning that the Laplace transform of the system time-domain function is the system transfer function $ \mathcal{L} \{g(t)\} = G(s) $ .

This is also the impulse response of the system! 
$ \mathcal{L} \{\delta(t) * g(t)\} = \mathcal{L} \{\delta(t)\} \ \mathcal{L} \{g(t)\} = 1 \cdot G(s) = G(s) $ 

Similarly the response of the system to the step function $ H(t) $ is therefore $ \mathcal{L} \{H(t)\} \ \mathcal{L} \{g(t)\} = \dfrac{1}{s} G(s)  $

### System Stability

#### Poles and Zeros
**Zeros** - Values of $ s $ for system transfer function $ H(s) \to 0 $ - [$ \text{Numerator} \to 0 $]

**Poles** - Values of $ s $ for system transfer function $ H(s) \to \infty $ - [$ \text{Denominator} \to 0 $]


__*Example:*__
$$ F(s) = \frac{s-c}{(s-a)^{2} + b^{2}} $$
*Zeros:* $ s = c \quad (s-c = 0)$ $ \qquad \qquad $ *Poles:* $ s = a \pm ib \quad ((s-a)^{2} + b^{2} = 0) $


#### Pole-Zero Plot


