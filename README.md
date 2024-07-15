# House-price-prediction

I have implemented a comprehensive solution to predict house prices using a variety of models, including Linear Regression, Decision Tree, Random Forest, XGBoost, Support Vector Machine, k-Nearest Neighbors, and Neural Networks.

#Project Highlights:

#1.Data Loading and Preprocessing:
We start by loading the dataset and converting the date column to a datetime object for easier manipulation.
We extract the year and month from the date and drop unnecessary columns (id and date).
Missing values are handled by dropping any rows with NaNs.

#2.Feature and Target Separation:
The dataset is split into features (X) and the target variable (y), where the target variable is the house price.

#3.Train-Test Split:
We split the data into training and testing sets to evaluate our models' performance on unseen data.

#4.Model Training and Evaluation:
We define a helper function evaluate_model() to train each model and calculate the RMSE and R² scores for performance evaluation.
Models included in this project are:
Linear Regression
Decision Tree
Random Forest
XGBoost
Support Vector Machine (SVR)
k-Nearest Neighbors
Neural Networks (using Keras and TensorFlow)

#5.Model Performance:
Linear Regression: RMSE = 212036.1654, R² = 0.7026
Decision Tree: RMSE = 211372.5139, R² = 0.7045
Random Forest: RMSE = 150257.8166, R² = 0.8507
XGBoost: RMSE = 142414.6545, R² = 0.8658
Support Vector Machine: RMSE = 400942.5278, R² = -0.0634
k-Nearest Neighbors: RMSE = 186712.8618, R² = 0.7694
Neural Network: RMSE = 191165.3486, R² = 0.7583

#6.Model Selection:
After training and evaluating each model, we select the best-performing model based on RMSE. The best model for this project is XGBoost.

#7.Visualization:
We plot actual vs. predicted prices for each model to visually inspect their performance.
Feature importance is plotted for models that provide this information, helping us understand which features are most influential in predicting house prices.

#8.Feature Relationships:
We visualize the relationships between all independent features and the target variable (house prices) using scatter plots. This helps us understand the correlation between each feature and house prices.

#9.User Interaction:
Now, users can predict the house price by providing input for various features such as the number of bedrooms, bathrooms, square footage, and more.

