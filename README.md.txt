# Telco Customer Churn Analysis

## Project Overview

This project analyzes customer churn for a telecommunications company. The objective was to identify the customer segments most likely to churn, build predictive models, and provide data-driven retention recommendations.

## Business Problem

Customer churn reduces recurring revenue and increases customer acquisition costs. This project investigates the factors associated with churn and identifies high-risk customers for targeted retention efforts.

## Dataset

The dataset contains 7,032 customer records and 21 variables, including:

- Customer demographics
- Contract type
- Internet service type
- Payment method
- Monthly charges
- Total charges
- Customer tenure
- Churn status

## Tools Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Power BI

## Data Cleaning

The following preparation steps were completed:

- Corrected the CSV delimiter issue
- Converted `TotalCharges` to a numeric data type
- Removed 11 records with missing total charges
- Checked for duplicate customer IDs
- Created customer tenure groups for churn analysis
- Prepared categorical variables for machine learning using one-hot encoding

## Key Findings

| Churn Driver | High-Risk Segment | Churn Rate |
|---|---|---:|
| Customer tenure | 0–12 months | 47.7% |
| Payment method | Electronic check | 45.3% |
| Contract type | Month-to-month | 42.7% |
| Internet service | Fiber optic | 41.9% |
| Customer segment | Senior citizens | 41.7% |

Overall, 26.6% of customers churned.

## Predictive Modeling

Two classification models were tested:

| Model | Accuracy | Churn Recall |
|---|---:|---:|
| Logistic Regression | 78.9% | 47% |
| XGBoost | 79.5% | 53% |

XGBoost was selected as the stronger model because it identified more customers who eventually churned.

## Business Recommendations

1. Improve onboarding and engagement during the first 12 months of service.
2. Encourage month-to-month customers to upgrade to annual or two-year contracts.
3. Offer incentives for Electronic Check customers to switch to automatic payment methods.
4. Review Fiber optic pricing, service quality, and customer support.
5. Provide targeted support and retention offers for senior customers.

## Dashboard

The Power BI dashboard includes:

- Executive churn KPIs
- Churn analysis by contract, internet service, payment method, and tenure
- Customer risk segmentation
- Retention recommendations

## Conclusion

The analysis found that churn is concentrated among newer customers with month-to-month contracts, Fiber optic internet service, and Electronic Check payment methods. Retention strategies focused on these segments could reduce customer attrition and protect recurring revenue.