# lightweight-cnn-for-flood-region-detection
### Knowledge Distillation for Efficient Semantic Segmentation

## overview
This repository contains a curated implementation of my **Master’s thesis**, which focuses on developing **lightweight convolutional neural networks (CNNs)** for **flooded region detection in Unmanned Aerial Vehicles(UAV) images**.  

The project explores how **knowledge distillation** can be used to transfer knowledge from a high-capacity teacher model to a compact student model, enabling efficient inference while maintaining competitive performance.

This work is motivated by real-world deployment constraints, where **computational efficiency, memory usage, and inference speed** are critical.

## problem statement 
Flood detection plays an important role in disaster response and environmental monitoring.  
However, state-of-the-art deep learning models are often **too large and computationally expensive** for deployment on edge devices or in resource-constrained environments.

**Objective:**
- Achieve accurate flood segmentation
- Reduce model size and computational cost
- Preserve performance through knowledge distillation

## Dataset
This project uses the **FloodNet** dataset (Rahnemoonfar et al., 2021), an open-source benchmark for flood segmentation from aerial imagery.

- High-resolution aerial images
- Pixel-level segmentation annotations
- Task: Flood vs. non-flood region segmentation
Standard preprocessing and data augmentation were applied.

## Approach
- High-capacity **teacher model(PSPNet)** trained for accurate segmentation
- Compact **student model(MobileNet)** optimized for efficiency
- Knowledge distillation using soft targets from the teacher
- Evaluation of accuracy vs. computational efficiency trade-offs

---

## Results
- Significant reduction in model parameters and computational cost
- Lightweight models achieve **comparable segmentation accuracy**
- Knowledge distillation proved effective for flood mapping tasks

Metrics:
- Performance: Mean Intersection over Union (MeanIoU)
- Computational cost: Memory size & training time + inference time

---

## Key Takeaways
- Knowledge distillation enables compact models to retain spatial understanding
- Lightweight architectures are suitable for real-time and edge deployment
- Efficiency should be evaluated alongside accuracy, not separately
 
