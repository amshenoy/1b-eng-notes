# Psychrometry

# Psychrometry

## Gas Mixtures

State Properties ($ P, V $) - Moles Scaled

Material Properties ($ c_{p}, c_{v}, R, u, h, s $) - Mass Scaled

</br>

### Key Principles

#### Mass = Mr $ \times $ Moles
$ n_{i} = \dfrac{m_{i}}{M_{r_{i}}} $
#### Conservation
$ m_{T} = \sum_{i} m_{i} \quad (n_{T} = \sum_{i} n_{i}) \qquad P_{T} = \sum_{k} P_{k} $ 

</br>

### Derived Measures

#### Partial Pressure $ - \quad P_{k} = P_{T} \dfrac{n_{k}}{n_{T}} = P_{T} \dfrac{n_{k}}{ \sum_{i} n_{i} } = P_{T} \dfrac{\dfrac{m_{k}}{M_{r_{k}}}}{ \sum_{i} \dfrac{m_{i}}{M_{r_{i}}} } $

#### Partial Volume $ - \quad V_{k} = V_{T} \dfrac{n_{k}}{n_{T}} $

#### $ M_{r \ Equivalent} - \quad M_{r_{T}} = \dfrac{m_{T}}{n_{T}} = \dfrac{ \sum_{i} m_{i} }{ \sum_{i} n_{i} } = \dfrac{ \sum_{i} m_{i} }{ \sum_{i} \dfrac{m_{i}}{M_{r_{i}}} } $

#### $ R_{Equivalent} - \quad R_{T} = \dfrac{\bar{R}}{M_{r_{T}}} $ 

#### $ \rho_{Equivalent} - \quad \rho_{T} = \dfrac{P_{T}}{R_{T} \ T} $

#### $ V_{Equivalent} - \quad V_{T} = \dfrac{m_{T} R_{T} T}{P_{T}} $ 


## Hygrometry

#### Specific Humidity $ - \quad \omega = \dfrac{\dot{m_{v}}}{\dot{m_{a}}} = \dfrac{ M_{r \ v} \ P_{v} } { M_{r \ a} \ P_{a} } \quad \Big( = \dfrac{ R_{a} } { R_{v}} \dfrac{ P_{v} } { P_{a} } \Big) $
(Note*: $ P_{a} = P_{T} - P_{v} $)

#### Relative Humidity $ - \quad \phi = \dfrac{n_{v}}{n_{\text{v-sat}}} = \dfrac{P_{v}}{P_{\text{v-sat}}} \quad (\small {\text{Dewpoint:} \phi=1 \ \text{ie.} \ P_{v} = P_{v-sat}}) $

</br>

##### Problem-Solution Process (Water/Steam + Air)
$ \omega = \dfrac{\overbrace{18}^{M_{r} \ H_{2}O}}{\underbrace{29}_{M_{r} \text{Air}}} \dfrac{P_{v}}{ \underbrace{P_{T}}_{P_{atm}} - P_{v}} = \dfrac{\dot{m_{v}}}{\dot{m_{T}} - \dot{m_{v}}} $

</br>

$ \phi = \dfrac{ P_{v} }{
\\
\underbrace{P_{v-sat}}_{ \color{blue}{H_{2}O-\text{Table}_{P}[g](T)}}
}  
\qquad \Bigg(
P_{v} = \dfrac{\omega}{\omega + \dfrac{M_{r \ v}}{M_{r \ a}}} \text{ and } P_{a} = \dfrac{\omega}{\omega + \dfrac{M_{r \ a}}{M_{r \ v}}} \Bigg)
 $ 

