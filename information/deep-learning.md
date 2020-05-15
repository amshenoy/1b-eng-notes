# Deep Learning

## Perceptron

### Architecture
$ \sigma(x) = \text{Activation Function} \small\text{(Non-Linearity)} $
### $$ z = \sigma \big( \boldsymbol w \cdot \boldsymbol x + b \big) $$

### Training (Optimisation)
$ C(\boldsymbol w) = \text{Cost Function} \ \small\text{(Objective/Error/Loss Function to be minimised)} $

$$ \boldsymbol w^{*} = \arg\min_{\boldsymbol w} C(\boldsymbol w) $$ 
No analytical solution to this optimisation problem! Hence use optimisation algorithms like gradient descent.

### Hyperparameters

#### Common Activation Functions
##### $$
\text{Sigmoid} \qquad \dfrac{1}{1+e^{-x}}
\\
\text{Hyperbolic Tan} \qquad \tanh(x) = \dfrac{e^{x}-e^{-x}}{e^{x}+e^{-x}}
\\
\text{Softmax}
$$ 

#### Common Cost Functions
##### $$
\text{Cross-Entropy} \qquad CEE(\boldsymbol w) = - \sum_{i} y_{i} \log(z_{i}) \qquad \text{Classification}
\\
\text{Mean Squared} \qquad MSE(\boldsymbol w) = \dfrac{1}{N} 
 \sum_{i} (y_{i} - z_{i})^{2} \qquad \text{Regression}
\\
\text{Mean Absolute} \qquad MAE(\boldsymbol w) = \dfrac{1}{N} \sum_{i} |y_{i} - z_{i}| \qquad \text{Regression}
\\
\text{Sum Squared} \qquad SSE(\boldsymbol w) = \sum_{i} (y_{i} - z_{i})^{2} \qquad \text{Regression}
$$

## Multi-Layer Perceptron


## Convolutional Networks


