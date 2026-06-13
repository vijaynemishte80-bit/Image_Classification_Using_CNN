Cat and Dog Image Classification Using CNN

Overview

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify images as either Cats or Dogs. The dataset is created from the CIFAR10 dataset by filtering only cat and dog classes. Data augmentation techniques are applied to improve model generalization and performance.

Dataset

- Dataset: CIFAR10
- Classes Used:
  - Cat
  - Dog
- Training Data: Cat and Dog images from CIFAR10 training set
- Testing Data: Cat and Dog images from CIFAR10 test set

Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Scikit Learn
- Deep Learning

Key Features

- Image preprocessing and normalization
- Data augmentation
  - Random Horizontal Flip
  - Random Rotation
- Custom dataset creation
- CNN based image classification
- Model training and evaluation
- Performance metrics generation
- Confusion Matrix and Classification Report

Model Architecture

Convolutional Layers

1. Conv2D (3 → 32) + ReLU + MaxPooling
2. Conv2D (32 → 64) + ReLU + MaxPooling
3. Conv2D (64 → 128) + ReLU + MaxPooling

Fully Connected Layers

- Linear Layer (2048 → 256)
- ReLU Activation
- Output Layer (256 → 2)

Training Configuration

Parameter| Value
Optimizer| Adam
Loss Function| Cross Entropy Loss
Epochs| 10
Batch Size| 64

Evaluation Metrics

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report
- Validation Loss

Project Workflow

1. Load CIFAR10 Dataset
2. Filter Cat and Dog Images
3. Apply Data Augmentation
4. Build CNN Model
5. Train the Model
6. Evaluate Performance
7. Generate Metrics and Reports

Results

The CNN model successfully learns features from cat and dog images and performs binary image classification with strong accuracy on the test dataset.

Future Improvements

- Transfer Learning using ResNet or VGG
- Hyperparameter Tuning
- More Data Augmentation Techniques
- Model Deployment using Flask or Streamlit
- Real Time Image Classification

Author

Developed as a Deep Learning and Computer Vision Project using PyTorch.
