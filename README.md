# House-price-prediction-model
A machine learning project for predicting California housing prices using regression models. The pipeline includes data preprocessing, stratified train-test splitting, model comparison, and final prediction using a trained Random Forest Regressor saved with joblib.

## Project Overview

The model is trained on the housing.csv dataset and uses a custom preprocessing pipeline to handle:

- Missing values
- Feature scaling
- Encoding of categorical data

To ensure balanced data distribution, the dataset is split using stratified sampling based on income categories.

## Models Used

The following regression models were trained and evaluated:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

After cross-validation, *Random Forest Regressor* performed the best, with the lowest RMSE and the most stable results.

## Features

- Complete machine learning workflow
- Custom preprocessing pipeline
- Stratified train-test split
- Cross-validation for model evaluation
- Model saving with joblib
- Prediction on new input data
- Output saved to .output.csv

## Workflow

1. Load the dataset.
2. Preprocess the data carefully.
3. Split the data using stratified sampling.
4. Train and evaluate multiple regression models.
5. Select the best-performing model.
6. Save the trained model using joblib.
7. Use the saved model to predict house prices for new data in input.csv.
8. Store predictions in .output.csv.

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- joblib

Install dependencies with:

```bash
pip install pandas numpy scikit-learn joblib
