## Lacuna-Solar-Survey-Challenge
# Overview
This repository contains my solution to the **[Lacuna-Solar-Survey-Challenge](https://zindi.africa/competitions/lacuna-solar-survey-challenge)**.  
The task: **predict the number of solar panels and solar boilers** in satellite and drone images from Madagascar.  
The challenge supports renewable energy tracking and sustainable development.
# Approach
 **Models:**  
  - DenseNet-121 (baseline)  
  - EfficientNet-B4 (high-capacity)  
  - ResNet-50 (experimental Faster R-CNN backbone)  
  **Data augmentation:** Albumentations (crop, flip, color jitter, distortion, dropout)  
  **Training setup:**  
  - Loss: L1 (MAE), directly aligned with competition metric
  - Optimizer: AdamW  
  - Early stopping + best checkpointing  
