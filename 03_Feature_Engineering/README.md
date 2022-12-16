# Feature Engineering
## (1) Handling Outliers: 
### Since we aim to find a general pattern for default prediction, we got rid of the samples with values located outside the Mean ± 3 times Standard Deviation.

## (2) Deletion:
### - For features updated after borrowers being default (“total_pymnt”, “total_rec_int”, “total_rec_late_fee”, “total_rec_prncp”), we exclude them from models, since they were unknown at the time when issuing the loan. (They are highly correlated to Default.) <br><br> - For features unrelated to the analysis (“zip_code” and “loan_id”), we deleted them all. <br><br> - For feature “emp_title”, there are 20,000+ kinds of job titles in it. Regardless of what kinds of adjustment we applied to it, we still cannot decrease its number of categories into a relatively reasonable range, so we exclude it from the models.



