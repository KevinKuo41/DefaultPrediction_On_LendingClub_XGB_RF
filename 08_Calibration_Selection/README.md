# Calibration Approach Selection
#### In order to convert classification outcomes to continuous probabilities, Logistic Regression and Isotonic Regression were implemented and compared. <br><br> By randomly allocating different samples into training, test, and hold-out calibration dataset, the result of calibration would thus change and deviate. To achieve a more robust calibration outcome, we chose to run  5 calibrations with different random allocations, and then take the average on them to produce our predicted default rate.

## 1. Calibration for Random Forest Model
### (1) Isotonic Regression

### (2) Logistic Regression


## 2. Calibration for XGBoost Model
### (1) Isotonic Regression

![圖片](https://user-images.githubusercontent.com/92542287/208212184-d1c77050-befd-4663-bcde-62b4be65ebea.png)



### (2) Logistic Regression

