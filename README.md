# German Credit Risk Analysis
## Project Overview
This project focuses on analyzing the German Credit Dataset, which contains information about 1,000 loan applicants. Each applicant is classified as either a "Good" or "Bad" credit risk based on various attributes. The dataset includes both numerical and categorical features that describe the applicants' demographic and financial status. The goal of this project is to cluster the customers and classify whether an applicant is considered a good or bad credit risk.

## Dataset Information
### Context
The German Credit Dataset originally contains 20 categorical/symbolic attributes, but only a selected set of relevant attributes are used in this analysis. The dataset includes attributes such as age, sex, job, housing status, savings accounts, checking accounts, credit amount, duration of the loan, and the purpose of the loan. The target variable is the credit risk, which is classified as either "Good" or "Bad."

### Selected Attributes
- Age (numeric)
- Sex (text: male, female)
- Job (numeric: 0 - unskilled and non-resident, 1 - unskilled and resident, 2 - skilled, 3 - highly skilled)
- Housing (text: own, rent, or free)
- Saving accounts (text - little, moderate, quite rich, rich)
- Checking account (numeric, in DM - Deutsch Mark)
- Credit amount (numeric, in DM)
- Duration (numeric, in months)
- Purpose (text: car, furniture/equipment, radio/TV, domestic appliances, repairs, education, business, vacation/others)
- Risk (Target value - Good or Bad Risk)
** Project Tasks
The project is structured into several key steps to achieve the goal of clustering customers and classifying credit risk:

### 1. Exploratory Data Analysis (EDA) and Data Cleaning
EDA: Perform an exploratory analysis to understand the distribution of the data, identify any missing values or outliers, and observe relationships between features.
Data Cleaning: If necessary, clean the data by handling missing values, correcting data types, or removing irrelevant columns.
### 2. One-Hot Encoding
Categorical Encoding: Apply one-hot encoding to convert categorical variables into numerical form, enabling them to be used in machine learning models.
### 3. Visualization and Log Transformation
Histograms: Visualize the distribution of numerical features using histograms to check for skewness.
Log Transformation: If skewness is observed, apply log transformation to normalize the data. Re-check the histograms to ensure normalization.
### 4. Feature Scaling
Scaling: Apply feature scaling to standardize the numerical features, making them suitable for clustering and classification.
### 5. Clustering
Numerical Features Only: Use only numerical features for the clustering process.
Elbow Method: Apply the elbow method to determine the optimal number of clusters. Plot the graph to visualize the results.
PCA Visualization: Use Principal Component Analysis (PCA) to reduce the dimensionality and visualize the clusters.
### 6. Classification
- KFOLD Cross-Validation: Implement KFOLD cross-validation to evaluate the performance of your chosen classifier.
- Classification: Use a classifier of your choice (e.g., Logistic Regression, Random Forest, SVM, XGBoost) to classify applicants as "Good" or "Bad" credit risks.      
- Evaluation Metrics: Report the evaluation metrics, including accuracy, precision, recall, F1-score, and any other relevant metrics.
## Conclusion
This project aims to provide a comprehensive analysis of the German Credit Dataset by clustering the customers and classifying credit risks. Through EDA, feature scaling, clustering, and classification, the project seeks to develop a model that can accurately assess the credit risk of loan applicants. The insights gained from this analysis can be valuable for banks and financial institutions in making informed decisions regarding loan approvals.
