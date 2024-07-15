# House Price Prediction Project

Welcome to my House Price Prediction project! This repository contains a comprehensive solution to predict house prices using various machine learning algorithms. Here's a detailed overview of the project:

## Project Overview

I have implemented a variety of machine learning models to predict house prices based on a dataset containing detailed features of houses.

## Project Highlights

### Data Loading and Preprocessing

- Loaded the dataset and converted the date column to a datetime object for easier manipulation.
- Extracted the year and month from the date and dropped unnecessary columns (`id` and `date`).
- Handled missing values by dropping any rows with NaNs.

### Feature and Target Separation

- Split the dataset into features (`X`) and the target variable (`y`), where `y` represents the house price.

### Train-Test Split

- Split the data into training and testing sets to evaluate model performance on unseen data.

### Model Training and Evaluation

- Defined a helper function `evaluate_model()` to train each model and calculate RMSE and R² scores for evaluation.
- Implemented the following models:
  - Linear Regression
  - Decision Tree
  - Random Forest
  - XGBoost
  - Support Vector Machine (SVR)
  - k-Nearest Neighbors
  - Neural Networks (using Keras and TensorFlow)

### Model Performance

- **Linear Regression**: RMSE = 212036.1654, R² = 0.7026
- **Decision Tree**: RMSE = 211372.5139, R² = 0.7045
- **Random Forest**: RMSE = 150257.8166, R² = 0.8507
- **XGBoost**: RMSE = 142414.6545, R² = 0.8658 **(Best Model)**
- **Support Vector Machine**: RMSE = 400942.5278, R² = -0.0634
- **k-Nearest Neighbors**: RMSE = 186712.8618, R² = 0.7694
- **Neural Network**: RMSE = 191165.3486, R² = 0.7583

### Model Selection

- Selected the best-performing model based on RMSE, which is XGBoost.

### Visualization

- Plotted actual vs. predicted prices for each model to visually inspect their performance.
- Visualized feature importance for models that provided this information to understand which features influence house prices the most.

### Feature Relationships

- Visualized the relationships between all independent features and the target variable (house prices) using scatter plots to explore correlations.

### User Interaction

- Implemented user interaction to predict house prices based on input features such as number of bedrooms, bathrooms, and square footage.

## Getting Started

To get started with this project, clone the repository and follow the instructions in the `README.md` file to set up your environment and run the code.

## Technologies Used

- Python
- Scikit-learn
- XGBoost
- TensorFlow
- Keras
- Matplotlib
- Pandas
- NumPy
