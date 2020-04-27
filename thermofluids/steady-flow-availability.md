# Steady Flow Availability (Exergy)

### Gibbs Free-Energy
$$ \Delta G = \Delta H - T_{0} \Delta S$$
$$ \qquad b_{2} - b_{1} = (h_{2}- h_{1}) - T_{0} (s_{2} - s_{1}) $$

### Steady Flow Availability Equation
### $$  
\underbrace{
\underbrace{ \dot{m} (b_{2} - b_{1}) }_{ \text{Max Power} \\
\text{Potential} } \\
}_{ \\ \\ \dot{m} ((h_{2}- h_{1}) - T_{0} (s_{2} - s_{1})) }
=
- 
\underbrace{
\underbrace{ \dot{W_{x}} }_{ \text{Shaft Power} } \\
}_{ \\ \\ \eta \\ \dot{m} (c_{p}(T_{1}- T_{2})) }
+ 
\underbrace{
\underbrace{ \int (1 - \dfrac{T_{0}}{T}) \ d \dot{Q} }_{ \text{Transfer of Power Potential} \\ \text{due to Heat Transfer} } \\
}_{\text{(Indirect Calculation)} \\ \text{ie. rearrange for this} \\ \\ = 0 \text{ if adiabatic C.V } }
-
\underbrace{
\underbrace{  T_{0} \ \dot{S}_{\text{irrev}} }_{\text{Lost Power Potential} \\ \text{due to irreversibilities}} \\
}_{ 
\sum_{i}^{N} \ \dot{m} T_{0} \Delta s_{i} 
\\ 
\Delta s \ = \ c_{p} \ ln ( \frac{T_{2}} {T_{1}} ) - R \ ln(\frac{P_{2}}{P_{1}}) \\ (\text{Databook})
}
$$

### Model Examples for Analysis
</br>

#### Gas Turbine

(Insert Diagram here)

$ P_{4} = P_{atm} $ </br>
$ \dot{W_{x}} = \dot{W_{T}} - \dot{W_{C}} $

</br>

#### Jet Engine

(Insert Diagram here)

$ P_{5} = P_{atm} $ </br>
$ \dot{W_{T}} = \dot{W_{C}} \quad (\dot{W_{x}} = 0)$ </br>
$ h_{4} = h_{5} + \frac{v_{5}^{2}}{2} \quad (\text{SFEE in nozzle}) $ 

