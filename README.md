# Predicting Tracheostomy Need in Infants with Severe Bronchopulmonary Dysplasia


# Abstract

Objective: In collaboration with Dr. Chris Schmid, this project aims to develop statistical models for predicting the composite outcome of tracheostomy or death, considering the indication criteria and timing of tracheostomy placement. 
   
Methods: We proposed four models: 1) 36-Week Model Without Interactions; 2) 36-Week Model With Interactions; 3) 44-Week Model Without Interactions; 4) 44-Week Model With Interactions. The first step in model development involves constructing datasets for both the 36-week and 44-week models. We address missing data in each dataset using the multiple imputation technique under the MAR assumption. We then allocate 70\% of each imputed dataset as training data and 30\% as the testing set, ensuring the same proportion of the outcome in both sets through stratification. The variable selection process is conducted using a lasso model. The third step involves examining the frequency table of zero coefficients across the five imputed datasets and removing variables that are nearly zero. Finally, we evaluate the performance of the four proposed models using both discrimination and calibration metrics. 

Results: Overall, all four models demonstrate similarly high performance in predicting the need for tracheostomy in infants with severe bronchopulmonary dysplasia. The 44-week models have a higher AUC score, indicating better performance in distinguishing between the two outcomes. They also have lower Brier scores, suggesting more accurate probabilistic predictions. The 44-week models are more precise in predicting positive cases, while the 36-week models excel in predicting negative cases. In healthcare contexts, where correctly identifying true positives is often crucial due to the potential consequences of missing a serious condition, the 44-week models may be more appropriate.


# Repository Files

Project2.rmd: R script for data preprocessing, EDA, modeling, evaluations

Project2.pdf: Full project report
