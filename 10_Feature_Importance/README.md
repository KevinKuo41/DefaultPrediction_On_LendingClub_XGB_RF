# Feature Importance
## 1. Random Forest Model

## 2. XGBoost Model
| Rank | Feature                          | Importance |
|------|----------------------------------|------------|
| 1    | Grade                            | 45.40%     |
| 2    | Sub-Grade                        | 18.50%     |
| 3    | Interest Rate                    | 6.40%      |
| 4    | Term                             | 4.20%      |
| 5    | Credit Inquiry in Last 6 Months  | 2.00%      |
| 6    | Home Ownership                   | 1.80%      |
| 7    | Employment Length                | 1.60%      |
| 8    | Loan Amount                      | 1.30%      |
| 9    | No. of Currently Active Bankcard | 1.20%      |
| 10   | Verification Status              | 1.00%      |

## 3. Underlying Mechanisms Between Features and Default
### (1) Grades
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







