# Analysis Report

## Credit Risk Classification

> The purpose of this analysis is to evaluate the performance of a machine learning model designed to classify loan applicants as either low-risk (0) or high-risk (1). The dataset consists of financial information such as loan size, interest rates, borrower income, debt-to-income ratio, and other factors that could influence credit risk. The target variable in this analysis is loan_status, which has two possible values:

	•  Low Risk (0) – Borrowers who are likely to repay their loans.

	•  High Risk (1) – Borrowers who pose a higher likelihood of default.

## Machine Learning Process

	•	Data Preprocessing – The dataset was loaded, and the features (X) and labels (y) were defined.

	•	Splitting the Data – The data was divided into training and testing sets to evaluate model performance.

	•	Model Selection – A Logistic Regression model was used to classify loan applicants based on their financial attributes.

	•	Model Evaluation – Performance was assessed using accuracy, precision, and recall scores.


## Results

	•  Accuracy: 99%

	•  Precision:
		• Low-Risk (0): 100%
		• High-Risk (1): 84%

	•  Recall:
		• Low-Risk (0): 99%
		• High-Risk (1): 94%


## Summary

 > The Logistic Regression model performed exceptionally well, achieving a **99% accuracy rate**. It was > particularly effective in identifying low-risk borrowers, with **100% precision**, meaning that all predicted low-risk loans were indeed low-risk. For high-risk borrowers:
 - The recall score of 94% indicates that the model successfully identified most high-risk applicants.

 - However, the 84% precision means that some borrowers classified as high-risk might actually be low-risk.

> I recommend using this model for credit risk classification. It is highly accurate and effectively identifies high-risk borrowers, which is crucial for minimizing financial risk. However, given the lower precision for high-risk classifications, additional validation steps—such as manual review of high-risk applicants—may be necessary before final loan decisions are made.