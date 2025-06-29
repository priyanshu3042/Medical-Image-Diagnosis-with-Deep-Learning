# Medical Image Diagnosis with Deep Learning
> A deep learning-based medical image classification system using CNN and transfer learning to detect **Pneumonia** from chest X-ray images.
---
##  Project Overview

This project leverages deep learning and medical imaging to detect **Pneumonia** from chest X-ray scans. Using the **Chest X-ray Pneumonia dataset** from Kaggle, a **transfer learning-based CNN model** (MobileNetV2) is trained to classify images into `Normal` and `Pneumonia` categories.

---

##  Features

-  Transfer Learning using MobileNetV2
-  Data Augmentation for robustness
-  Grad-CAM for visualizing model attention (explainable AI)
-  High accuracy with lightweight model
-  Easy-to-deploy via Google Colab / Streamlit

---

##  Dataset

- Source: [Kaggle - Chest X-ray Pneumonia Dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)
- Size: ~2 GB (≈5,800 images)
- Classes: 
  - `Normal` (healthy patients)
  - `Pneumonia` (infected patients)
  - https://drive.google.com/drive/folders/1tGTyHeg-3m6JAl6458ENgn-Hr-bLPEDv?usp=drive_link

## Structure

chest_xray/
├── train/
├── val/
└── test/

##  Model Architecture

-  **Base Model:** MobileNetV2 (pre-trained on ImageNet)
-  GlobalAveragePooling + Dense layers
-  Activation: Sigmoid
-  Loss: Binary Cross-Entropy
-  Optimizer: Adam (LR = 1e-4)
-  Metrics: Accuracy, Precision, Recall

## Results
Metric	                 Score
Accuracy	              94–97%
Precision	               High
Recall	              High (important in medical)
Inference Time	       ~20ms/image

## License
This project is licensed under the MIT License.
Feel free to use, share, and modify with attribution.





