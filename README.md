# 🚗 Autonomous Driving with HDPE-InterFuser

> **Graduation Project** | Achieving **0.004 Validation Loss** on CARLA Benchmark.

[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org/)
[![WandB](https://img.shields.io/badge/Weights_&_Biases-FFBE00?style=for-the-badge&logo=WeightsandBiases&logoColor=white)](https://wandb.ai/)

## 📖 Overview
This project presents an enhanced autonomous driving model based on the **InterFuser** architecture. We introduce a novel **HyperDimensional Positional Encoding (HDPE)** mechanism that significantly improves the model's spatial awareness and safety in complex urban scenarios.

## 🌟 Key Features
* **HDPE Encoding:** Replaces standard positional encodings with a polar-coordinate based system using Gaussian saliency masking, focusing attention on critical road elements.
* **Transformer Backbone:** Uses ResNet + Transformer Encoder-Decoder to process multi-view camera inputs.
* **Advanced Loss Landscape:**
    * **Focal Loss:** Handles class imbalance in object detection.
    * **EIoU Loss:** Ensures precise bounding box regression.
    * **Weighted Waypoint Loss:** Prioritizes near-future trajectory accuracy.

## 📊 Results & Performance
The model was trained for **57+ Epochs** using a OneCycleLR scheduler.

| Metric | Result | Description |
| :--- | :--- | :--- |
| **Total Loss** | **0.0041** 🏆 | Indicates exceptional convergence and high precision. |
| **Traffic Accuracy** | **>99%** | Accurate detection of surrounding vehicles. |
| **Junction Accuracy** | **High** | Reliable classification of road junctions and signals. |

## 🛠️ How to Run
1. **Clone the repo:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/HDPE-Autonomous-Driving.git](https://github.com/YOUR_USERNAME/HDPE-Autonomous-Driving.git)
