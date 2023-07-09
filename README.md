# Polynomial Regression Model

This repository contains code for training and evaluating a polynomial regression model using the provided dataset. 
The model is implemented in Python and utilizes the scikit-learn library.

## Files

- `linear_regression.py`: This file contains the main code for training and evaluating the polynomial regression model.

## Prerequisites

To run the code in this repository, you need to have the following dependencies installed:

- Python 3.x
- NumPy
- scikit-learn
- matplotlib

## Dataset

The dataset used for training and testing the model is stored in two files:

- `x_dataset.npy`: This file contains the input features (x values) of the dataset.
- `y_dataset.npy`: This file contains the corresponding target values (y values) of the dataset.

## Training and Evaluation

The polynomial regression model is trained and evaluated using the following steps:

1. The dataset is loaded using the `DatasetLoader` class.
2. The dataset is split into training and testing sets using a test size of 20% and a random seed of 42.
3. The model is trained and evaluated for different degrees of polynomial features.
4. For each degree, the input arrays are reshaped and polynomial features are created using `PolynomialFeatures` from scikit-learn.
5. The model is trained using linear regression (`LinearRegression` from scikit-learn) on the polynomial features.
6. Predictions are made on the test set using the trained model.
7. Mean squared error (MSE) and R-squared (R2) scores are computed to evaluate the model's performance.
8. Actual and predicted values are plotted using matplotlib for visualization.

## Results

The results of the polynomial regression model are displayed through scatter plots for each degree. 
The plots show the actual values (in blue) and the predicted values (in red) on the test set. 
The degree of the polynomial, MSE, and R2 scores are also shown in the plot title.
