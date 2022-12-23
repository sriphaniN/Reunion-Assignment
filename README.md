
# Data Science Assignment - REUNION


---

### Background

A person’s creditworthiness is often associated (conversely) with the likelihood they may default on loans. 

We’re giving you anonymized data on about 1000 loan applications, along with a certain set of attributes about the applicant itself, and whether they were considered high risk.

0 = Low credit risk i.e high chance of paying back the loan amount

1 = High credit risk i.e low chance of paying back the loan amount

- **Dataset**
    
    [data.zip](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2c3317f5-a58f-4cd0-af29-65e728c3f51e/data.zip)
    
- **Dataset Description**
    
    The dataset has two files:
    
    1. `applicant.csv`: This file contains personal data about the (primary) applicant
    - Unique ID: `applicant_id` (string)
    - Other fields:
        - Primary_applicant_age_in_years (numeric)
        - Gender (string)
        - Marital_status (string)
        - Number_of_dependents (numeric)
        - Housing (string)
        - Years_at_current_residence (numeric)
        - Employment_status (string)
        - Has_been_employed_for_at_least (string)
        - Has_been_employed_for_at_most (string)
        - Telephone (string)
        - Foreign_worker (numeric)
        - Savings_account_balance (string)
        - Balance_in_existing_bank_account_(lower_limit_of_bucket) (string)
        - Balance_in_existing_bank_account_(upper_limit_of_bucket) (string)
    
    1. `loan.csv`: This file contains data more specific to the loan application
    - Target: `high_risk_application` (numeric)
    - Other fields:
        - applicant_id (string)
        - Months_loan_taken_for (numeric)
        - Purpose (string)
        - Principal_loan_amount (numeric)
        - EMI_rate_in_percentage_of_disposable_income (numeric)
        - Property (string)
        - Has_coapplicant (numeric)
        - Has_guarantor (numeric)
        - Other_EMI_plans (string)
        - Number_of_existing_loans_at_this_bank (numeric)
        - Loan_history (string)
        

### **TASK-1**

1. Do the Exploratory Data Analysis & share the insights.
2. How would you segment customers based on their risk (of default).
3. Which of these segments / sub-segments would you propose be approved?
    - For e.g. Would a person with critical credit history be more creditworthy? Are young people more creditworthy? Would a person with more credit accounts be more creditworthy?
4. Tell us what your observations were on the data itself (completeness, skews).

### **TASK-2**

**Develop the ML model(s) to predict the credit risk(low or high) for a given applicant.** 

**Business Constraint:** Note that it is worse to state an applicant as a low credit risk when they are actually a high risk, than it is to state an applicant to be a high credit risk when they aren’t.

**Provide the answers for the below points:**

1. Explain your intuition behind the features used for modeling.
2. Are you creating new derived features? If yes explain the intuition behind them.
3. Are there missing values? If yes how you plan to handle it.
4. How categorical features are handled for modeling.
5. Describe the features correlation using correlation matrix. Tell us about few correlated feature & share your understanding on why they are correlated.
6. Do you plan to drop the correlated feature? If yes then how.
7. Which ML algorithm you plan to use for modeling.
8. **Train two (at least) ML models** to predict the credit risk & provide the confusion matrix for each model.
9. How you will select the hyperparameters for models trained in above step.
10. Which metric(s) you will choose to select between the set of models.
11. Explain how you will export the trained models & deploy it for prediction in production.

