Predicting High-Value Invoices Based on Country
Overview
This project analyzes retail transaction data to predict whether an invoice qualifies as "high value" based on the customer's country. Using a logistic regression model, the goal is to help businesses identify regions with higher revenue potential.

Objective
To predict whether an invoice's total revenue exceeds $500, based solely on the country associated with the customer.
Tools Used:
Python (Jupyter Notebook)
pandas
scikit-learn
matplotlib

Process
Loaded and cleaned the "Online Retail" dataset.
Created a new Revenue feature by multiplying quantity and unit price.
Aggregated revenue at the invoice level.
Classified invoices as "high-value" based on a $500 revenue threshold.
Merged invoice revenue with country information.
One-hot encoded the country variable.
Built and trained a logistic regression model.
Evaluated model performance using accuracy score and classification report metrics.

Key Findings
The logistic regression model achieved an overall accuracy of 80.2% on the test set.
The model predicted non-high-value invoices (class 0) with high precision (81%) and very high recall (99%), meaning it was extremely good at identifying regular (non-high-value) invoices.
However, the model struggled to correctly predict high-value invoices (class 1), with only 2% recall and 42% precision.
This suggests that using only "Country" as a feature is not sufficient to accurately identify high-value invoices — additional variables (like customer purchase history or invoice totals) would likely improve the model's ability to capture high-value transactions.

Files
Predict_if_an_invoice_is_high_value_based_on_country_using_logistic_regression.ipynb — Full project notebook.

How to Run
Install required libraries: pandas, scikit-learn, matplotlib.
Ensure you have access to the Online Retail.xlsx dataset.
Open the notebook and run each cell sequentially to reproduce the results.

