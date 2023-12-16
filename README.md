# Predicting Tracheostomy Need in Infants with Severe Bronchopulmonary Dysplasia


# Abstract

Objective: In collaboration with Dr. Chris Schmid, this project aims to develop statistical models for predicting the composite outcome of tracheostomy or death, considering the indication criteria and timing of tracheostomy placement. 
   
Methods: We proposed four models: 1) 36-Week Model Without Interactions; 2) 36-Week Model With Interactions; 3) 44-Week Model Without Interactions; 4) 44-Week Model With Interactions. The first step in model development involves constructing datasets for both the 36-week and 44-week models. We address missing data in each dataset using the multiple imputation technique under the MAR assumption. We then allocate 70\% of each imputed dataset as training data and 30\% as the testing set, ensuring the same proportion of the outcome in both sets through stratification. The variable selection process is conducted using a lasso model. The third step involves examining the frequency table of zero coefficients across the five imputed datasets and removing variables that are nearly zero. Finally, we evaluate the performance of the four proposed models using both discrimination and calibration metrics. 

Results: Overall, all four models demonstrate similarly high performance in predicting the need for tracheostomy in infants with severe bronchopulmonary dysplasia. The 44-week models have a higher AUC score, indicating better performance in distinguishing between the two outcomes. They also have lower Brier scores, suggesting more accurate probabilistic predictions. The 44-week models are more precise in predicting positive cases, while the 36-week models excel in predicting negative cases. In healthcare contexts, where correctly identifying true positives is often crucial due to the potential consequences of missing a serious condition, the 44-week models may be more appropriate.

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
