# Movie Recommendation System
This project implements a Movie Recommendation System using the MovieLens dataset. The goal is to recommend movies to users based on their past ratings.<br><br>
![03fb507e0ce5590520c511b35374785e](https://github.com/user-attachments/assets/7cf4911f-5752-49ef-b52f-db445d06c060)


## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Dataset](#dataset)
- [Data Processing](#data-processing)
- [Model](#model)
- [Training](#training)
- [Evaluation](#evaluation)
- [Output](#output)
- [Conclusion](#conclusion)


## Introduction

The goal of this project is to build a recommendation system that suggests movies to users based on their past ratings. This system uses collaborative filtering and Singular Value Decomposition (SVD) for recommendations.

## Installation

To run this project, you need to have Python and the following libraries installed:
- numpy
- pandas
- matplotlib
- requests

You can install the required libraries using pip:

```bash
pip install numpy pandas matplotlib requests
```


## Dataset

The MovieLens 100k dataset is used in this project. It consists of 100,000 ratings from 943 users on 1682 movies.



## Data Processing
The data is loaded and processed as follows:
1. Load Data: Download and unzip the dataset.
2. Read Data: Load the data files into Pandas DataFrames.
3. Preprocess Data: Merge datasets, create a utility matrix, and handle missing values.


## Model
The model uses collaborative filtering and SVD to recommend movies based on cosine similarity.

## Training
The training process involves the following steps:
- Load Dataset: Read and preprocess the data.
- Create Utility Matrix: Construct a matrix with users as rows and movies as columns, containing ratings.
- Handle Missing Values: Fill missing values in the utility matrix.
- Compute SVD: Perform Singular Value Decomposition to factorize the utility matrix.
- Calculate Similarities: Compute the cosine similarity between movies.
The model is trained over several cycles (epochs) to refine the recommendations.

## Evaluation
The system takes user input for a movie name and number of recommendations needed, then provides the top similar movies based on the trained model.


## Output

https://github.com/user-attachments/assets/d9291799-28f6-4856-a176-ea91c47f5863




## Conclusion
This project successfully demonstrates a movie recommendation system using collaborative filtering and SVD. The system provides accurate recommendations based on user input, showcasing the potential of recommendation algorithms in practical applications.
