# Predicting Tracheostomy Need in Infants with Severe Bronchopulmonary Dysplasia

# Introduction

This project develops statistical models to predict the need for tracheostomy or death in infants with severe bronchopulmonary dysplasia (BPD).

BPD is a chronic lung disease resulting from preterm birth and mechanical ventilation. Tracheostomy may benefit infants with severe BPD but also has risks. Accurately predicting tracheostomy need could enable targeted interventions to improve outcomes.

The data originates from the Bronchopulmonary Dysplasia (BPD) Collaborative Registry, containing 996 infants <32 weeks gestational age with severe BPD from 9 centers in the US and Sweden.

# Data Preprocessing

* Converted categorical variables into factors

* Corrected invalid entries

* Created composite outcome variable

* Removed duplicate rows

# Key Findings

* Lasso AUC: 0.900, Sensitivity: 0.855, Specificity: 0.796

* Logistic Regression AUC: 0.884, Sensitivity: 0.766, Specificity: 0.852

# Limitations

* Multiple imputation may introduce bias

* No interaction terms or random effects


# Repository Files

Project2.rmd: R script for data preprocessing, EDA, modeling, evaluations

Project2.pdf: Full project report
