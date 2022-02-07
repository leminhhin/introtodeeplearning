# Lecture 4 Generative models

Unsupervised learning

## Autoencoders

input --(encode)--> compress --(decode)--> reconstruct input

learns from how good the reconstruction is

### VAE (Variational autoencoders)

- is an optimized AE
- uses regularization to introduce smoothness in information
- loss func = reconstruction loss + reularization term

## GAN (Generative Adversarial Networks)

- generator produces fake data from starting from noise
- discriminator identifies which are real, fake
- goal: discriminator cannot tell which are real

