# Lecture 7 Evidential Deep Learning

## Uncertainty

- Aleatoric uncertainty (data uncertainty)
  - high when input data is noisy
  - cannot be reduced by adding data
- Epistemic uncertainty (model uncertainty)
  - high when missing training data
  - can be reduced by adding data

## Epistemic uncertainty

Solution: Bayesian NN

- Weight: use a probability distribution instead of a constant

## Bayesian NN

Bayes rules is not always computable

Use: aprroximations through sampling

Downsides:

- Slow: running the network T times for every input
- Memory, efficiency, calibration