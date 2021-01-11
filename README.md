# Sales forecast
It is necessary to build a sales forecast model for each store 31 days in advance. There are 20 stores (id). Evaluation Metric - Scaled Mean Absolute Error (sMAE), sMAE < 0.12 is desirable.

## Files
Training sample file: train.csv
File with test sample (without target variables): test.csv
Example file format with the result of the prediction: predict_example.csv

## Results
received on the 1-last-month holdout from train.csv
|   model  | RMSE |  sMAE  |
|----------|------|--------|
| XGBoost  | 85.5 | 0.0916 |
| Linear   | 98.1 | 0.1092 |

## Pipelines / Models
* Time Series Feature Generation
* Time Series Cross Validation
* Hyperparameters Search
* LinearRegression
* XGBoost

## Dependencies
* xgboost
* Optuna

