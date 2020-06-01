# Plastic Theory

## Plastic Moment

$ Z_{p} \qquad \small \text{Plastic Section Modulus} $
$$ M_{p} = \sigma_{} Z_{p} $$
$ m_{p} \qquad \small \text{Plastic Moment Capacity (Plastic Moment per unit length of yield-line/slip-line)}$ 

## Upper-Bound Theory

### Beams & Frames (Hinge Analysis)

$ \delta_{i} = l_{i} \theta_{i} $

For all assumed plastic nodes in the beam structure, calculate the overall work done $ W.D $ by the applied forces and the overall energy dissipated $ E.D $  by the plastic deflection of the beam:
$$ W.D = \sum_{i} F_{i} \cdot \delta_{i} \quad \Big( = \sum_{i} \int_{x=0}^{x=l_{i}} q(x)_{i} \cdot \delta_{i}(x) dx \Big) $$ 
$$ E.D = \sum_{i} M_{p \ i} \cdot \theta_{i} $$

Equate $ W.D $ and $ E.D $ to form an equation and solve for any unknown variables. Use linear superposition of forces in the above method when necessary. For frames, consider different locations of  plastic hinges to find the best lower-bound of load.

### Slabs (Yield-Line Analysis)
$ d_{k} \qquad \small \text{Distance of COM (of considered section) from the axis of rotation }$
$$ W.D = \sum_{k} p_{k} A_{k} \cdot d_{k} \quad \Big( = \int P \ dV \Big) $$
$$ E.D = \sum_{i} m_{p \ i} \ l_{i} \ \theta{i} $$

### Materials (Slip-Line Analysis)

## Lower-Bound Theory
