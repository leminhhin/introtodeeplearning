# Lecture 5 Reinforcement Learning

policy pi: best action to take at state s

pi*(s) = argmax Q(s,a)

## Deep Q Learning

Q function: expected total reward

Input: state s

Output: vector of Q(s,a_i)

policy = best action maximizes Q function

Loss function: feed back best action

Downsides:

- Complexity:
  - only action space is discrete and small
- Flexibility:
  - cannot learn stochastic policies

## Policy Gradient Learning

input: state s

output: mean, variance

policy = sample from N(mean, variance)

Upsides:

- can model continuous action space

### Training

1. Init agent
2. Run a policy until termination
3. Record all states, actions, rewards
4. Decrease probability of actions that resulted in low reward
5. Increase probability of actions high reward

Loss = -logP(a_t|s_t)R_t

Gradient descent update: w' = w + loss