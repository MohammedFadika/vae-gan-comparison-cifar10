# Comparative Study of VAEs and GANs for Generative Modeling on CIFAR-10

This repository contains the summary and findings of our study comparing various generative models (VAEs and GANs) on the CIFAR-10 dataset, exploring their performance, sample quality, and latent representations.

## Research Objectives

The primary objective of this project was to explore the comparative capabilities of Variational Autoencoders (VAEs) and Generative Adversarial Networks (GANs) as generative models. The study focused on:
- Sample quality assessment
- Latent representation analysis
- Training dynamics comparison
- Understanding how these models learn representations and generate data

The inclusion of β-VAE and WGAN-GP architectures specifically reflected our goal to investigate recent research on improving interpretability in VAEs and stability in GANs.

## Models Studied

Four main generative model architectures were implemented and compared:

- **Variational Autoencoder (VAE)**: Convolutional encoder and transposed convolutional decoder with a reparameterization trick
- **β-VAE (Beta-VAE)**: Modified VAE with a weighted KL divergence term
- **Generative Adversarial Network (GAN)**: Standard GAN with adversarial training between generator and discriminator
- **Wasserstein GAN with Gradient Penalty (WGAN-GP)**: Modified GAN structure with Wasserstein loss and gradient penalty

## Dataset

All models were trained on the CIFAR-10 dataset using normalized image inputs scaled to the range [-1, 1].

## Key Findings

Our experiments revealed several important insights:

1. **Sample Quality**: WGAN-GP produced the highest quality samples, followed by standard GAN, VAE, and β-VAE.
2. **Training Stability**: VAE models showed more stable training compared to GANs, with WGAN-GP significantly improving on standard GAN stability.
3. **Latent Space**: β-VAE provided more interpretable latent representations than standard VAE, enabling better control over generated features.
4. **Computational Requirements**: GAN-based models required more computational resources and careful hyperparameter tuning compared to VAE-based models.

## Requirements

The study used the following key dependencies:
- PyTorch
- torchvision
- NumPy
- Matplotlib
- scikit-learn

## Authors

This project was developed by:

- **Mohammed Fadika** - Academic City University College
- **Eyram Akligo** - Academic City University College
- **Regina Arthur** - Academic City University College

## License

This project is licensed under the MIT License. 