# Landslide Detection using Deep Learning and Uncertainty Estimation

## Overview

This project focuses on landslide segmentation from satellite imagery using deep learning techniques.

The repository contains two implementations:

1. Baseline Model: U-Net with ResNet34 encoder
2. Bayesian U-Net using Monte Carlo Dropout for uncertainty estimation

The project explores both accurate segmentation and model reliability in challenging geospatial regions.

---

## Implementations

### 1. U-Net with ResNet34 Encoder

#### Features
- U-Net architecture for semantic segmentation
- ResNet34 pretrained encoder
- Dice + BCE combined loss
- Transfer learning approach
- Efficient training using frozen encoder layers

#### Purpose
Establish a strong baseline model for landslide segmentation.

---

### 2. Bayesian U-Net with MC Dropout

#### Features
- Monte Carlo Dropout during inference
- Multiple stochastic forward passes
- Pixel-wise uncertainty estimation
- Confidence and error visualization

#### Purpose
Improve prediction reliability and identify uncertain regions in segmentation outputs.

---

## Dataset

The models were trained on a landslide segmentation dataset containing:
- Satellite imagery
- Binary landslide masks

---

## Technologies Used

- Python
- PyTorch
- OpenCV
- NumPy
- Matplotlib

---

## Outputs

The repository generates:
- Predicted segmentation masks
- Uncertainty maps
- Error maps
- Confidence-aware predictions

---

## Repository Structure

```bash
├── baseline_unet_resnet34.ipynb
├── bayesian_unet_mc_dropout.ipynb
└── README.md
