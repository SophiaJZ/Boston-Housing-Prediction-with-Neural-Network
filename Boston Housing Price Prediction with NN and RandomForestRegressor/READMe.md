# Boston-Housing-Prediction-with-Neural-Network and RandomForestRegressor

Here’s an improved and polished explanation suitable for a GitHub post:

Boston Housing Price Prediction Using Machine Learning Regression
This project focuses on predicting Boston housing prices using Machine Learning regression analysis. The primary goal is to evaluate and compare the performance of two Machine Learning models: Neural Network and RandomForestRegressor, based on their predictive accuracy using evaluation metrics such as Mean Absolute Error (MAE) and Mean Squared Error (MSE).

Models and Results:
- Neural Network:
-- MAE: 2.77
-- MSE: 15.17
- RandomForestRegressor:
-- MAE: 2.07
-- MSE: 8.11
  
From the results, the RandomForestRegressor outperformed the Neural Network, achieving lower error values for both MAE and MSE. This indicates that the RandomForestRegressor is better suited for this particular dataset and problem.

## Python Libraries used

- NumPy
- Panda
- Scikit-Learn
- KERAS
- Matplotlib

## Data Description:

### Features

- CRIM: Per capita crime rate by town
- ZN: Proportion of residential land zoned for lots over 25,000 sq. ft
- INDUS: Proportion of non-retail business acres per town
- CHAS : Charles River dummy variable (1 if tract bounds river; 0 otherwise)
- NOX: Nitric oxide concentration (parts per 10 million)
- RM: Average number of rooms per dwelling
- AGE: Proportion of owner-occupied units built prior to 1940
- DIS: Weighted distances to five Boston employment centers
- RAD: Index of accessibility to radial highways
- PTRATIO: Pupil-teacher ratio by town
- B: 1000(Bk — 0.63)², where Bk is the proportion of [people of African American descent] by town
- LSTAT: Percentage of lower status of the population
  
### Target (The Price)
- MEDV: Median value of owner-occupied homes in $1000s

## Acknowledgment
- Python for Microscopists by : Sreenivas Bhattiprolu
- https://www.kaggle.com/datasets/schirmerchad/bostonhoustingmlnd

