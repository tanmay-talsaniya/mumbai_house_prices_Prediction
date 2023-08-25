# House Price Prediction Project

## Introduction

This project focuses on predicting house prices using machine learning techniques. The goal is to develop a model that accurately estimates house prices based on various features such as location, property type, age, and more. The project involves data preprocessing, exploratory data analysis (EDA), model selection, hyperparameter tuning, and evaluation.

## Data

The dataset used for this project contains information about different properties, including features like property type (Apartment, Independent House, etc.), locality, region, status (Ready to Move or Under Construction), age of the property, number of bedrooms (BHK), area, and house price.

## Methodology

### Data Preprocessing

Data preprocessing is a critical step to ensure that the data is suitable for modeling. Categorical features are encoded using LeaveOneOut Encoder, while numerical features are scaled using Standard Scaler. This normalization process helps improve model performance by standardizing feature scales.

### Exploratory Data Analysis (EDA)

EDA involves analyzing and visualizing the data to gain insights and identify patterns. Visualizations such as scatter plots, histograms, and correlation matrices help us understand the relationships between variables and uncover key features influencing house prices.

### Model Selection

Multiple regression models are evaluated, including Linear Regression, Decision Tree Regressor, Random Forest Regressor, AdaBoost Regressor, Gradient Boosting Regressor, KNeighbors Regressor, XGB Regressor, and XGBRF Regressor. Among these, the RandomForestRegressor demonstrates promising potential due to its ability to capture complex relationships in the data.

### Hyperparameter Tuning

Hyperparameter tuning is conducted using techniques like RandomizedSearchCV to find the best combination of hyperparameters for the RandomForestRegressor. This process optimizes the model's performance and generalization ability.

### Feature Selection

Feature selection is guided by the correlation matrix. Features with weak correlations to the target variable are dropped, improving model efficiency and interpretability. In this case, the "type" feature is removed.

### Model Training and Evaluation

The selected RandomForestRegressor is trained on the preprocessed data. The model's performance is evaluated using metrics such as the Train Score, Test Score, Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R2) Score. These metrics provide insight into the model's accuracy and its ability to predict house prices effectively.

## Results

The final RandomForestRegressor model achieves impressive results:

- Train Score: 98.97%
- Test Score: 92.42%
- MAE: 1,737,664.62
- MSE: 35,487,875,200,333.21
- R2 Score: 91.37%

## Conclusion

This project demonstrates the power of data preprocessing, exploratory data analysis, and thoughtful model selection in achieving accurate house price predictions. The RandomForestRegressor, after hyperparameter tuning and feature analysis, emerges as the top performer, offering a robust solution for real-world house price estimation tasks.

Feel free to contribute and explore the code in this repository to understand and replicate the process of house price prediction using machine learning.
