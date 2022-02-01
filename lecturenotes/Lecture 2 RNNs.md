# Lecture 2 Recurrent neural networks

## Neurons with recurrence

- is used for sequence problem (video, sound, text)
- maintains a memory containing previous states
- ouput is based on input and past memories

## Word representing

### Embedding

transform data to a vector

- one hote encoding: binary vector
- learned embedding: word2vec

## Standard RNN Gradient

Problems:

- Exploding gradients (many values > 1)
- Vanishing gradients (many values < 1)

Solution:

- Exploding gradients: scale big gradients
- Vanishing gradients:
  - Activation function using RELU
  - Weight init to 0
  - Network architecture: gated cell

## Long short term memory

- uses gated cell to track information throughtout many time steps
- gated cell: control what info is passed through
  - forget: get rid of irrelevant info
  - store relevant info from current input
  - selectively update cell state
  - output a filtered version of cell state