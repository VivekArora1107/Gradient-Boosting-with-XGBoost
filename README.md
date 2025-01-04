# Gradient Boosting Machines (GBM) with XGBoost and LightGBM

This notebook demonstrates the use of Gradient Boosting Machines (GBM) using XGBoost and LightGBM for predicting sales data. The dataset used is the Rossmann Store Sales dataset from Kaggle.

## Table of Contents
1. [Introduction](#introduction)
2. [Setup](#setup)
3. [Data Loading](#data-loading)
4. [Data Preprocessing](#data-preprocessing)
5. [Feature Engineering](#feature-engineering)
6. [Model Training](#model-training)
7. [Evaluation](#evaluation)
8. [Visualization](#visualization)
9. [K-Fold Cross Validation](#k-fold-cross-validation)
10. [Hyperparameter Tuning](#hyperparameter-tuning)
11. [Final Model and Predictions](#final-model-and-predictions)
12. [Submission](#submission)

## Introduction
Rossmann operates over 3,000 drug stores in 7 European countries. The task is to predict 6 weeks of daily sales for 1,115 stores located across Germany. Reliable sales forecasts enable store managers to create effective staff schedules that increase productivity and motivation.

## Setup
Install the required libraries:
```bash
pip install xgboost lightgbm graphviz scikit-learn opendatasets
```

## Data Loading
Load the dataset from Kaggle using the `opendatasets` library.

## Data Preprocessing
- Merge the training and store datasets.
- Handle missing values.
- Encode categorical variables.
- Scale numerical features.

## Feature Engineering
- Extract date features (day, month, year, week of year).
- Calculate competition open months.
- Identify promo months.

## Model Training
Train the XGBoost model with the processed data.

## Evaluation
Evaluate the model using RMSE (Root Mean Squared Error).

## Visualization
Visualize the decision trees and feature importance.

## K-Fold Cross Validation
Use K-Fold Cross Validation to assess the model's performance.

## Hyperparameter Tuning
Tune hyperparameters like `n_estimators`, `max_depth`, and `learning_rate` to improve model performance.

## Final Model and Predictions
Train the final model on the entire training set with the best hyperparameters and make predictions on the test set.

## Submission
Prepare the submission file for Kaggle.

## Usage
Run the notebook cells sequentially to reproduce the results.

## License
This project is licensed under the MIT License.
