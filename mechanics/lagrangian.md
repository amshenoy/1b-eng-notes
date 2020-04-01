# Lagrangian Mechanics

### $$ Lagrangian = Kinetic Energy - Potential Energy $$
## $$ L = T - V $$

### Equations of Motion
$$ \frac{d}{dt}(\frac{\partial L}{\partial \dot{q}}) = \frac{\partial L}{\partial q} $$

$$ \frac{d}{dt}(p) = F $$

### Mass and Potential Matrices
Mass matrices must be symmetrical however potential matrices do not! For a N-body system, the kinetic energy of a single body is solely dependent on its own mass and velocity and hence the mass matrix must not only be symmetrical but also a diagonal matrix. However for a rigid body, the mass matrix is a symmetrical matrix.

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
