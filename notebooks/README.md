# Notebooks

This folder contains the implementation notebooks and pretrained model checkpoint used for reproducing the experiments reported in the paper:

**Cloud Removal from Satellite Imagery using a Lightweight Gated Attention U-Net**

## Files

### 1. 01_RICE1_Attention_UNet_Ablation.ipynb

This notebook contains the complete RICE1 experimental workflow, including:

- Modified U-Net baseline evaluation
- Attention U-Net variants:
  - No Attention
  - Light Attention
  - Gated Attention
- Multi-seed ablation experiments
- Quantitative evaluation using PSNR, SSIM, MAE, MSE, and inference time

The experiments reproduce the RICE1 results and ablation analysis reported in the manuscript.

---

### 2. 02_RICE2_Gated_Attention_UNet_Evaluation.ipynb

This notebook evaluates the final Gated Attention U-Net configuration on the RICE2 dataset.

The same architecture, preprocessing steps, loss function, and training configuration are used to validate the robustness of the proposed model on more challenging cloud conditions.

---

### 3. best_gated_attention_unet_rice1.pt

This file contains the pretrained PyTorch checkpoint of the Gated Attention U-Net model trained on the RICE1 dataset.

The checkpoint corresponds to the best-performing model selected from three independent training runs with different random seeds.

It is provided to support direct model loading, inference, and reproducibility without requiring retraining.

## Dataset

The experiments use the publicly available RICE dataset:

- RICE1: 500 paired cloudy/cloud-free images
- RICE2: 736 paired cloudy/cloud-free images
