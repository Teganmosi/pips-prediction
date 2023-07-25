# pips-prediction

This GitHub repository contains code for a machine learning regression task involving time series data.
The code focuses on predicting 'pips', a financial metric, using various models.

Here's an overview of what the repository offers:

1. Data Preprocessing: The code begins by loading the data from an Excel file and extracting features from lists in specific columns using a custom function 'extract_numbers'.

2. LSTM Model Training: An LSTM neural network model is built with 64 units and a dense layer with 1 unit for regression. The data is normalized using Min-Max scaling, reshaped to fit the LSTM input shape, and then trained on the training dataset using the mean squared error loss and the Adam optimizer.

3. Model Evaluation: The performance of the LSTM model is evaluated on both the training and testing datasets using the mean squared error loss. The model's predictions are also demonstrated using a new input sequence.

4. Hyperparameter Tuning: Hyperparameter tuning is performed for the LSTM model using GridSearchCV for different units, dropout rates, and L2 regularization values. This helps to identify the best combination of hyperparameters, leading to improved performance.

5. Evaluation of Other Models: The code implements Linear Regression, Gradient Boosting Regressor, Support Vector Machine (SVR), XGBoost, Random Forest Regressor, K-Nearest Neighbors (KNN), and Multi-Layer Perceptron (MLP) models for comparison with the LSTM model. The performance metrics (MAE and RMSE) for each model are calculated and plotted.

The repository provides valuable insights into the effectiveness of different regression models for the given time series prediction task. Users interested in financial time series prediction or machine learning enthusiasts looking to explore various regression algorithms would find this repository informative and useful.
