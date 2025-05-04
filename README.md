# LoanTap Logistic Regression

## Project Overview
This project implements a machine learning solution for LoanTap, an online platform that delivers customized loan products to millennials. The data science team at LoanTap needed an underwriting layer to determine the creditworthiness of individuals applying for personal loans. This solution uses logistic regression to predict whether a loan applicant is likely to fully pay back their loan or default (charge off).

## Business Problem
Given a set of attributes for an individual, determine if a credit line should be extended to them and establish appropriate repayment terms.

## Dataset
The dataset contains information about loan applicants including:
- Loan amount, term, and interest rate
- Applicant's financial information (annual income, debt-to-income ratio)
- Credit history (credit line age, public records, etc.)
- Employment information
- Home ownership status
- Verification status
- And many more relevant features

## Methodology
1. **Data Exploration & Visualization**
   - Analyzed distributions and relationships between variables
   - Created visualizations to understand factors affecting loan repayment
   - Identified correlations and patterns in the data

2. **Data Preprocessing**
   - Handled missing values using appropriate imputation techniques
   - Detected and treated outliers
   - Converted categorical variables through encoding methods
   - Applied feature engineering to create more predictive variables

3. **Model Building**
   - Built a logistic regression model to classify loan applications
   - Addressed class imbalance using SMOTE (Synthetic Minority Over-sampling Technique)
   - Applied K-fold cross-validation to ensure model stability

4. **Evaluation**
   - Evaluated model using various metrics: accuracy, precision, recall, F1-score
   - Created ROC curves and precision-recall curves to assess model performance
   - Achieved 89% accuracy on the test dataset

## Key Insights
- 36-month loans are preferred over 60-month loans
- Mortgage holders form the largest borrower segment, followed by renters
- Grade B borrowers show the highest loan repayment rate
- Sub-grade A1 borrowers demonstrate the lowest default rate
- High interest rates correlate with increased default risk (40%)
- Joint applications have higher repayment rates than individual applications

## Business Recommendations
- Implement stricter monitoring for high-interest loans due to increased default risk
- Promote low-interest loans which have >90% repayment probability
- Encourage joint loan applications
- Offer flexible loan terms aligned with customer income levels
- Target high-earning professions for loan distribution
- Maintain rigorous approval processes for essential loans
- Consider alternative credit assessment methods
- Strengthen credit bureau partnerships for better borrower evaluation

## Tools & Technologies
- Python
- Pandas, NumPy for data manipulation
- Matplotlib, Seaborn for data visualization
- Scikit-learn for machine learning implementation
- SMOTE for handling class imbalance

