# Semiconductors

## Introduction

**Metals** - Overlap of valence and conduction bands

**Semiconductors** - Valence and conduction band gap $ 0.5 < E_{g} < 2eV  \small \text{(non-strict values)} $

**Insulators** - Valence and conduction band gap $ E_{g} > 2eV  \small \text{(non-strict values)} $

</br>

Minimum Energy of Conduction Band $ \qquad \qquad - \qquad E_{c} $ </br>
Maximum Energy of Valence Band $ \qquad \qquad \quad - \qquad E_{v} $ </br>
Valence to Conduction Energy Band Gap $ \qquad - \qquad E_{g} = E_{c} - E_{v} $ </br>

</br>

$
n = \small\text{ Electron Concentration in Conduction Band } \qquad E > E_{c} \\
p = \small\text{ Hole Concentration in Valence Band } \qquad E < E_{v} \\
n_{i} = \small\text{ Intrinsic Carrier Concentration } \\
$

(Insert Diagram Here)

</br>

**Semiconductor Conductivity** - Dependent on **Electron/Hole Concentration** and **Drift Velocity**

**Thermal Equilibrium** - Rate of Electron-Hole Pair Formation = Rate of Electron-Hole Pair Recombination

</br>

## Fermi Function

The Fermi function $ f(E) $ is a probability function (not probability density) which outputs the probability of an electron having energy $ E $ under thermal equilibrium. This will be useful for us to find the probability of an electron being in the valence or the conduction band.

$$ \large f(E) = \dfrac{1}{1+e^{\frac{E-E_{f}}{kT}}} $$

The function is dependent on the Fermi energy level $ E_{f} $:

$$ E_{f} = \dfrac{E_{c} + E_{v}}{2} + \dfrac{1}{2} kT \ln \dfrac{N_{v}}{N_{c}} = \dfrac{E_{c} + E_{v}}{2} + \dfrac{3}{4} kT \ln \dfrac{m_{p}^{*}}{m_{n}^{*}} $$

For an intrinsic semiconductor at thermal equilibrium, the Fermi energy level $ E_{f} $ is roughly the midpoint of $ E_{v} $ and $ E_{c} $:
$$ E_{f} \approx \dfrac{E_{c} + E_{v}}{2} $$


## Conductivity


### Intrinsic Carriers
For **intrinsic** (undoped) semiconductors at **thermal equilibrium**, the following is true where $ n_{i} $ is a **temperature-dependent material property**:
$$ n = p = n_{i} $$

This essentially means that the "default" number of charge carriers at thermal equilibrium is the number of electrons in the conduction band which is equivalent to the number of holes in the valence band (since the electrons have moved from the valence band to the conduction band). 

### Mass Action Law

$$ \large \text{Law of Mass Action} \qquad np=n_{i}^{2} $$

The product of the number of electrons in the conduction band and the number of holes in the valence band is constant at a fixed temperature and is independent of the amount of donor and acceptor impurity added.
##### Note*: Applies to both intrinsic and extrinsic semiconductors.

</br>

### Semiconductor Doping
Consider silicon lattice:
(Insert Image Here)

We can now consider the overall **charge neutrality condition** to calculate the hole and electron concentrations in an extrinsic (doped) semiconductor.

For a non-degenerately doped p-and-n-type semiconductor:
$$ \large p + N_{D}^{+} = n + N_{A}^{-} $$ 

We can split this into useful dopant equations for one of p-type or n-type doping.

</br>


#### N-Type Dopant (Electron Donor)
- Group 5 Element - Atom contributes an electron to the lattice

$ N_{D}^{+} = \small\text{Number of Ionised Donors} \ (cm^{-3})$
### $$ n = p + N_{D}^{+} $$

##### If $ N_{D}^{+} >> n_{i} $, then $ n \approx N_{D}^{+} $

</br>

#### P-Type Dopant (Electron Acceptor / Hole Donor)
- Group 3 Element - Atom contributes a hole to the lattice

$ N_{A}^{-} = \small\text{Number of Ionised Acceptors} \ (cm^{-3})$
### $$ p = n + N_{A}^{-} $$

##### If $ N_{A}^{-} >> n_{i} $, then $ p \approx N_{A}^{-} $

</br>

##### Note*: We can combine the suitable $ \textbf{doping equation} $ with the $ \textbf{mass action law} $ to solve for $ n $ or $ p $ given $ N $ and $ n_{i} $

</br>

### Drift Velocity

Here we assume a proportionality relationship for drift velocity. 

### $$
\underbrace{v_{d}}_{\text{Drift Velocity}} = \underbrace{\mu}_{  \small\text{Const. of Proportionality} \\ \qquad \text{"Mobility"} } \quad \underbrace{\xi}_{\textbf{Low} \ \text{Electric Field}}
$$

##### Note*: The mechanism of transport we are considering is "drift transport" which is different to other mechanisms of transport such as diffusion.
##### Note*: Electric field must be low because at high electric fields, velocity saturation occurs due to optical phonon scattering or the Gunn effect (inter-valley electron transfer).

</br>

Now we need another equation that connects drift velocity to the electric field so that we can find some value for mobility. F=ma is not directly applicable as electrons collide with atoms in the lattice. However we can consider the electron to have effective mass $ m^{*} $, the mean collision time to be $ t_{col} $ with velocity $ v $ moving in an electric field with electric field strength $ \xi $:

$$ \large \dfrac{m_{n}^{*} \ v_{d}}{t_{col}} = q \ \xi $$ 

We can now rearrange for the mobility:
$$ \therefore \mu_{n} = \dfrac{q \ t_{col}}{m_{n}^{*}} $$

##### Note*: This is also applicable to holes and we can derive the same equations for holes. You must consider holes to be the movement of positive charge in the opposite direction to the direction of the electrons.

##### Note*: We avoid the use of E for electric field (electric field strength) as E also represents energy

</br>

### Current Density

Upon the application of a potential difference to a material, the gradient of the energy bands increases (imagine the slanting of the energy band downwards towards the +ve terminal). The electrons in both the conduction and the valence band are attracted towards the positive terminal. The electrons in the conduction band can freely move hence causing current flow however the electrons in the valence band are confined to fill the available holes in the valence band and hence the electrons in the valence band move into the vacant holes towards the positive terminal.



