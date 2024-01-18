# Car Price Prediction

## Overview
This project aims to predict the prices of cars based on various features. The dataset used for this analysis contains information about car specifications, such as engine size, horsepower, fuel type, and more.

## Dataset
The dataset used in this project is named "CarPrice_Assignment.csv" and consists of 205 entries with 26 columns. The columns include features such as car ID, symboling, car name, fuel type, aspiration, door number, car body, drivewheel, enginelocation, and more.

## Data Preprocessing
- Columns 'car_ID' and 'CarName' were dropped as they were not relevant for the predictive model.
- Categorical variables were one-hot encoded using dummy variables.
- The dataset was split into numerical and categorical features.
- Standard scaling was applied to numerical features to ensure uniformity.

## Models Used
1. **Linear Regression**
   - Achieved R-Squared: 0.8374
   - Root Mean Squared Error (RMSE): 2715.20

2. **Random Forest Regressor**
   - Hyperparameter tuning using RandomizedSearchCV.
   - Best parameters: {'n_estimators': 7, 'max_depth': 7}
   - Achieved R-Squared: 0.8873
   - RMSE: 2260.59

3. **Gradient Boosting Regressor**
   - Hyperparameter tuning using RandomizedSearchCV.
   - Best parameters: {'n_estimators': 116, 'max_depth': 5}
   - Achieved R-Squared: 0.8511
   - RMSE: 2598.33

4. **AdaBoost Regressor**
   - Number of estimators was optimized.
   - Achieved R-Squared: 0.8652
   - RMSE: 2472.39

## Feature Importance
- Feature importance was visualized for the Random Forest Regressor.

## Conclusion
The Random Forest Regressor performed the best among the models, achieving the highest R-squared value and the lowest RMSE. The feature importance analysis indicated that certain features play a more significant role in predicting car prices.

## Dependencies
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## How to Run
1. Ensure you have the required dependencies installed.
2. Clone the repository.
3. Run the Jupyter notebook.

Feel free to explore and modify the code to enhance the model or try different algorithms.
