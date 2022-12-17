# Calibration Approach Selection
#### In order to convert classification outcomes to continuous probabilities, Logistic Regression and Isotonic Regression were implemented and compared. <br><br> By randomly allocating different samples into training, test, and hold-out calibration dataset, the result of calibration would thus change and deviate. To achieve a more robust calibration outcome, we chose to run  5 calibrations with different random allocations, and then take the average on them to produce our predicted default rate.

## 1. Calibration for Random Forest Model
### (1) Isotonic Regression

### (2) Logistic Regression


## 2. Calibration for XGBoost Model
### (1) Isotonic Regression

![1](https://user-images.githubusercontent.com/92542287/208211824-a1387ac3-09d1-4dbd-a0c5-ac0a4b27024a.png)


### (2) Logistic Regression

