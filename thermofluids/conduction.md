# Thermal Conduction

## Fourier's Law
$$ \dot{q} = - \lambda \nabla T $$ 
In 1D (ie. 3D where $ x $ is the linear distance through a material and A is the area of the material plate):
$$ \dot{q} = \dfrac{\dot{Q}}{A} = - \lambda \dfrac{\partial T}{\partial x} $$ 


## Heat Transfer

### Electrical Analogy
$ T \longleftrightarrow V \quad \dot{Q} \longleftrightarrow I \quad R_{Th} \longleftrightarrow R $  

$ I = \dfrac{\Delta V}{R} \qquad \dot{Q} = \dfrac{\Delta T}{R_{Th}} $
$$ \dot{Q}_{i \rightarrow i+1} = - \dfrac{T_{i+1} - T_{i}}{R_{Th \ i}} = \dfrac{T_{i} - T_{i+1}}{R_{Th \ i}} $$ 

Resistance in series sums together like in the electrical analogy and a similar potential difference equation can be written for a "series circuit" of materials as shown below.
$$ \dot{Q}_{i \rightarrow j} = - \dfrac{T_{j} - T_{i}}{\displaystyle \sum_{k=i}^{j} R_{Th \ k}} = \dfrac{T_{i} - T_{j}}{\displaystyle \sum_{k=i}^{j} R_{Th \ k}} $$ 

##### Note*: We can also apply the electrical analogy to a "parallel circuit" of materials and similarly the "current" $ \dot{Q} $ is constant in a series circuit.

</br>

### Thermal Resistance
We can even use this heat transfer law for convection provided that viscosity and flow effects are negligible.

$ l $ is the length in the heat transfer direction. $ \lambda $ is the thermal conductivity. $ h $ is the heat transfer coefficient.

$ R_{Th \ \text{Conduction}} = \dfrac{l}{\lambda A} \qquad R_{Th \ \text{Convection}} = \dfrac{1}{h A} $

For a radial surface (such as a pipe or a cylinder) where $ L $ is length of pipe and $ r $ is the radius of the surface:
$ R_{Th \ \text{Conduction}} = \int_{r_{1}}^{r_{2}} \dfrac{dr}{\lambda (2 \pi r L)} = \dfrac{\ln \Big(\dfrac{r_{2}}{r_{1}}\Big)}{\lambda (2 \pi L)} \qquad R_{Th \ \text{Convection}} = \dfrac{1}{h (2 \pi r L)} $

#### Series Example

Assume we know $ T_{1} $ and $ T_{4} $ and the **heat transfer coefficient** / **thermal conductivity** of each of the materials $ 1, 2, 3 $.
$$ T_{1} \quad \qquad \small T_{2} \quad \qquad \small T_{3} \quad \qquad \normalsize T_{4} $$
$$ \large | \quad R_{1} \quad | \quad R_{2} \quad | \quad R_{3} \quad | $$
$$ |\quad \longrightarrow \qquad \quad x \quad \qquad \longrightarrow $$

**Problem:** Find $ T_{2} $ and $ T_{3} $

**Solution:**

**Method 1**: Either derive this from the electrical analogy:
 $ V_{x} = V_{1} - \underbrace{I}_{\dfrac{V_{1}-V_{4}}{R_{1 \rightarrow 4}}} \ R_{1 \rightarrow x} $

**Method 2**: Recognise that the "current" $ \dot{Q} $ is constant in a series circuit:  $ I = \dfrac{V_{1}-V_{x}}{R_{1 \rightarrow x}} = \dfrac{V_{1}-V_{4}}{R_{1 \rightarrow 4}} $


$$ \large \therefore T_{x} = T_{in} - \underbrace{\dot{Q}}_{\displaystyle \sum_{k=in}^{out} R_{Th \ k}} \sum_{k=in}^{x} R_{Th \ k} $$

## Lumped Capacity Model

