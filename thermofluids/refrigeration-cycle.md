## Refrigeration Cycle / Heat Pump Cycle
### Overview
- **Vapour Compression** Cycle
- **Multi-phase** Process
- Transfer heat to the higher temperature location
- Use of **refrigerant** fluid (Consider R-134a) 

### Cycle Process
(Insert T-s Diagram here)

State **1** - **Vapour** Saturated </br>
State **3** - **Liquid** Saturated

**1-2** - Compression - **Compressor** </br>
**2-3** - Condensation - **Condenser** </br>
**3-4** - Expansion - **Throttle** </br>
**4-1** - Evaporation - **Evaporator** </br>

(Insert P-h diagram here)

$ 
\text{Compressor} \qquad w_{c} = h_{2} - h_{1} \qquad \qquad \qquad \qquad h_{1} = \small \color{blue}{\text{R-134a}-\text{SAT-Table}_{h}\big[g\big]\Big(P_{1}\Big)} \\

\text{Condenser} \qquad \quad q_{23} = h_{3} - h_{2} \qquad \qquad \qquad \quad h_{2} = \small \color{blue}{\text{R-134a}-\text{SH-Table}_{h}\big[T_{SH}\big]\Big(P_{2}\Big)} \\

\text{Throttle} \qquad \qquad h_{4} = h_{3} \qquad \qquad \qquad \qquad \qquad h_{3} = \small \color{blue}{\text{R-134a}-\text{SAT-Table}_{h}\big[f\big]\Big(P_{3}\Big)} \\

\text{Evaporator} \qquad q_{41} = h_{1} - h_{4} \qquad \\
$

### Coefficient of Performance (COP)
#### Refrigerator
$
COP_{R} = 
\underbrace{ \dfrac{q_{\text{in}}}{ w_{\text{in}} } \\}
_{\\ \dfrac{h_{1}-h_{4}}{h_{2}-h_{1}} } 
= 
\underbrace{ \dfrac{q_{c}}{q_{h} - q_{c}} \\}
_{\\ \dfrac{h_{1}-h_{4}}{(h_{2}- \underbrace{h_{3}}_{h_{4}}) - (h_{1}-h_{4})} }

\qquad \qquad \qquad
\text{Carnot} \ COP_{R} = \underbrace{ \dfrac{T_{c}}{T_{h} - T_{c}} \\}_{\dfrac{T_{1}}{T_{3} - T_{1}}}
$

#### Heat Pump
$
COP_{HP} = \underbrace{ \dfrac{q_{\text{out}}}{ w_{\text{in}} } \\}
_{\\ \dfrac{h_{2}-h_{3}}{h_{2}-h_{1}} } 
= 
\underbrace{ \dfrac{q_{c}}{q_{h} - q_{c}} \\}
_{\\ \dfrac{h_{2}-h_{3}}{(h_{2}- \underbrace{h_{3}}_{h_{4}}) - (h_{1}-h_{4})} }

\qquad \qquad \qquad
\text{Carnot} \ COP_{HP} = \underbrace{\dfrac{T_{h}}{T_{h} - T_{c}} \\}_{\dfrac{T_{3}}{T_{3} - T_{1}}}
$
 
##### Note*: Always use |q| for calculating COPs to not make mistakes in signs.
$ q_{h} = q_{32} $ and $ q_{c} = q_{41} $
