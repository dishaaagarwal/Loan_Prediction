## Loan-Prediction-Dataset

From the challange hosted at: https://datahack.analyticsvidhya.com/contest/practice-problem-loan-prediction-iii/


## Problem Statement:

Dream Housing Finance company deals in all home loans. They have presence across all urban, semi urban and rural areas. Customer first apply for home loan after that company validates the customer eligibility for loan.

The company wants to automate the loan eligibility process (real time) based on customer detail provided while filling online application form. These details are Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History and others. To automate this process, they have given a problem to identify the customers segments, those are eligible for loan amount so that they can specifically target these customers. Here they have provided a partial data set.


## The Data

Variable | Description
----------|--------------
Loan_ID | Unique Loan ID
Gender | Male/ Female
Married | Applicant married (Y/N)
Dependents | Number of dependents
Education | Applicant Education (Graduate/ Under Graduate)
Self_Employed | Self employed (Y/N)
ApplicantIncome | Applicant income
CoapplicantIncome | Coapplicant income
LoanAmount | Loan amount in thousands
Loan_Amount_Term | Term of loan in months
Credit_History | credit history meets guidelines
Property_Area | Urban/ Semi Urban/ Rural
Loan_Status | Loan approved (Y/N)




## Loan_Prediction Notebook Description

In this Notebook I have Implemented Full Stack Data Science Project on the Loan_Prediction dataset using Logistic Regression. My main aim in this Notebook is to try discover more in the dataset while keeping model building simple so that it becomes easy to understand the concepts.



### Table of Content


1. **Hypothesis Generation**
   
   i. Salary : Applicants with high Salary have higher chance of paying the loan.

   ii. LoanAmount: If it is less then chances of Loan approval is more.

   iii. Loan_Amount_term: Less is the period or amount the more is the chances of Loan approval

   iv. EMI: Less is the EMI to be paid/ month the more is the chances of Loan approval. 


2. **EDA (Univariate and Bi-variate Analysis)**

![](/images/numerical_features.png)

Numerical Features

![](/images/categorical_features.png)

Categorical Features

![](/images/numerical_bivariate_analysis.png)

Bivariate Analysis on numerical features

![](/images/categorical_bivariate_analysis.png)

Bivariate Analysis on categorical features


3. **Missing Value Imputation and Outlier Detection.**

![](/images/Outlier_analysis_.png)

Outlier Analysis

4. **Feature Engineering.**

![](/images/Total_Income_Feature_Engineering.png)

Created new Feature -> Total_Income

5. **Preparing data for Model Building.**

![](/images/test_data_histogram.png)

Final Test data to be used

![](/images/train_data_histogram.png)

Final Train data to be used

6. **Model-Building-1 using CV**

For this I have compared across 3 models -> KNN, Logistic Regression, Decision Tree.
Logistic Regression gave the highest accuracy and precision > LR: 0.807797 (0.027162)


7. **Evaluation metrics using Accuracy_score,ROC_curve**

My accuracy score on test data was 80%

![](/images/ROC_AUC.png)

ROC-AUC curve for test data


8. **Model-Building-1 using Feature Selection,Feature Scaling and Hyper-Parameter Tuning.**

For this I had used SelectKBest as well as ExtraTree classifier to select the best features.Later I had used GridSearchCV for HyperParameter Tuning.


9. **Re-Training the Model with the selected Parameters.**

My accuracy has improved to *83%.*


10. **Making Predictions and the Test Data.**


11. **Making the Sample_Submissing with the Predictions.**

I was able to achieve an accuracy of *77%* on the leaderboard. 
