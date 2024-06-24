# Handwritten-Digit-Recognition-with-LeNet5-Model-in-PyTorch

# Introduction
This project implements handwritten digit recognition using the LeNet-5 model in PyTorch. The workflow includes data preprocessing, model training, evaluation, and deployment through a Flask web application.

# Prerequisites
Python 3.7+
PyTorch
torchvision
Flask
NumPy
Matplotlib

# Data Preprocessing
## One Hot Encoding
Convert labels to one hot encoding if necessary.

## Data Reshaping
Reshape the data to fit the input dimensions required by the LeNet-5 model.

## Data Augmentation
Apply data augmentation techniques to increase the diversity of the training data.

## Data Sampling
Sample the dataset if needed to balance the classes or reduce the dataset size for quicker iterations.

# Model Implementation
## Neural Network
Implement the LeNet-5 model with appropriate layers.

## Initialize LeNet-5 Model
Initialize the LeNet-5 model architecture.

## Define Loss Function
Define the loss function, typically cross-entropy for classification tasks.

## Define Optimizer and Dense Layers
Define the optimizer (e.g., Adam, SGD) and configure the dense layers.

## Training and Testing
Load Data
Load the MNIST dataset into data loaders for training and testing.

## Train Model
Train the LeNet-5 model using the training data, adjusting weights through backpropagation.

## Test Model
Test the model using the test data to evaluate its performance.

## Evaluation and Improvement
Evaluate the model's performance and implement techniques to improve accuracy, such as hyperparameter tuning, additional data augmentation, or using ensemble methods.

# Flask Application
Deploy the trained LeNet-5 model using a Flask web application. In this setup, users can upload an image through a web interface, which is then received by the Flask server. The server preprocesses the image, applying necessary transformations like resizing and normalization. The preprocessed image is fed to three different models for prediction, each providing its own prediction. These predictions are then aggregated using a voting mechanism to determine the final class label. The predicted label is subsequently displayed to the user through the web interface.

# Conclusion
This project demonstrates the implementation of a handwritten digit recognition system using the LeNet-5 model in PyTorch and deployment through a Flask web application. The steps cover data preprocessing, model training, evaluation, and web deployment.
