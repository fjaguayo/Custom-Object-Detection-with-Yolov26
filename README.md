# Custom Object Detection with YOLOv26: Industrial Components

## Overview
This project demonstrates a complete professional workflow for developing a custom object detection system using **YOLOv11**, the latest state-of-the-art iteration from Ultralytics. 

The primary goal was to overcome the limitations of generic pre-trained models by training a neural network to recognize specific industrial objects: **Green Circles, Brown Circles, and Green Squares**.

## Tech Stack
* **Model:** YOLOv26s (Small) - Optimized for a balance between speed and accuracy.
* **Framework:** Ultralytics.
* **Environment:** Google Colab with NVIDIA T4 GPU.
* **Dataset Management:** Roboflow.
* **Libraries:** Python, OpenCV, Torch.

## Methodology
### 1. Dataset Preparation
* **Data Acquisition:** Images were captured from multiple angles, lighting conditions, and backgrounds to ensure model robustness.
* **Labeling:** Manual bounding box annotation was performed using Roboflow.
* **Data Splitting:** 70% Training, 20% Validation, and 10% Testing.

### 2. Transfer Learning
Instead of training from scratch, I utilized **Transfer Learning**. By "fine-tuning" a model pre-trained on the COCO dataset, high accuracy was achieved with a smaller custom dataset.

### 3. Training Configuration
* **Epochs:** 15.
* **Image Size:** 640px.
* **Optimization:** Monitored via Loss Curves and Confusion Matrices to prevent overfitting.

## Results
The model successfully tracks objects in real-time
