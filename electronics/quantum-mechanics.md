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

Essentially the Hamiltonian Operator (ie. Total Energy)
