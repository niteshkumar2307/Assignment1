🧠 CIFAR-10 Image Classification using CNN

This project implements a Convolutional Neural Network (CNN) to classify images from the CIFAR-10 dataset using TensorFlow/Keras.
It includes data loading, preprocessing, model creation, training, evaluation, visualization, and confusion matrix generation.
📌 Project Overview

The CIFAR-10 dataset contains 60,000 color images (32×32×3), categorized into 10 classes:
airplane
automobile
bird
cat
deer
dog
frog
horse
ship
truck
The goal of this project is to build an accurate CNN classifier for these categories.
🚀 Features

Loads and preprocesses CIFAR-10 dataset
Custom CNN model built using Keras Sequential API
Training with validation split
Accuracy & loss visualization
Confusion matrix generation
Model saved as .h5
Modular code structure (dataset/model/train/evaluate)

▶️ How to Run the Project

1. Install Dependencies
    pip install -r requirements.txt
2. Train the Model
python src/train.py

This will:
Train the CNN
Save the model inside: saved_model/model.h5
Generate accuracy & loss plots in results/

📊 Evaluation
Run evaluation:
python src/evaluate.py

This will:
Load trained model
Predict on the test dataset
Generate a confusion matrix (results/confusion_matrix.png)

📈 Example Output

✔ Accuracy Curve
Shows training vs validation accuracy across epochs.

✔ Loss Curve
Shows training vs validation loss across epochs.

✔ Confusion Matrix
Displays class-wise classification performance.

🛠 Tech Stack
Python 3.x
TensorFlow / Keras
NumPy
Matplotlib
Seaborn
Scikit-learn

📌 Future Enhancements

Add Data Augmentation

Add Batch Normalization

Use deeper CNN architectures (ResNet, VGG, MobileNet)

Hyperparameter tuning

Export model to TensorFlow Lite
