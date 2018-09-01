# Home-Credit-Default-Risk
Kaggle problem to predict whether an applicant is likely to repay or default the loan based on applicant's data, previous loan history within and outside the company. Achieved a ROC-AUC score of 0.788 with the final_submission_script notebook in the competition. 

Description of the datasets: 
1. application_{train|test}.csv: Static data for all applications. One row represents one loan in our data sample.

2. bureau.csv: All client's previous credits provided by other financial institutions that were reported to Credit Bureau (for clients who have a loan in our sample).
For every loan in our sample, there are as many rows as number of credits the client had in Credit Bureau before the application date.

3. bureau_balance.csv: Monthly balances of previous credits in Credit Bureau.

4. POS_CASH_balance.csv: Monthly balance snapshots of previous POS (point of sales) and cash loans that the applicant had with Home Credit.

5. credit_card_balance.csv: Monthly balance snapshots of previous credit cards that the applicant has with Home Credit.

6. previous_application.csv: All previous applications for Home Credit loans of clients who have loans in our sample.
There is one row for each previous application related to loans in our data sample.

7. installments_payments.csv: Repayment history for the previously disbursed credits in Home Credit related to the loans in our sample.
There is a) one row for every payment that was made plus b) one row each for missed payment


Description of the uploaded scripts: 

1. Data_exploration: EDA of the application dataset. It can also be found as a Kaggle Kernel here: https://www.kaggle.com/tejase13/data-exploration

2. Application_dataset: Feature engineering application dataset and experimenting with different modeling techniques such as Logistic regression, Random forest and Gradient boosting

3. Final_submission_script: Modelled by Gradient boosting on the master dataset created by merging all the datasets at application level
