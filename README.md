# Predicting Tracheostomy Need in Infants with Severe Bronchopulmonary Dysplasia

# Introduction
This project develops statistical models to predict the need for tracheostomy in infants with severe bronchopulmonary dysplasia (BPD).

The data is from the BPD Collaborative Registry comprising infants <32 weeks gestational age with severe BPD from centers in the US and Sweden. It contains variables on demographics, respiratory support, and clinical status recorded at birth, 36 weeks, 44 weeks, and discharge.

The outcome is a composite tracheostomy/death variable, with 1 indicating tracheostomy or death occurred.

# Data Preprocessing
Converted categorical variables into factors
Corrected invalid entries
Created composite outcome variable
Removed duplicate rows

# Key Findings
Lasso regression and best subset logistic regression performed similarly
Both models had AUC ~0.9 for discrimination
Lasso model more sensitive, logistic model more specific

# Limitations:
High missingness
No interaction terms
No mixed effects for clusters

# Repository Files
project2.rmd: R script for data preprocessing, EDA, modeling, evaluations
project_report.pdf: Full project report
