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
Conv2D (32 filters, 3×3, ReLU)

MaxPooling2D (2×2)

Conv2D (64 filters, 3×3, ReLU)

MaxPooling2D (2×2)

Flatten
Dense (128, ReLU)

Dropout (0.5)

Dense (10, Softmax)


### Training Configuration

| Parameter | Value |
|----------|-------|
| Optimizer | Adam |
| Loss Function | Categorical Cross-Entropy |
| Batch Size | 64 |
| Epochs | 10 |
| Evaluation Metric | Accuracy |

---

## Results

| Model | Training Accuracy | Testing Accuracy | Notes |
|-------|------------------|------------------|-------|
| CNN (this work) | ~85–90% | ~70–75% | Simple CNN, only normalization applied |

---

## Output Visualizations

All visualizations are available inside the `results/` directory:

- Training accuracy curve  
- Training loss curve  
- Confusion matrix  
- Classification report (Precision, Recall, F1-Score)  
- Sample predictions (model output vs. true labels)

---

## How to Run the Project

### 1. Install Dependencies
```bash
pip install -r requirements.txt

