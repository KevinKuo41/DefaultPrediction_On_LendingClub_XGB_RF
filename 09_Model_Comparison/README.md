# Model Comparison
## 1. Confusion Matrix
### Random Forest Model

| Class          | Precision | Recall | F1-Score | Support |
|----------------|-----------|--------|----------|---------|
| Fully Paid (0) | 0.82      | 0.63   | 0.72     | 104,291 |
| Default (1)    | 0.44      | 0.68   | 0.53     | 43,705  |
| Weighted Avg.  | 0.71      | 0.65   | 0.66     | 147,996 |

![圖片](https://user-images.githubusercontent.com/92542287/208227479-26886907-da0a-4bc8-9735-d0ba640086bc.png)

### XGBoost Model

| Class          | Precision | Recall | F1-Score | Support |
|----------------|-----------|--------|----------|---------|
| Fully Paid (0) | 0.83      | 0.65   | 0.72     | 104,291 |
| Default (1)    | 0.44      | 0.67   | 0.54     | 43,705  |
| Weighted Avg.  | 0.71      | 0.65   | 0.67     | 147,996 |

![圖片](https://user-images.githubusercontent.com/92542287/208213877-37e39f16-e9a1-498f-b542-7a6a1f6cde30.png)



### (3) Precision-Recall Curve
![圖片](https://user-images.githubusercontent.com/92542287/208227519-aa76a51e-b11c-49a1-8e18-371b2c140912.png)


## 2. ROC Curve
### Random Forest Model
![圖片](https://user-images.githubusercontent.com/92542287/208227496-1b152c08-e34c-4111-bf25-48cbab26ff81.png)

### XGBoost Model
![圖片](https://user-images.githubusercontent.com/92542287/208213912-3f0589b6-42a9-4114-927d-aa7a3f59a209.png)

### (3) Precision-Recall Curve
![圖片](https://user-images.githubusercontent.com/92542287/208213935-1e5deffb-c1f3-441b-811c-7ccce832a073.png)

## 3. Precision-Recall Curve
### Random Forest Model
![圖片](https://user-images.githubusercontent.com/92542287/208227519-aa76a51e-b11c-49a1-8e18-371b2c140912.png)

### XGBoost Model
![圖片](https://user-images.githubusercontent.com/92542287/208213935-1e5deffb-c1f3-441b-811c-7ccce832a073.png)
