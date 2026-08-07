# Customer-Churn-Prediction-with-Retention-Analysis-and-Customer-Segmentation-on-Telecom-Dataset
Exploratory Data Analysis (EDA) on IBM Telecom Dataset 7,043 customer records to identify attrition drivers.
Tech Stack :  Python, Pandas, NumPy, Matplotlib, Seaborn

Key Findings: Churn Rate: ~26.5% total churn (1,869 churned vs. 5,174 retained). Risk Factor: High churn in early tenure months.  Drivers: Competitor offers &amp; better devices.  

Dataset Overview: The project analyzes the Telco_customer_churn.xlsx dataset, containing 7,043 rows and 33 columns detailing customer demographics, account information, and service usage:  Customer Demographics: Gender, Senior Citizen, Partner, Dependents  Account Metrics: Contract Type, Payment Method, Paperless Billing, Monthly Charges, Total Charges, Tenure Months  Customer Value: Customer Lifetime Value (CLTV), Churn Score  Target Variables: Churn Label (Yes/No), Churn Value (1/0), Churn Reason.

Random Forest Algorithm
  Type: Supervised Ensemble Algorithm (Classification and Regression).
  Core Mechanism: Builds multiple Decision Trees during training and merges their outputs (voting for classification, averaging for regression) to            improve accuracy and control overfitting.
  Application on your Dataset:Target Variable: Churn Value (or Churn Label).
     Feature Selection: Uses continuous variables like Tenure Months, Monthly Charges, CLTV, as well as categorical features (after one-hot encoding)              like Contract or Payment Method.
     Key Insights: Provides Feature Importance scores, allowing you to see which factors (e.g., contract length, monthly fees) contribute most heavily to          customer churn.
     Recall: 74% and Accuracy: 78%

K-Means Clustering Algorithm
  Type: Unsupervised Clustering Algorithm.
  Core Mechanism: Partitions N observations into K distinct clusters based on feature similarity (Euclidean distance to cluster centroids).
  Application on your Dataset:
     Target Variable: None required.
     Use Case (Customer Segmentation): Groups customers based on behavioral and financial metrics such as Monthly Charges, Tenure Months, and CLTV.
     Key Insights: Identifies distinct customer personas (e.g., High Value - High Risk vs. Low Spending - Long Tenure) to help tailor marketing or retention strategies.
