# Stock Price Prediction
This project focuses on predicting stock prices using a Long Short-Term Memory (LSTM) model implemented in TensorFlow. The model is trained and tested on historical stock price data.<br> <br>
![1_hVQp6GjkMF0ynqCLPxSAgA](https://github.com/user-attachments/assets/1b4f228c-db48-4d0e-897f-9d86ac90f7ab)


## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Dataset](#dataset)
- [Data Processing](#data-processing)
- [Model-Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Visualization](#visualization)
- [Output](#output)
- [Conclusion](#conclusion)


## Introduction

The goal of this project is to predict the closing prices of a stock using historical stock price data. This project uses a Long Short-Term Memory (LSTM) neural network for time series forecasting.


## Installation

To run this project, you need to have Python and the following libraries installed:
- numpy
- pandas
- matplotlib
- datetime
- yfinance
- tensorflow
- scikit-learn
You can install the required libraries using pip:

```bash
pip install pandas datetime matplotlib yfinance numpy tensorflow scikit-learn
```


## Dataset

The dataset is fetched from Yahoo Finance using the yfinance library. In this project, we use the historical stock prices of TCS (Tata Consultancy Services) from January 1, 2010, to the present day.


## Data Processing
The data is processed as follows:
1. Load Data: Download the dataset using yfinance.
2. Drop Unnecessary Columns: Remove columns such as Date and Adj Close that are not needed for the prediction.
3. Plot Data: Visualize the closing prices and moving averages.
4. Split Data: Split the dataset into training and testing sets.
5. Normalize Data: Scale the data using MinMaxScaler.

## Model Architecture
The LSTM model consists of the following layers:
1. LSTM: 50 units, ReLU activation, return sequences
2. Dropout: 20%
3. LSTM: 60 units, ReLU activation, return sequences
4. Dropout: 30%
5. LSTM: 80 units, ReLU activation, return sequences
6. Dropout: 40%
7. LSTM: 120 units, ReLU activation
8. Dropout: 50%
9. Dense: 1 unit

## Training
The training process involves the following steps:
- Compile Model: Use Adam optimizer and Mean Squared Error loss function.
- Train Model: Fit the model on the training data for 100 epochs.

## Evaluation
The model is evaluated on the test set using Mean Absolute Error (MAE) and R2 score. These metrics provide insight into the model's accuracy and performance.
<br><code>MAE on test set: 6.54% </code> <br>
<code>R2 score: 0.9702856476907452 </code>

## Visualization
Visualizations are created to compare the actual and predicted stock prices. The following plots are generated:
- Moving Averages of 100 and 200 Days<br><br>
![Screenshot 2024-10-20 045029](https://github.com/user-attachments/assets/fac3aaf6-e84c-4082-9995-0c65820707f0)

   <br>
- R2 Score Bar Plot<br><br>
![Screenshot 2024-10-20 045001](https://github.com/user-attachments/assets/9a98e347-603e-47b1-9833-2e2d4648cc4b)

<br>
  
- Actual vs Predicted Scatter Plot<br><br>
![Screenshot 2024-10-20 045131](https://github.com/user-attachments/assets/a3c8238d-12f3-4398-a354-2b01f3f11d8d)

  <br>

## Output
- Original and Predicted Prices <br><br>
![Screenshot 2024-10-20 044819](https://github.com/user-attachments/assets/ee350967-e8aa-4c09-995b-b1afe229ff0f)




## Conclusion
This project successfully demonstrates the use of LSTM for stock price prediction. The model provides accurate predictions based on historical data, showcasing the potential of deep learning in time series forecasting.
