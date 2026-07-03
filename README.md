# Cloud Removal from Satellite Imagery using Gated Attention U-Net

PyTorch implementation of a lightweight Gated Attention U-Net for cloud removal from satellite imagery using the RICE1 and RICE2 datasets.

This repository contains the official PyTorch implementation accompanying the paper:

**Cloud Removal from Satellite Imagery using a Lightweight Gated Attention U-Net**

The method introduces a Gated Attention U-Net architecture for paired optical satellite image cloud removal.

## Dataset

Experiments are performed using the publicly available RICE dataset.

- RICE1: 500 image pairs
- RICE2: 736 image pairs

Dataset Link:
https://www.kaggle.com/datasets/shubhank001/rice-remote-sensing-images-for-cloud-removal

## Experiments

### RICE1 Evaluation

Notebook: 01_RICE1_Attention_UNet_Ablation.ipynb

Includes:

- Modified U-Net baseline
- No Attention variant
- Light Attention U-Net
- Gated Attention U-Net
- Multi-seed ablation study


### RICE2 Evaluation

Notebook: 02_RICE2_Gated_Attention_UNet_Evaluation.ipynb


The final Gated Attention U-Net configuration is independently trained and evaluated on RICE2 using the same experimental settings.

## Requirements

- Python 3.x
- PyTorch
- torchvision
- numpy
- scikit-image
- matplotlib


## Citation
Raj Gaurav Mishra, Anuj Kumar, Sangeeta Pant, Ketan Kotecha, Ajith Abraham, Cloud Removal from Satellite Imagery using a Lightweight Gated Attention U-Net.

## License

MIT License
