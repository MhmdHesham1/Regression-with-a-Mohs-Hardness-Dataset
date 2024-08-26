# Mohs Hardness Prediction

This project aims to predict the Mohs hardness of materials using various regression models. It's part of a Kaggle competition (Playground Series S3E25).

## Overview

The code performs the following main tasks:
1. Data loading and preprocessing
2. Model training and evaluation
3. Prediction on test data and submission file creation

## Dependencies

- numpy
- pandas
- scikit-learn
- xgboost
- catboost

## Data

The project uses two datasets:
- `train.csv`: Contains features and Mohs hardness values for training
- `test.csv`: Contains features for prediction

## Models

The following regression models are implemented and compared:
1. Random Forest
2. Gradient Boosting
3. Decision Tree
4. K-Nearest Neighbors
5. XGBoost
6. CatBoost
7. Voting Regressor (ensemble of the above models)

## Evaluation Metrics

Models are evaluated using:
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R2 Score

## Usage

1. Ensure all dependencies are installed
2. Place the dataset files in the appropriate directory
3. Run the Jupyter notebook or Python script
4. The best performing model (CatBoost in this case) is used to generate predictions on the test set
5. A submission file 'submission.csv' is created with the predictions

## Results

The CatBoost model performed best with the following metrics:
- Mean Squared Error: 1.4876
- Mean Absolute Error: 0.9097
- R2 Score: 0.4527

## Future Improvements

- Feature engineering
- Hyperparameter tuning
- Trying other advanced models or ensembles


