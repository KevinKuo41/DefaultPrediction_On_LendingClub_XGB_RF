# Calibration Approach Selection
#### In order to convert classification outcomes to continuous probabilities, Logistic Regression and Isotonic Regression are implemented and compared. By randomly allocating different samples into training, test, and hold-out calibration dataset, the result of calibration would thus change and deviate. To achieve a more robust calibration outcome, we choose to run 5 calibrations with different random allocations, and then take the average on them to produce our predicted default rate.

## 1. Calibration for Random Forest Model
### (1) Isotonic Regression
![圖片](https://user-images.githubusercontent.com/92542287/208262780-cd27d815-c6dd-4a02-b3c8-5962c78aa2e7.png)

### (2) Logistic Regression
![圖片](https://user-images.githubusercontent.com/92542287/208262857-bba655e4-6b19-4fe7-8f66-bc0ee7864f36.png)

#### For Random Forest Model, calibration with Logistic Regression leads to a relatively optimistic view for clients with lower default probabilities and a rather conservative view for clients with higher default probabilities, which is a good thing from the view of Risk Management. Thus, we applied the calibration with Logistic Regression for RF Model.

## 2. Calibration for XGBoost Model

### (1) Isotonic Regression
![圖片](https://user-images.githubusercontent.com/92542287/208212184-d1c77050-befd-4663-bcde-62b4be65ebea.png)

### (2) Logistic Regression
![圖片](https://user-images.githubusercontent.com/92542287/208212227-2ef52e34-e3b9-498a-843f-668e5e4361c8.png)

#### For XGBoost Model, calibration with Isotonic Regression generates a better pattern of calibrated predicted default rates since it scatters more evenly and has a better distribution around the area close to 0 (lower-left area)


#### On the other hand, although all the patterns of calibrated predicted default rates are in the shape of a backward curve instead of a perfect 45-degree line, in this project, we aim to avoid defaulters and make profits. Hence, a backward curve means we have a relatively conservative default prediction. This fact is not bad from the aspect of risk management. Thus, we applied the calibration with Isotonic Regression for XGBoost Model.
