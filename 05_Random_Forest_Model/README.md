# Setup of Random Forest Classification Model
#### 1. We apply Undersampling Approach as the rebalancing technique on the dataset for Random Forest Model <br><br><br> 2. For the Random Forest Model, we select 38 out of 42 feature variables in the dataset to train and test the model (The number of 38 is decided based on the Average Precision below)

| #  |  Rebalancing Method | No. of Features |  F1-Score |  Avg. Precision |
|----|---------------------|-----------------|-----------|-----------------|
| 0  | oversample          | 20              | 0.402943  | 0.472199        |
| 1  | oversample          | 22              | 0.401299  | 0.472843        |
| 2  | oversample          | 24              | 0.404656  | 0.476852        |
| 3  | oversample          | 26              | 0.400585  | 0.474349        |
| 4  | oversample          | 28              | 0.401341  | 0.475996        |
| 5  | oversample          | 30              | 0.399925  | 0.475585        |
| 6  | oversample          | 32              | 0.398974  | 0.477381        |
| 7  | oversample          | 34              | 0.400226  | 0.476694        |
| 8  | oversample          | 36              | 0.399093  | 0.477511        |
| 9  | oversample          | 38              | 0.399109  | 0.478158        |
| 10 | oversample          | 40              | 0.400068  | 0.477812        |
| 11 | oversample          | 42              | 0.398203  | 0.476843        |


#### 3. After 5-fold cross-validation for Hyperparameter tuning, the 4 optimal hyperparameters for the Random Forest Model on the dataset: <br> (The details of Hyperparameter Tuning are outlined in 07_Hyperparameter_Tuning)
             n_estimators=1000
             max_depth=100
             min_samples_split=14
             min_samples_leaf=9
            
#### 4. For the performance metrics, we use Confusion Matrix, ROC Curve, and Precision-Recall Curve (Please refer to the 09_Model_Comparison)
