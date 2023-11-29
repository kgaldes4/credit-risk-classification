# credit-risk-classification

sources cited in notebook

Project Instructions:

The instructions for this Challenge are divided into the following subsections:

Split the Data into Training and Testing Sets

Create a Logistic Regression Model with the Original Data

Write a Credit Risk Analysis Report

Split the Data into Training and Testing Sets
Open the starter code notebook and use it to complete the following steps:

Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

NOTE
A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

Split the data into training and testing datasets by using train_test_split.

Create a Logistic Regression Model with the Original Data
Use your knowledge of logistic regression to complete the following steps:

Fit a logistic regression model by using the training data (X_train and y_train).

Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

Evaluate the model’s performance by doing the following:

Generate a confusion matrix.

Print the classification report.

Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

Write a Credit Risk Analysis Report
Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the README.md file included in your GitHub repository.

Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:

An overview of the analysis: Explain the purpose of this analysis.

The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

Analysis:

Overview of the Analysis
The purpose of this analysis is to create a model to identify applicants as a “healthy loan” or as a “high risk” loan based on the many factors associated with each applicant. The data is first cleaned and prepared to enter the model, then the model is trained by the data, lastly evaluated to see how effective the model is.   
Results
I created 2 models to test and the results are as follows:
	Model 1:
•	Balanced accuracy score scored at 95%
•	Precision for “healthy loans” was 100%
•	Recall for “healthy loans” was 99%
•	Precision for “high risk loans" was 85%
•	Recall for "high risk loans” was 91%
Model 2:
•	Balanced accuracy score scored at 99%
•	Precision for “healthy loans” was 99%
•	Recall for “healthy loans” was 99%
•	Precision for “high risk loans" was 99%
•	Recall for "high risk loans” was 99%
Summary
While the first model overall did an ok job at predicting “healthy loans”, the model did not do as well predicting “high risk loans”. The second model was extremely accurate at predicting both loans with all statistics scoring out at 99%. It is clear to me that the second model would be preferable to use for identifying the creditworthiness of borrowers. One restraint on the first model that I believe had a huge influence on the results was the discrepancy between the “high risk loan” data and the “healthy loan” data (619-18765).
