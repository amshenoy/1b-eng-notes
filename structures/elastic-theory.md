## Force Method for Trusses

### Number of Redundancies
$$ n - m = b + r - Dj $$
$ n = Redundancies $ - Number of Redundancies </br>
$ m = 0 $ - Number of Mechanisms (Static Trusses $ \therefore m = 0 $) </br>
$ b = Bars $ - Number of Bars </br>
$ r = Restraints (Reactions) $ - Number of Reaction Forces </br>
$ D = 2 $ - Number of Dimensions (2D Trusses $ \therefore D = 2 $)</br>
$ j = Joints $ - Number of Joints

### $$ \therefore n = b + r - 2j $$

### Tensions
$$
\underline{t} = \underline{t_{0}} + \sum_{i=0}^{n} x_{i}\underline{s_{i}} \quad (n = \text{Num of Redundancies})
$$
$ \underline{t_{0}} $ - $ \text{Applied loads} $ with $ \text{redundant bars} = 0 \quad $ - Particular Solution </br>
$ \underline{s_{i}} $ - $ \text{Self-Stress (No loads) } $ where $ \text{redundant bar}_{i} = 1 $ and $ \text{other redundant bars} = 0 \quad $ - Homogenous Solution </br>

### Flexibility Matrix
In the truss case, the flexibility matrix is a diagonal matrix.
$$
F = 
\begin{pmatrix}
\frac{L_{1}}{A_{1} E_{1}} & ... & 0 \\
\vdots & \ddots & \vdots \\
0 & ... & \frac{L_{i}}{A_{i} E_{i}}
\end{pmatrix}
$$
As the flexibility matrix is diagonal we can solely consider the diagonal vector.
$$ \underline{f} = \begin{pmatrix} \frac{L_{1}}{A_{1}E_{1}} \\ \vdots \\ \frac{L_{i}}{A_{i}E_{i}} \end{pmatrix}
(= \frac{\underline{L}}{\underline{A}\underline{E}})
$$

### Extensions
Now we can calculate the extensions by multiplying the flexibility matrix with the parameterised tensions. Alternatively for a diagonal matrix, this is the same as the hadamdard product of the diagonal vector with the parameterised tensions.
$$ \underline{e} = F \underline{t} = \underline{f} \circ \underline{t} $$ 

Note that if a truss has pre-stress (ie. pre-extension), then the modified equation for extension is the following:

$$ \underline{e} = \underline{f} \circ \underline{t} + \underline{e_{0}} $$

### Tension Calculation
We can now use virtual work to calculate the values of $ x_{i} $ which we will then use to calculate the tensions.
</br>
The virtual work equation simplifies down to the following:
$$ \underline{s_{i}} \cdot \underline{e} = 0 $$ 

 We can use the above equation for each $ \underline{s_{i}} $ to find each $ x_{i} $ which we can then substitute into $ \underline{t} $ to find the values of tensions for each of the bars.

### Point Displacement at Applied Loads
$$ \underline{P}^{*} \cdot \underline{\delta} =\underline{t}^{*} \cdot \underline{e} $$

$ \underline{P}^{*} \text{ = } \underline{1} $
