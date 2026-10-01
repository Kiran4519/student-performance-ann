# Student Performance Prediction Using ANN

## Project Overview

This project uses an Artificial Neural Network (ANN) to predict a student's final examination marks based on three academic factors:

* Attendance
* Study Hours
* Internal Marks

The project demonstrates data preprocessing, feature scaling, ANN model development, training, evaluation, and prediction using Python and TensorFlow/Keras.

> **Note:** The dataset used in this project is synthetically generated for educational purposes. The model results should not be interpreted as real-world student performance accuracy.

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* TensorFlow
* Keras
* Google Colab / Jupyter Notebook

## Dataset

The dataset contains **500 synthetic student records** with the following variables:

| Feature        | Description                                          |
| -------------- | ---------------------------------------------------- |
| Attendance     | Student attendance percentage                        |
| Study_Hours    | Average study hours                                  |
| Internal_Marks | Internal examination marks                           |
| Final_Marks    | Target variable representing final examination marks |

## Data Preprocessing

The following preprocessing steps were performed:

1. Generated the synthetic dataset.
2. Separated input features and target variable.
3. Divided the dataset into training and testing sets using an 80/20 split.
4. Applied `StandardScaler` to normalize the input features.
5. Used the training data to fit the scaler and transformed both training and testing data.

## ANN Architecture

The Artificial Neural Network consists of:

```text
Input Layer: 3 Features
        ↓
Dense Layer: 16 Neurons + ReLU
        ↓
Dense Layer: 8 Neurons + ReLU
        ↓
Output Layer: 1 Neuron + Linear
```

### Model Configuration

* Optimizer: Adam
* Loss Function: Mean Squared Error (MSE)
* Evaluation Metric: Mean Absolute Error (MAE)
* Epochs: 100
* Batch Size: 16
* Validation Split: 20%

## Model Performance

The trained model produced the following results on the test dataset:

| Metric   | Result |
| -------- | -----: |
| MAE      |   4.62 |
| RMSE     |   5.67 |
| R² Score |  0.852 |

These results are based on the synthetic dataset created for this educational project.

## Sample Prediction

The trained ANN was used to predict the final marks of a sample student.

**Student Details:**

* Attendance: 85%
* Study Hours: 4
* Internal Marks: 78

**Predicted Final Marks: 71.16**

## Project Workflow

```text
Data Generation
      ↓
Data Preprocessing
      ↓
Train/Test Split
      ↓
Feature Scaling
      ↓
ANN Model Creation
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Student Performance Prediction
```

## How to Run

1. Open `Student_Performance_ANN.ipynb` in Google Colab or Jupyter Notebook.
2. Install the required libraries if necessary:

```bash
pip install -r requirements.txt
```

3. Run the notebook cells sequentially.
4. Review the training graph, evaluation metrics, and prediction output.

## Project Files

```text
Student_Performance_ANN.ipynb
README.md
requirements.txt
```

## Conclusion

This project demonstrates how an Artificial Neural Network can be used for a regression problem to estimate student final marks from academic factors. It provides practical experience with data preprocessing, feature scaling, neural network architecture, model training, evaluation metrics, and prediction.
