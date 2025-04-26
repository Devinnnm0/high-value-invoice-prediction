# Predicting High-Value Invoices Based on Country

## Overview
This project analyzes retail transaction data to predict whether an invoice qualifies as "high value" based on the customer's country. Using a logistic regression model, the goal is to help businesses identify regions with higher revenue potential.

## Objective
- Predict whether an invoice's total revenue exceeds $500 based solely on the customer's country.

## Tools Used
- Python (Jupyter Notebook)
- pandas
- scikit-learn
- matplotlib

## Key Findings
- **Model Accuracy:** The logistic regression model achieved an overall accuracy of 80.2% on the test set.
- **Prediction Strength:** The model predicted non-high-value invoices (class 0) with high precision (81%) and very high recall (99%).
- **Limitation:** The model struggled to correctly predict high-value invoices (class 1), with only 2% recall and 42% precision.
- **Business Insight:** Using only "Country" as a predictor is not sufficient to capture high-value invoices accurately. Including additional features such as customer history or invoice totals would likely improve model performance.

## Files
- `Predict_if_an_invoice_is_high_value_based_on_country_using_logistic_regression.ipynb` — Full project notebook including data processing, modeling, and evaluation.

## How to Run
1. Install required libraries: `pandas`, `scikit-learn`, `matplotlib`.
2. Ensure you have access to the `Online Retail.xlsx` dataset.
3. Open the `Predict_if_an_invoice_is_high_value_based_on_country_using_logistic_regression.ipynb` notebook.
4. Run each cell sequentially to reproduce the results.
