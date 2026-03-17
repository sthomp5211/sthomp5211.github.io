# Early Stage Diabetes Risk Profiling

## Overview
This project evaluated whether symptom based data could be used to identify patients at elevated risk of diabetes and support a simple screening rule for clinics with limited testing capacity.
The analysis was based on the UCI Early Stage Diabetes Risk dataset, which includes approximately 520 patient records and physician verified symptom indicators.

## Business or Clinical Question
Can a short symptom based screener help clinics accurately identify high risk patients more efficiently when diagnostic testing resources are limited?

## Dataset
- Source: UCI Early Stage Diabetes Risk Prediction dataset
- Sample size: Approximately 520 patients
- Outcome: Diabetes positive or negative
- Predictors: Age, gender, and 14 symptom indicators

## Methods

The analysis included:
- data preprocessing and quality review
- exploratory analysis of symptom prevalence by diabetes status
- Welch t test for age differences
- chi square testing for symptom associations
- multivariable logistic regression
- ROC and AUC analysis for threshold evaluation

## Key Findings
- Several symptoms showed strong association with diabetes status, especially **polydipsia**, **polyuria**, and **sudden weight loss**
- Patients classified as positive for diabetes were older on average
- The multivariable logistic regression model identified strong symptom based predictors even after adjustment
- The model achieved excellent discrimination with an **AUC of approximately 0.96**
- A simple decision rule could support fast triage in settings with limited lab capacity

- ## Why This Project Matters

- This project demostrates how statistical modeling can be translated into a practical screening recommendation. Rather than stopping at model performance, the analysis connects findings to an operational decision: how to prioritize scarce testing slots in a rural clinical setting.

- ## Tools Used

  - R
  - tidyverse
  - ggplot2
  - logistic regression
  - ROC analysis
 
  ## Project Deliverables

  - presentation deck
  - statistical analysis in R
  - ROC and threshold interpretation
  - screening recommnedation based on risk indicators
 
  ## Next Improvements

  If I were extending this project further, I would add:

  - model comparision across logistic regression, decision tree, and random forest
  - confusion matrix and classification metrics at selected thresholds
  - calibration analysis
  - a reproducible Github reposistory with cleaned scripts and figures
  
