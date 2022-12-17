# Feature Importance
## 1. Random Forest Model
| Rank | Feature                            | Importance |
|------|------------------------------------|------------|
| 1    | Interest Rate                      | 12.90%     |
| 2    | Sub-Grade                          | 11.43%     |
| 3    | Installment                        | 4.60%      |
| 4    | Total Credit Limit                 | 3.89%      |
| 5    | Average Current Balance            | 3.79%      |
| 6    | Loan Amount                        | 3.69%      |
| 7    | Repayment Term                     | 3.64%      |
| 8    | Monthly Debt Payments / Total Debt | 3.63%      |
| 9    | Total Current Balance              | 3.57%      |
| 10   | Total Credit Revolving Balance     | 3.49%      |

## 2. XGBoost Model
| Rank | Feature                          | Importance |
|------|----------------------------------|------------|
| 1    | Grade                            | 45.40%     |
| 2    | Sub-Grade                        | 18.50%     |
| 3    | Interest Rate                    | 6.40%      |
| 4    | Repayment Term                   | 4.20%      |
| 5    | Credit Inquiry in Last 6 Months  | 2.00%      |
| 6    | Home Ownership                   | 1.80%      |
| 7    | Employment Length                | 1.60%      |
| 8    | Loan Amount                      | 1.30%      |
| 9    | No. of Currently Active Bankcard | 1.20%      |
| 10   | Verification Status              | 1.00%      |

## 3. Comparison
#### As we can find, the Random Forest model relies on each feature variable much more evenly than the XGBoost model does. Instead, the XGBoost model puts more than 60% of its reliance on only two feature variables Grade & Sub-Grade.

## 4. Underlying Mechanisms Between Features and Default
### (1) Grade & Sub-Grade
#### Grade is set based on the individual’s credit score, which takes account of the individual’s payment history and recent credit behaviour.
### (2) Interest Rate
#### Interest Rate on loans is decided based on the individual’s grade, so Grades and Interest Rate are highly related.
### (3) Repayment Term
#### Borrowers choosing 60 months as their repayment term have a bit higher probability of default, which may be related to the liquidity the borrower possesses.
### (4) Credit Inquiry in Last 6 Months
#### If a borrower has credit inquiry records in the last 6 months, it means that he/she had tried to borrow from other financial institutions and thus may have heavier financial burdens.
### (5) Home Ownership & Employment Length
#### Both are associated of borrower's financial stability
### (6) Verification Status
#### Document Verifications includes 1. Business Tax returns. 2. Proof of personal income. 3. Proof of identity and address for you or your business, so the candidate may have higher financial stability if candidate can provide these evidences
### (7) Installment & Monthly Debt Payments / Total Debt
#### Installment is the monthly payment owed by the borrower if the loan originates. Both Installment & Monthly Debt Payments / Total Debt would impact the liquidity and saving ability of the borrower.
### (8) Average Current Balance & Total Current Balance
#### Both are associated of borrower's liquidity and disposable fund
### (9) Loan Amount
#### The higher the Loan Amount, the higher the interest and installment the borrower need to repay
### (10) Total Credit Revolving Balance
#### Total Credit Revolving Balance is related to the borrower's unpaid repayment amount
