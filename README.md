# Credit Risk Classification Report

To run the code:

1. Ensure you have the required libraries installed:
   ```bash
   pip install numpy pandas scikit-learn
   ```
2. Place the `lending_data.csv` file in the `Resources` folder.
3. Run the Jupyter Notebook `credit_risk_classification.ipynb` to train and evaluate the model.

### Dependencies

- Python 3.x
- NumPy
- Pandas
- Scikit-learn

This project focuses on building a machine learning model to classify loan applicants as either low-risk (healthy loan) or high-risk (high-risk loan) based on various financial and demographic factors. The model is trained using a dataset containing features such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The goal is to predict the loan status (0 for healthy loan, 1 for high-risk loan) with high accuracy and reliability.

### Dataset

The dataset used in this project is stored in the `Resources` folder and is named `lending_data.csv`. It contains the following columns:

- `loan_size`: The size of the loan.
- `interest_rate`: The interest rate of the loan.
- `borrower_income`: The income of the borrower.
- `debt_to_income`: The debt-to-income ratio of the borrower.
- `num_of_accounts`: The number of accounts the borrower has.
- `derogatory_marks`: The number of derogatory marks on the borrower's credit history.
- `total_debt`: The total debt of the borrower.
- `loan_status`: The status of the loan (0 for healthy loan, 1 for high-risk loan).

### Methodology

#### Data Preprocessing

1. **Data Loading**: The dataset is loaded into a Pandas DataFrame for further processing.
2. **Feature and Label Separation**: The target variable (`loan_status`) is separated from the features.
3. **Train-Test Split**: The data is split into training and testing sets using `train_test_split` from `sklearn.model_selection`.

## Analysis

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
