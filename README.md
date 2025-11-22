🖼️ CIFAR-10 Image Classification Using Convolutional Neural Networks (CNN)

📌 Overview

This project implements a Convolutional Neural Network (CNN) model for classifying images from the CIFAR-10 dataset as part of a deep learning assignment.

The task involved:

Selecting a publicly available dataset

Applying an ML/DL algorithm covered in class

Implementing the solution in Python

Providing code, README, and report

The model achieves:

Metric	Value
Training Accuracy	~85–90%*
Testing Accuracy	~70–75%*

(*Performance varies based on training duration and hyperparameters.)

Simple normalization was used.
No augmentation techniques were applied.

📊 Dataset

Name: CIFAR-10 – 10-Class Natural Image Dataset

Source: Google Dataset Search / Keras Datasets

Dataset Details

60,000 color images

32×32 resolution, RGB

10 classes:
airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

50,000 training images

10,000 test images

Preprocessing

Pixel values normalized: 0–255 → 0–1

Resized/reshaped to (32, 32, 3)

Labels converted to one-hot encoded vectors

Dataset split into:

Training

Validation

Testing

📝 Abstract

The CIFAR-10 dataset is a widely used benchmark for evaluating image classification algorithms.
This project implements a simple yet effective CNN using Python and TensorFlow/Keras to classify CIFAR-10 images.

Despite having a shallow architecture and no augmentation, the network achieves strong performance with more than 70% testing accuracy, demonstrating effective feature learning through convolutional layers.

⚙️ Methodology
1️⃣ Preprocessing

Loaded dataset using Keras

Converted pixel values to floating-point

Scaled pixel values to [0, 1]

One-hot encoded labels

2️⃣ CNN Architecture

The CNN contains the following layers:

Conv2D (32 filters, 3×3, ReLU)
MaxPooling2D (2×2)

Conv2D (64 filters, 3×3, ReLU)
MaxPooling2D (2×2)

Flatten
Dense (128, ReLU)
Dropout (0.5)
Dense (10, Softmax)


This architecture is highly suitable for CIFAR-10, offering a balance between performance and computational efficiency.

3️⃣ Training

Optimizer: Adam

Loss: Categorical Cross-Entropy

Batch Size: 64

Epochs: 10

Metrics: Accuracy

✅ Results
Model	Training Accuracy	Testing Accuracy	Notes
CNN (This Work)	85–90%	70–75%	Simple CNN, normalized inputs

All visualizations are saved in the results/ folder.

📷 Output Visualizations

This project includes the following outputs:

🔹 Training Accuracy Curve

Shows improvement in accuracy over epochs.

🔹 Training Loss Curve

Depicts loss reduction during training.

🔹 Confusion Matrix

Provides class-wise performance evaluation.

🔹 Classification Report

Precision, Recall, and F1-Score for all 10 classes.

🔹 Sample Predictions

Visual representation of model predictions vs. true labels.

All output files are available inside:
