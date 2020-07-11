# AnalyticsVidhya_LoanPrediction
## Problem Statement
Dream Housing Finance company deals in all kinds of home loans. They have presence across all urban, semi urban and rural areas. Customer first applies for home loan and after that company validates the customer eligibility for loan.

Company wants to automate the loan eligibility process (real time) based on customer detail provided while filling online application form. These details are Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History and others. To automate this process, they have provided a dataset to identify the customers segments that are eligible for loan amount so that they can specifically target these customers. 

Following are the features in tha dataset:
- Loan_ID
- Gender
- Married
- Dependents: 1, 2, 2+
- Education: Graduate, non Graduate
- Self_Employed
- ApplicantIncome
- CoapplicantIncome
- LoanAmount
- Loan_Amount_Term
- Credit_History: 0, 1
- Property_Area: Urban, Suburban, Rural

Target Variable
- Loan_Status

The very first step before building a Machine Learning model is to understand the data. Deriving insights and understnading the data is called **Exploratory Data Analysis (EDA)**. The initial segments of the code help you to do this. Following are the insights I got after performing an EDA.
1. On looking at the box plots we understand that less than half of our loans are classified as not accepted.
2. All applicants with an income greater than 20,000 have higher level of education and most of the dataset is comprised of applicants with higher education.
## Handling missing values
I have imputed categorical features with the mode, and numerical features with the median of the data. An alternative would be to try to use other features to predict the missing feature values. 
## Feature Engineering
After doing feature engineering and looking at the heatmap we understand that - ApplicantIncome and LoanAmount have high colinearity. Also credit history seems to be highly correlated with loan status, this points to it being the most important feature for our model. 
## Final steps
The final steps is to perform Mdoel parameter Tuning and Selection. I have used the following classificatin techniques to which performs the best. Random Forest Classfier , Gradient Boosting Classification and Logistic Regression.

[Link to the problem statement.](https://datahack.analyticsvidhya.com/contest/practice-problem-loan-prediction-iii/)

