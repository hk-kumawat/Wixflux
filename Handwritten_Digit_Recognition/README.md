# Handwritten Digit Recognition

This project focuses on recognizing handwritten digits using a Convolutional Neural Network (CNN) implemented in TensorFlow. The model is trained and tested on the MNIST dataset, which contains 70,000 grayscale images of handwritten digits (0-9).

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Visualization](#visualization)
- [Results](#results)
- [Output](#contributing)

## Introduction

The goal of this project is to create a model capable of recognizing handwritten digits with high accuracy. This model can be used in various applications such as digitizing handwritten notes, automatic number plate recognition, and more.

## Installation

To run this project, you need to have Python and the following libraries installed:
- TensorFlow
- NumPy
- Matplotlib

You can install the required libraries using pip:

```bash
pip install tensorflow numpy matplotlib
```


## Dataset

The MNIST dataset is used for training and evaluating the model. It consists of 60,000 training images and 10,000 testing images. Each image is a 28x28 pixel grayscale image of a digit.


## Model Architecture
1. The Convolutional Neural Network (CNN) consists of the following layers:
2. Conv2D: 64 filters, kernel size (2,2), ReLU activation
3. MaxPooling2D: pool size (2,2)
4. Dropout: 30%
5. Conv2D: 32 filters, kernel size (2,2), ReLU activation
6. MaxPooling2D: pool size (2,2)
7. Dropout: 30%
8. Flatten
9. Dense: 256 units, ReLU activation
10. Dropout: 50%
11. Dense: 10 units, Softmax activation


## Training
The model is trained using the Adam optimizer and sparse categorical crossentropy loss function. The training process includes:
- Batch size: 60
- Epochs: 10
- Validation split: 30%

## Evaluation
The model is evaluated on the test set to measure its performance. The evaluation metrics include accuracy and loss.

## Visualization
The training process and results are visualized using Matplotlib. The following plots are generated:
- Model Accuracy
- Model Loss

## Results
The model achieved an 0.9900000095367432 test accuracy score on the test set.

## Output
