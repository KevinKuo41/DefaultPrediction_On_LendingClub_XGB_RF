# Setup of Random Forest Classification Model
#### 1. We apply Undersampling Approach as the rebalancing technique for Random Forest Model <br><br><br> 2. For the Random Forest Model, we select the most important 38 out of 42 feature variables in the dataset to train and test the model <br><br><br> 3. After 5-fold cross-validation for Hyperparameter tuning, the 4 optimal hyperparameters for XGBoost Model on the dataset: <br> (The details of Hyperparameter Tuning are outlined in 07_Hyperparameter_Tuning)
             n_estimators=1000
             max_depth=100
             min_samples_split=
             min_samples_leaf=
            
#### 4. For the performance metrics, we use Confusion Matrix, ROC Curve, and Precision-Recall Curve (Please refer to the 09_Model_Comparison)
