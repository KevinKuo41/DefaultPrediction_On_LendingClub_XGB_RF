# Calibration Approach Selection
#### In order to convert classification outcomes to continuous probabilities, Logistic Regression and Isotonic Regression are implemented and compared. By randomly allocating different samples into training, test, and hold-out calibration dataset, the result of calibration would thus change and deviate. To achieve a more robust calibration outcome, we choose to run 5 calibrations with different random allocations, and then take the average on them to produce our predicted default rate.

## 1. Calibration for Random Forest Model
### (1) Isotonic Regression

### (2) Logistic Regression

#### For Random Forest Model, Calibration with Isotonic Regression generates a better pattern of calibrated predicted default rates, since it scatters more evenly and especially has a better distribution around the area close to 0 (lower-left area)

## 2. Calibration for XGBoost Model

### (1) Isotonic Regression
![圖片](https://user-images.githubusercontent.com/92542287/208212184-d1c77050-befd-4663-bcde-62b4be65ebea.png)

### (2) Logistic Regression
![圖片](https://user-images.githubusercontent.com/92542287/208212227-2ef52e34-e3b9-498a-843f-668e5e4361c8.png)

#### For XGBoost Model, Calibration with Isotonic Regression generates a better pattern of calibrated predicted default rates, since it scatters more evenly and especially has a better distribution around the area close to 0 (lower-left area)

#### On the other hand, although all the patterns of calibrated predicted default rates are in the shape of a backward curve instead of a perfect 45-degree line, in this project, we aim to avoid defaulters and make profits. Hence, a backward curve means we have a relatively conservative default prediction. This fact is not a bad thing thing from the aspect of risk management.
