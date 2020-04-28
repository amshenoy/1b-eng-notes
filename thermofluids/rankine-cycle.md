# Rankine Cycle

### Overview
- **Steam Turbine** Cycle

</br>

### Working Fluids
$
\text{Total Volume} \qquad V = V_{f} + V_{g} \\
\qquad\qquad \qquad\qquad mv = m_{f}v_{f} + m_{g}v_{g} \\
\\~\\
\text{Dryness Fraction} \qquad x = \dfrac{v-v_{f}}{v_{g}-v_{f}} = \dfrac{m_{g}}{\underbrace{m_{g}+m_{f}}_{m}}\\
\qquad \qquad \qquad \qquad \qquad  = \dfrac{s-s_{f}}{s_{g}-s_{f}} = \dfrac{v-v_{f}}{v_{g}-v_{f}}


$

### Cycle Processes

State **1** - **Liquid** Saturated </br>
State **3** - **Vapour** Saturated

</br>

#### Full Cycle with Reheat
(Insert T-s Diagram here)

**1-2** - Compression - **Pump** </br>
**2-3** - Evaporation (Heat Input) - **Boiler** </br>
**3-4** - Expansion - **Turbine 1** </br>
**4-5** - Reheat </br>
**5-6** - Expansion - **Turbine 2** </br>
**6-1** - Condensation (Heat Rejection) - **Condenser** </br>


</br>

#### Simplified Cycle
(Insert 2nd T-s Diagram here)

**1-2** - Compression - **Pump** &emsp; &emsp; &nbsp; &nbsp; (+W) </br>
**2-3** - Evaporation - **Boiler** &emsp; &emsp; &emsp; (+Q)</br>
**3-4** - Expansion - **Turbine** &emsp; &emsp; &emsp; (-W)</br>
**4-1** - Condensation - **Condenser** &nbsp; &nbsp; (-Q)</br>

</br><hr></br>

### Calculations
$ 

\color{red}{v_{f1}} = \small \color{blue}{H_{2}O-\text{SAT-Table}_{v}\big[f\big]\Big(P_{1}\Big)}

\qquad \qquad

\color{red}{h_{1}} = \small \color{blue}{ H_{2}O-\text{SAT-Table}_{h}\big[f\big]\Big(P_{1}\Big) }

\\

\text{Pump} \qquad w_{p}  \approx (P_{2}-P_{1})\color{red}{v_{f1}} \times \dfrac{1}{\eta_{c}} \quad ( \small \text{Water Incompressible} ) \qquad \Big(= h_{12} = h_{2} - \color{red}{h_{1}} \Big) \\
$
</br></br>
$
\therefore \color{purple}{h_{2}} = \color{red}{h_{1}} + w_{p} = \color{red}{h_{1}} + (P_{2} - P_{1})\color{red}{v_{f1}} \times \dfrac{1}{\eta_{c}}
\\
\text{Boiler} \qquad \qquad q_{23} = \color{red}{h_{3}} - \color{purple}{h_{2}} \qquad \qquad \qquad \qquad \color{red}{h_{3}} = \small \color{blue}{H_{2}O-\text{SAT-Table}_{h}\big[g]\Big(P_{3}\Big)} \\
$
</br></br>
$
\color{purple}{h_{4s}} \Longrightarrow x = \dfrac{\overbrace{s_{4s}}^{\color{red}{s_{3}}} - \color{red}{s_{f}}}{\color{red}{s_{g}} - \color{red}{s_{f}}} = \dfrac{\color{purple}{h_{4s}} - \color{red}{h_{f}}}{\color{red}{h_{g}} - \color{red}{s_{f}}}
\qquad
\therefore 
\color{purple}{h_{4s}} = \color{red}{h_{f}} + (\color{red}{h_{g}}-\color{red}{h_{f}})\dfrac{\overbrace{s_{4s}}^{\color{red}{s_{3}}}-\color{red}{s_{f}}}{\color{red}{s_{g}}-\color{red}{s_{f}}}
\\
\small \text{Note*: All values for 4s at }P_{4}\text{ except }s_{4s}\text{ which equals }\color{red}{s_{3}}
\\
s_{4s} = \color{red}{s_{3}} = \small \color{blue}{H_{2}O-\text{SAT-Table}_{s}\big[g]\Big(P_{3}\Big)}
\\
 \color{red}{s_{g}} = \small \color{blue}{H_{2}O-\text{SAT-Table}_{s}\big[g]\Big(P_{4}\Big)} \qquad
 \color{red}{s_{f}} = \small \color{blue}{H_{2}O-\text{SAT-Table}_{s}\big[f]\Big(P_{4}\Big)}
\\
 \color{red}{h_{g}} = \small \color{blue}{H_{2}O-\text{SAT-Table}_{h}\big[g]\Big(P_{4}\Big)} \qquad
 \color{red}{h_{f}} = \small \color{blue}{H_{2}O-\text{SAT-Table}_{h}\big[f]\Big(P_{4}\Big)}
\\
\small \text{Note*: Alternatively get }\color{purple}{h_{4s}}\text{ from }\color{blue}{H_{2}O - \text{H-S-Diagram}(s=s_{3}, P=P_{3})}
\\~\\
\text{Turbine} \qquad \quad w_{t} = -h_{34} = \color{red}{h_{3}} - h_{4} = (\color{red}{h_{3}} - \color{purple}{h_{4s}}) \eta_{t} \\
$
</br></br>
$
\therefore \color{green}{h_{4}} = \color{red}{h_{3}} - w_{t} = \color{red}{h_{3}} - (\color{red}{h_{3}} - \color{purple}{h_{4s}}) \eta_{t}
\\
\text{Condenser} \qquad q_{41} = \color{red}{h_{1}} - \color{green}{h_{4}} \\
$
</br></br>
$
\text{Reheat Parameters} \\
\color{red}{h_{5}} = \small \color{blue}{H_{2}O-\text{SAT-Table}_{h}\big[g]\Big(T_{5}\Big)}
\\
\color{green}{h_{6}} \text{ and } \color{purple}{h_{6s}} \Rightarrow \text{Same method as for } \color{green}{h_{4}} \text{ and } \color{purple}{h_{4s}}
$
</br></br>

#### Efficiency

$
\eta_{\text{Thermal}} = \dfrac{w_{\text{net}}}{q_{\text{in}}} 
\quad = \quad 
\dfrac{w_{t} - w_{p}}{q_{23}} 
\quad  \text{ or }  \quad 
\dfrac{w_{t1} + w_{t2} - w_{p}}{q_{23} + q_{45}} (\text{in the reheat case})
$

##### Note*: Area inside cycle of T-s diagram = $ w_{net} $ 
