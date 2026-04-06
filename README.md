# Deep-Learning-Based-Super-Resolution-for-Brain-MRI-Using-MedSRGAN
Deep Learning-Based Super-Resolution for Brain MRI Using MedSRGAN
This repository contains the implementation of MedSRGAN, a deep learning-based super-resolution model for enhancing Brain MRI images. The model is based on the Residual Whole Map Attention Network (RWMAN) and a discriminator network, trained in an adversarial manner to generate high-resolution MRI scans.

  📌 Project Overview
The MedSRGAN framework consists of:

Generator (RWMAN): A deep convolutional neural network with residual attention blocks to generate high-resolution MRI scans from low-resolution images.
Discriminator: A convolutional network that distinguishes real high-resolution images from generated ones.
Loss Functions: A combination of adversarial loss, perceptual loss, and SSIM-based structural loss.

  📂 Repository Structure
MedSRGAN/

data_pipeline.py # Preprocessing pipeline for data loading

discriminator.py # Discriminator network implementation

generator.py # Generator (RWMAN) network implementation

losses.py # Loss functions used for training

training.py # Training loop and model optimization

notebooks/ # Jupyter notebooks for training & evaluation

data/ # Folder to store dataset (not included in repo)

  🚀 Installation & Setup
1️⃣ Clone the Repository
git clone  cd Deep-Learning-Based-Super-Resolution-for-Brain-MRI-Using-MedSRGAN

Model Architecture

Generator (RWMAN) • Initial Convolution • Residual Whole Map Attention Blocks • Upsampling layers • Final Convolution Layer

Discriminator • Takes High-Resolution (HR) and Low-Resolution (LR) images as input • Passes through multiple convolutional blocks • Fully connected layers classify images as real or fake

Model_architecture

Performance Metrics

The model is evaluated using: • Peak Signal-to-Noise Ratio (PSNR) • Structural Similarity Index (SSIM) • Adversarial Loss & Perceptual Loss
