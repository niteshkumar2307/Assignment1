# CIFAR-10 Image Classification Using Convolutional Neural Networks (CNN)

## Overview
This project implements a Convolutional Neural Network (CNN) to classify images from the CIFAR-10 dataset into 10 natural image categories. The objective of this assignment was to apply a deep learning algorithm covered in class using Python and evaluate its performance on a publicly available dataset.

The model achieves strong performance without data augmentation, demonstrating the ability of CNNs to learn visual features effectively.

---

## Dataset Information

**Dataset:** CIFAR-10  
**Source:** Keras / Google Dataset Search

| Property | Value |
|---------|-------|
| Total Images | 60,000 |
| Training Images | 50,000 |
| Test Images | 10,000 |
| Image Size | 32 × 32 × 3 (RGB) |
| Number of Classes | 10 |
| Classes | airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck |

### Preprocessing Steps
- Pixel value normalization (0–255 → 0–1)
- Reshaped to `(32, 32, 3)`
- Labels converted to one-hot encoded vectors
- Dataset split into training, validation, and testing subsets

---

## Model Architecture

