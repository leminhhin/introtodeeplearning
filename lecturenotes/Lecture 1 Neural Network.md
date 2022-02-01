# Lecture 1 Neural network

## Perceptron

3 steps:

- dot product (input and weight)
- add bias
- activation function

### Activation function

- is a non linear function
- example: sigmoid, relu
- to introduce non linearities to the network (data in real world is non linear)

## Loss function

- empirical loss: total loss over entire dataset
- binary cross entropy loss:
  - used for 0 to 1 probability output
  - calculate how far ground truth to predicted
- mean squared error loss: used for output continuous real numbers

## Loss optimization

### Gradient descent

- Loop
  - Compute gradient (backpropagation)
  - Update weights

### Optimized gradient descent

- Problem with traditional GD: converge to local minimum
- Solution: adaptive learning rate
  - SGD
  - Adam

## Batching

- smoother convegence
- faster training

## Overfitting

Problem: model is too complex -> can not generalize data

Solution: Regularization

### Regularization

- dropout: during traning, randomly set some activations to 0
- early stopping: stop training when detecting overfit test data