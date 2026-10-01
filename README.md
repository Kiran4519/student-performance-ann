# Student Performance Prediction Using ANN

## Project Overview

This project demonstrates how an Artificial Neural Network (ANN) can predict student final marks using attendance percentage, daily study hours, and internal marks.

## Objective

To understand how a neural network learns relationships between input features and a numerical target using a regression model.

## Input Features

* Attendance (%)
* Study Hours per Day
* Internal Marks

## Target Variable

* Predicted Final Marks

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* TensorFlow / Keras
* Google Colab

## Methodology

1. Generate a synthetic student dataset.
2. Separate input features and target values.
3. Split the dataset into training and testing sets.
4. Standardize the input features.
5. Build an ANN using dense layers and ReLU activation.
6. Train the model using the Adam optimizer and mean squared error loss.
7. Evaluate predictions using MAE, RMSE, and R².
8. Predict marks for a sample student.

## Important Note

This project uses synthetic data generated for educational purposes. Its predictions are illustrative and should not be used to make real academic decisions.

## How to Run

Open `Student_Performance_ANN.ipynb` in Google Colab and run the cells from top to bottom.

