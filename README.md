# Hyper-Parameter-Tuning-and-cross-validation
# Problem Statement: 
In this project, we will predict whether an applicant should be approved a Credit Loan or not. To predict the model,we are going to use K Nearest Neighbor algorithm. We are going to perform Hyper Parameter tuning by plotting Accuracy vs # of k (nearest neighbors) and preferring stability over accuracy. Also, we will perform 10 fold cross validation. 

#- Credit loan approval prediction: We have a dataset of credit loan approval. We have 11 dependent features in this dataset, such as:
'Gender' : Male or Female (Categorical data type)
'Married' : Yes or No (Categorical data type)
'Dependents': Number of dependent persons on the applicant (Integer data type)
'Education': Education of the applicant. "Graduate" or "not Graduate"
'Self_Employed': Yes or No(Categorical data type)
'ApplicantIncome': Income of the applicant(Float Type)
'CoapplicantIncome': Income of co-applicant(Float type)
'LoanAmount': Required Loan Amount (Float data type)
'Loan_Amount_Term': Tenure of the loan (Float data type)
'Credit_History': 1 or 0 ( Good or Bad,Categorical data type)
'Property_Area': Urban ir Rural (Categorical data type)
'Loan_Status': Yes or No, loan approved por not (Categorical data type)

#- Technical Features of the project:
From a technical point of view, the main aspects of python covered throughout the notebook are:

Libraries: Pandas, Numpy, Sklearn,
data manipulation: pandas, numpy, 
modeling: K Nearest neighbor. 
Visualization : matplotlib
Evaluation: Cross Validation score. 

#-Exploratory Data Analysis 
We have performed EDA by dropping the rows which have missing values. Then we have converted the categorical data into numeric form.  After that we have done random sampling on the model. 
#-Hyper Parameter Tuning:
By using Matplotlib library, we have plotted a graph of number of K neighbors VS accuracy. We have preferred stability over accuracy. By observing the graph, awe can see that after number of neighbors 30, the accuracy becomes constant. Hence, we choose the value of K to be 30.

#- Model building and cross validation.
After hyper paramater tuning, we apply KNN algorithm on train data set with number of K equals to 30. By using cross validation, we apply 10 fold cross validation. The mean accuracy we got is 71%.
