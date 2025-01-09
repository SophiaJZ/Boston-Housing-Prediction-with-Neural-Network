# Boston-Housing-Prediction-with-Neural-Network

This project predicts Boston housing prices using Machine Learning Regression analysis. Preprocessing was implemented before all other processes. A neural network model with two hidden layers was used, where ReLU was applied as the activation function for the hidden layers, and a linear function was used for the output layer. The model was trained multiple times with different parameter to achieve the best performance and results.

For evaluation, Mean Squared Error (MSE), Mean Absolute Error (MAE), and loss were chosen to assess the quality of the results. The prediction results were found to be quite close to the actual values.

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
