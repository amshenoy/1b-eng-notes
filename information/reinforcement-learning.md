# Reinforcement Learning

## State-Space Models


## Dynamic Programming

### Bellman Equation (Deterministic)

$
\small V_{s_{n}} = \text{Value of state} \ s_{n} \\
\small R(s_{n}, a) = \text{Reward for performing action} \ a \ \text{ in state } s_{n} \\
\small V_{s_{n+1}} = \text{Value of next state after taking action} \ a \\
$ 
$$ \large V_{s_{n}} = \max_{a} ( R(s_{n},a) + \gamma V(s_{n+1}) ) $$

### Bellman Equation (Stochastic)

$ 
\small P( s_{n}, a, s_{n+1}) = \text{Probability of moving to state } s_{n+1} \text{ given current state } s_{n} \text{ and action } a \\
\small \gamma = \text{Discount Factor} \\
$
$$ \large V_{s_{n}} = \max_{a} \Big( R(s_{n},a) + \gamma \sum_{s_{n+1}} P( s_{n}, a, s_{n+1}) V(s_{n+1}) \Big) $$

### Solutions

#### Policy Iteration
$$  $$

#### Value Iteration

## Q-Learning


## Deep Q-Learning





