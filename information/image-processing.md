# Image Processing

## Edge Detection
### $$ \nabla S = \nabla G_{\sigma} * I $$

**Meaning**

Gradient of the smoothed image = Gradient of the convolution of a gaussian filter with the image 

##### Note*: Purpose of the gaussian filter is to remove noise

**Objective** 

We are trying to find where the $ \nabla S $ equals 0 (ie. is a minimum, ie. detected edges).

</br>

### 1D Edge Detection
### $$ s^{'}(x) = g^{'}_{\sigma}(x) * i(x) $$ 
**Convolution Derivative Theorem:**
$ \dfrac{d}{dx} \Big( s(x) \Big) = \dfrac{d}{dx} \Big( g_{\sigma}(x) * i(x) \Big)
= \dfrac{dg_{\sigma}(x)}{dx} * i(x) $ 

$$ \therefore s^{'}(x) = g^{'}_{\sigma}(x) * i(x) $$
$$ \text{Also} \ \therefore s^{''}(x) = g^{''}_{\sigma}(x) * i(x) $$
A significant computation speedup!!!

</br>

### 2D Edge Detection
### $$ \nabla S = \nabla G_{\sigma} * I $$

$$ S(x, y) = G_{\sigma}(x, y) * I(x, y) = \iint G_{\sigma}(u, v) I(x-u, y-v) \ du \ dv $$

A significant computation speedup from using the 1D gaussian functions:
$$ G_{\sigma}(x, y) * I(x, y) = g_{\sigma}(x) * ( g_{\sigma}(y) * I(x, y) ) $$

</br>

##### Note*: $ \dfrac{\partial S}{\partial x} = \dfrac{S(x+1, y) - S(x-1, y)}{2} = \text{ Rows of } S(x, y) * [\frac{1}{2},0,-\frac{1}{2}]$


