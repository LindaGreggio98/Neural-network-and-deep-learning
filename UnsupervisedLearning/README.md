# Autoencoders and Variational Autoencoders — FashionMNIST

This repository contains the implementation and analysis of **autoencoders** and **variational autoencoders (VAEs)** trained on the **FashionMNIST** dataset.

The main goal of this project is to explore how autoencoders compress and reconstruct image data, and to evaluate their behavior as generative models. We investigate:
- the effect of **latent space dimension** on reconstruction quality,
- visualization of the latent space,
- sampling from latent space to *generate new images*,
- and the organization of latent features for downstream tasks like classification.

We also implement a **Variational Autoencoder** to achieve a more regularized latent space that enables meaningful generative sampling.

## Features

- Fully-connected and convolutional autoencoders  
- Variational Autoencoder (VAE)  
- Reconstruction and generative experiments  
- Latent space visualization  
- Linear classification on frozen latent representations

## Experiments

The following analyses are included:

1. **Reconstruction with different latent dimensions**: comparison of reconstruction loss and visual quality as latent space size changes.

2. **Latent Space Visualization**: 2D projection of latent codes with class labels.

3. **Generative Sampling**: random samples decoded from latent space for both autoencoders and VAEs.

4. **Classification on Latent Features**: train a linear classifier on the encoder bottleneck and compare results with a CNN classifier.

## Dataset

- **FashionMNIST**
  - 60,000 training images
  - 10,000 test images
  - 10 clothing categories
  - Grayscale images of size 28×28
