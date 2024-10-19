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
- [Output](#output)
- [Conclusion](#conclusion)


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

The MNIST dataset is used for training and evaluating the model. It consists of 60,000 training images and 10,000 testing images. Each image is a 28x28 pixel grayscale image of a digit.<br><br>
![MNIST-0000000001-2e09631a_09liOmx](https://github.com/user-attachments/assets/f5987023-9524-4bf8-a4bb-2156d509c9a7)



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
<br><code>Test loss: 0.0241182143806917 </code> <br>
<code>Test accuracy: 0.9900000095367432 </code>
## Visualization
The training process and results are visualized using Matplotlib. The following plots are generated:
- Model Accuracy
- Model Loss<br><br>
![Screenshot 2024-10-20 023325](https://github.com/user-attachments/assets/3b3aa299-bff0-411d-9a24-7a552cf3dd58)


## Output
![Screenshot 2024-10-20 023427](https://github.com/user-attachments/assets/30143ba6-ad03-4060-9e10-aecae23a104d)


## Conclusion
This project successfully demonstrates the use of Convolutional Neural Networks (CNNs) for recognizing handwritten digits. By leveraging the power of TensorFlow and the well-known MNIST dataset, we trained a model that achieved high accuracy in classifying digits from 0 to 9.

Throughout the project, we:
- Implemented a robust CNN architecture designed for image recognition.
- Preprocessed and normalized the MNIST dataset to improve training efficiency.
- Trained the model using the Adam optimizer and sparse categorical crossentropy loss function.
- Visualized the training process to monitor accuracy and loss.
- Evaluated the model on the test set to ensure generalization.

The results show that our model is capable of accurately recognizing handwritten digits, which can be applied to various practical applications such as digitizing handwritten notes, automating data entry, and more.

