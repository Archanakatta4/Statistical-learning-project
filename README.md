## Analysis of Cardiovascular Disease Risk Factors
## Project Overview
This project utilizes the Framingham Heart Study dataset to predict the 10-year risk of coronary heart disease (CHD) based on various demographic, clinical, and lifestyle factors. The dataset, originally sourced from Kaggle, contains over 4,240 records and 16 attributes, including blood pressure, cholesterol levels, smoking status, and other relevant health metrics. This prediction model serves as a tool for assessing CHD risk and is designed to aid in clinical decision-making and preventive healthcare strategies.

## Dataset
Source: Framingham Heart Study, via Kaggle.
Attributes: 16 attributes, including age, sex, cholesterol, blood pressure, BMI, smoking habits, diabetes status, etc.
Objective: Predict the likelihood of developing CHD within the next 10 years.

## Installation and Setup
Prerequisites
R (Version >= 4.0)
Required libraries: tidyverse, caret, ggplot2, dplyr, randomForest, pROC.

## Data Preprocessing
Missing Values: The dataset contains missing values, which are removed using na.omit().
Feature Transformation: Some variables are converted to factors, and numeric variables are scaled for consistent feature scaling.
Data Split: The data is split into training (80%) and testing (20%) sets using stratified sampling to preserve the distribution of target variables.

## Exploratory Data Analysis (EDA)
EDA includes visualizations to investigate the relationships between key predictors (e.g., age, cholesterol, systolic blood pressure) and CHD risk by gender. This analysis reveals trends such as:

Older individuals and higher cholesterol levels correlate with an increased CHD risk.
Lifestyle factors, including smoking status and glucose levels, show potential impact on CHD outcomes.

## Feature Engineering and Selection
Features were selected through stepwise regression to enhance model performance. Selected predictors included:

Sex
Age
Cigarettes per day
Prevalent stroke
Systolic blood pressure (sysBP)
Total cholesterol (totChol)

## Modeling
The project employs a Random Forest classifier due to its robustness in handling high-dimensional data and complex relationships:
Model performance was assessed using accuracy, precision, recall, F1-score, and the ROC-AUC metric.

## Results
The model achieved an accuracy of approximately 85% and an AUC of 0.69, indicating effective performance in distinguishing high-risk from low-risk individuals.

## Conclusion
The Random Forest model provides valuable insights for CHD risk prediction, with high sensitivity and robust accuracy, making it a reliable tool for clinical risk assessment. Future research could further enhance the model's performance by integrating additional variables or testing advanced machine learning methods.



