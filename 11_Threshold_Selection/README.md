# Loan Selection Strategy (Threshold Selection)
#### Based on the ROC Curve and the Recall-Precision Curve, we know that the XGBoost model outperforms Random Forest Model, so here we use the XGBoost model to conduct further research on the Loan Selection Strategy and find the optimal predicted default rate threshold to achieve the highest loan return when lending money on LendingClub platform.

#### After the calibration process, our XGBoost can be used only to predict the probability of loan defaults. However, it doesn’t offer us a granular view with respect to how much return loans can generate, which is especially vital for investors to make profit on the LendingClub platform. <br><br> As a result, in order to help investors avoid unnecessary losses and make reasonable profit, we run our XGBoost model on test samples to get each borrower's predicted default probability, and then calculate the average loan returns for borrowers accepted under different default rate. <br><br> Our predicted default probabilities can serve as a threshold for investors to decide which loans to accept. When applying 12% as the threshold in selecting borrowers, investors will have a lower default rate, a steady payoff, and the highest loan return, 1.55%. The optimal threshold and its brought return is shown as the golden star in the below graph. <br><br>

![圖片](https://user-images.githubusercontent.com/92542287/208196847-e471f232-ead1-43e7-8c15-efaf066dd231.png)



