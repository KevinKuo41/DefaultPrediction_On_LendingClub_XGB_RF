# Rebalancing Data

#### In the dataset, 29.7% of the samples are defaulters, and 70.3% are non-defaulters, so we know this is an imbalanced dataset. To improve the performance of the Machine Learning Technique, we implement a rebalancing approach to adjust the data. Three rebalancing approaches, Oversampling, Undersampling, and SMOTE, are the most often used. <br><br> Since the 42 feature variables include some categorical features, the SMOTE approach is not a suitable rebalancing tool for our dataset. (The main reason is that the implementation of SMOTE is based on the simulation with applying KNN. However, in categorical features, the different figures only mean different classes instead of the actual distance between samples.) <br><br>Thus, we test the implementation of the Oversampling and Undersampling approach on both Random Forest and XGBoost models and choose the one with better Average Precision and F1-Score to conduct further model training. <br><br>(The scores below are the average scores of 5-fold split implementation on the training dataset of 75% samples)

## Random Forest Model
#### Result: 
| Method        | F1-Score | Avg. Precision |
|---------------|----------|----------------|
| Oversampling  | 0.4008   | 0.4786         |
| **Undersampling** | **0.5228**   | **0.4791**         |
#### For Random Forest Model, the Undersampling Approach outperforms.

## XGBoost Model
#### Result: 
| Method        | F1-Score | Avg. Precision |
|---------------|----------|----------------|
| **Oversampling**  |**0.5299**| **0.5014**     |
| Undersampling | 0.5290   | 0.4993         |
#### For XGBoost Model, the Oversampling Approach outperforms.
