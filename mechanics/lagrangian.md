# Lagrangian Mechanics

## Introduction

### $$ Lagrangian = Kinetic Energy - Potential Energy $$

## $$ L = T - V $$

### Equations of Motion
$$ \frac{d}{dt}(\frac{\partial L}{\partial \dot{q}}) = \frac{\partial L}{\partial q} $$

$$ \frac{d}{dt}(p) = F $$

## Mass and Potential Matrices

Mass matrices must be symmetrical however potential matrices do not! For a N-body system, the kinetic energy of a single body is solely dependent on its own mass and velocity and hence the mass matrix must not only be symmetrical but also a diagonal matrix. However for a rigid body, the mass matrix is a symmetrical matrix.[ [1] ](https://physics.stackexchange.com/questions/95627/can-a-mass-matrix-be-asymmetric)

$$
m_{ij} = \frac{\partial^2 T}{\partial \dot{q}_{i} \dot{q}_{j}}
\quad
M = \frac{1}{2}
\stackrel{\mbox{Symmetric Matrix}}{%
\begin{pmatrix}
2m_{1 1} & ... & m_{i 1} \\
\vdots & \ddots & \vdots \\ 
m_{j 1} & ... & 2m_{i j}
\end{pmatrix}
%}
= 
\stackrel{\mbox{Diagonal Matrix}}{%
\begin{pmatrix}
m_{1 1} & ... & 0 \\
\vdots & \ddots & \vdots \\ 
0 & ... & m_{i j}
\end{pmatrix}
%}
$$

$$ 
k_{ij} = \frac{\partial^2 V}{\partial q_{i} q_{j}}
\quad
K = \frac{1}{2}
\stackrel{\mbox{Symmetric Matrix}}{%
\begin{pmatrix}
2k_{1 1} & ... & k_{i 1} \\
\vdots & \ddots & \vdots \\ 
k_{j 1} & ... & 2k_{i j}
\end{pmatrix}
%}
$$

## Natural Frequencies & Normal Modes

#### Natural Frequencies $ \omega_{i} $ 
Calculate the eigenvalues $ \omega_{i} $ of $ K - M \omega_{i}^{2} $
$$ det(K - M \omega_{i}^{2}) = 0 $$

#### Normal Modes $ \underline{\hat{q_{i}}} $
Calculate the eigenvector $ \underline{\hat{q_{i}}} $ of $ K - M \omega_{i}^{2} $ for each eigenvalue $ \omega_{i} $ (ie. all the eigenvectors)
$$ (K - M \omega_{i}^{2}) \underline{\hat{q_{i}}} = \underline{0} $$

#### Normal Coordinates
We can decouple complex mechanical systems by converting the presumed coordinate system $ \underline{q} $ into a more insightful coordinate system $ \underline{n} $ using the calculated eigenvectors $ \underline{\hat{q_{i}}} $.

### $$ n_{i} = \underline{\hat{q_{i}}} \cdot \underline{q} $$
Our new coordinate system is the following:
$$ \underline{n} = \begin{bmatrix}
           n_{1} \\
           n_{2} \\
           \vdots \\
           n_{m}
         \end{bmatrix}
$$

## Stability

### Equilibrium Points
$$ \dfrac{dV}{dt} = 0 $$

#### Stability Criteria
$$ \dfrac{d^{2}V}{dt^{2}} > 0 \quad \therefore Minimum \quad \therefore Stable $$
$$ \dfrac{d^{2}V}{dt^{2}} < 0 \quad \therefore Maximum \quad \therefore Unstable $$

### Phase Portraits
Plot $ \dot{q_{i}} $ against $ q_{i} $

</br></br>

Every path in the phase portrait represents the trajectory that the system will follow if that inital conditions match that of the path. 

All equilibrium points must be some sort of convergence/divergence.

A convergence represents a stable equilibrium point.
A divergence represents an unstable equilibrium point.

There are many different ways a system can have equilibrium points:
* Center Point - Stable
* Saddle Point - Unstable

* Converging Point - Stable
* Diverging Point - Unstable

* Converging Spiral - Stable
* Diverging Spiral - Unstable

A closed curve is periodic and hence be considered as an equilibrium path (non-diverging).
 
</br></br>
