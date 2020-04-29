# Quantum Mechanics

## Wave-Particle Duality
Note*: A-Level Revision

### Double-Slit Experiment
(Insert Diagram Here)
...

### Equations

Planck's Constant &emsp; $ h = 6.626... × 10^{-34} \ m^{2} kg s^{-1}  \qquad \hbar = \dfrac{h}{2 \pi} $


Wavelength &emsp; $ \lambda = \dfrac{h}{p} = \dfrac{h}{mv} \qquad $ 

Wave Vector &emsp; $ k = \dfrac{2 \pi}{\lambda} $

Momentum &emsp; $ p = mv = \dfrac{h}{\lambda} = \hbar \ k $

Energy &emsp; &emsp; $ E = hf = h \dfrac{c}{\lambda} = \hbar \ \omega $

</br><hr></br>

## Wave Function
Consider the wave function of a particle to be $ \psi $ containing information of all the measurable properties of the particle.

For simplification of analysis, it is best to consider the 1D case: </br>
1D - $ \psi(x, t) $ &emsp;
2D - $ \psi(x, y, t) $ &emsp;
3D - $ \psi(x, y, z, t) $ &emsp;

Probability Density (of finding particle between $ x  $ and $ x + \delta x$) = $ \psi \psi^{*} $ 

$ \therefore $ If $ \psi(x, t) $ is real, $$ P(a < p_{x} < b) = \int_{x=a}^{x=b} |\psi^{2}| dx $$

### Wave Operators
We can operate on the wave-function $ \psi(x, t) $ to determine the attributes of the wave-particle.

#### Momentum
$$ \hat{p_{x}} = \dfrac{\hbar}{i} \dfrac{\partial}{\partial x} $$
In the 2D $ \psi(x, y, t) $ or 3D $ \psi(x, y, z, t) $ case, the operator is a vector operator (using the grad operator $ \nabla $ ):
$$ \underline{\hat{p}} = \begin{bmatrix} \hat{p_{x}} \\
           \hat{p_{y}} \\
           \hat{p_{z}}
         \end{bmatrix}
= \dfrac{\hbar}{i} \nabla $$

#### Energy
$$ \hat{E} = - \dfrac{\hbar}{i} \dfrac{\partial}{\partial t} $$

In each case, applying the operator $ \hat{\Theta} $ returns the attribute $ \Theta $ itself multiplied by the wave-function $ \psi $:
$$ \hat{\Theta} ( \psi ) = \Theta \psi $$

#### Example:
Let $ \psi $ be a plane wave $ \psi = Ae^{i(k x - \omega t)}$:
$$ \therefore \hat{p_{x}} ( \psi ) = \dfrac{\hbar}{i} \dfrac{\partial \psi}{\partial x} = ik \dfrac{\hbar}{i} Ae^{i(k x - \omega t)} = k \hbar \ \psi \qquad \therefore p_{x} = k \hbar $$
$$ \therefore \hat{E} ( \psi ) = - \dfrac{\hbar}{i} \dfrac{\partial \psi}{\partial t} = -i\omega \dfrac{\hbar}{i} Ae^{i(k x - \omega t)} = \omega \hbar \ \psi \qquad \therefore E = \omega \hbar $$

</br><hr></br>

## Schrodinger's Equation

### Introduction
Schrodinger's equation is essentially the application of the Hamiltonian $ \hat{H} $ (ie. Total Energy $ \hat{E} $) operator on a wave function.

As we saw previously, the **time-dependent** energy operator is as follows:
$$ \hat{E} = - \dfrac{\hbar}{i} \dfrac{\partial}{\partial t} $$

However we can also calculate the energy operator as follows:
$$ \text{Total Energy} = \text{Kinetic Energy} + \text{Potential Energy} $$

$$ \text{Kinetic Energy Operator} \qquad \hat{T} = \Bigg(\dfrac{|\underline{\hat{p}}|^{2}}{2m} = -\dfrac{\hbar^{2}}{2m} \nabla^{2} \Bigg)= \dfrac{\hat{p_{x}}^{2}}{2m} = - \dfrac{\hbar^{2}}{2m} \dfrac{\partial^{2}}{\partial x^{2}} $$

$$ \text{Potential Energy Operator} \qquad \hat{V} \qquad \small \text{(Dependent on Potential terrain)} $$

$$ \text{Energy Operator (Hamiltonian)} \qquad \hat{H} = \hat{T} + \hat{V} = \dfrac{\hat{p_{x}}^{2}}{2m} + \hat{V} $$

Therefore we can now equate the **time-dependent** energy operator with the hamiltonian operator giving the following:
$$ \Big(\hat{H} =\Big) \qquad \hat{T} + \hat{V} = \hat{E}$$ 

This is the full "Schrodinger operator":
$$ \dfrac{\hat{p_{x}}^{2}}{2m} + \hat{V} = - \dfrac{\hbar}{i} \dfrac{\partial}{\partial t} $$
$$ - \dfrac{\hbar^{2}}{2m} \dfrac{\partial^{2}}{\partial x^{2}} + \hat{V} = - \dfrac{\hbar}{i} \dfrac{\partial}{\partial t} $$

Applying this to our wave function $ \psi $ gives us the famous Schrodinger equation:
$$ - \dfrac{\hbar^{2}}{2m} \dfrac{\partial^{2} (\psi)}{\partial x^{2}} + \hat{V}(\psi) = - \dfrac{\hbar}{i} \dfrac{\partial(\psi)}{\partial t} $$
$$ - \dfrac{\hbar^{2}}{2m} \dfrac{\partial^{2} \psi}{\partial x^{2}} + V \psi = - \dfrac{\hbar}{i} \dfrac{\partial \psi}{\partial t} $$

However we will be looking at the **time-independent** Schrodinger equation (ie. $\hat{E} (\psi) = \text{Constant} = E \psi $):
$$ - \dfrac{\hbar^{2}}{2m} \dfrac{\partial^{2} \psi}{\partial x^{2}} + V \psi = E \psi $$

### Solutions

Linear PDE
