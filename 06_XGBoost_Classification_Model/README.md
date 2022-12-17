# Setup of XGBoost Classification Model
#### 1. We apply Oversampling Approach as the rebalancing technique on the dataset for XGBoost Model <br><br><br> 2. After 5-fold cross-validation for Hyperparameter tuning, the 8 optimal hyperparameters for XGBoost Model: <br> (The details of Hyperparameter Tuning are outlined in 07_Hyperparameter_Tuning)
             eta=0.15
             max_depth=6
             min_child_weight=4
             gamma=1.6
             colsample_bytree=0.9
             subsample=0.6
             reg_alpha=0.2
             reg_lambda=1             
#### 3. For the performance metrics, we use Confusion Matrix, ROC Curve, and Precision-Recall Curve <br> (Please refer to the 09_Model_Comparison)
