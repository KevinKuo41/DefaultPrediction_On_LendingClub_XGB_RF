# Hyperparameter Tuning
#### We use grid search and apply 5-fold cross validation on the training dataset for hyperparameter tuning. 

## 1. Optimal Hyperparameters for Random Forest Model
#### The leftmost values in column Values are the optimal parameters, and the values within the brackets are the range we grid search through


## 2. Optimal Hyperparameters for XGBoost Model
#### The leftmost values in column Values are the optimal parameters, and the values within the brackets are the range we grid search through
* Since the XGBoost Classifier has some issue when applying with the gridsearch() and RandomUnderSampler() function, we apply our codes to conduct the gridsearch manually rather than using the sklearn gridsearch() function.

| 8 Hyper Parameters  | Values             |
|---------------------|--------------------|
| eta                 | 0.15 (0.05 - 0.50) |
| max_depth           | 6 (3 - 10)         |
| min_child_weight    | 4 (1 - 10)         |
| gamma               | 1.6 (0 - 1.9)      |
| colsample_bytree    | 0.9 (0.1 - 0.9)    |
| subsample           | 0.6 (0.1 - 0.9)    |
| reg_alpha           | 0.2 (0.1 - 1.0)    |
| reg_lambda          | 1 (0.1 - 1.0)      |
