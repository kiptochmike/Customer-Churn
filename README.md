# Telecommunications Customer Churn Prediction Project

## Table of Contents
1. [Overview](#overview)
2. [Project Phases](#project-phases)
    - [Business Understanding](#business-understanding)
    - [Data Understanding](#data-understanding)
    - [Data Preparation](#data-preparation)
    - [Modeling](#modeling)
    - [Evaluation](#evaluation)
    - [Conclusion](#conclusion)
    - [Recommendation](#recommendation)
    - [Next Steps](#next-steps)

## Overview:
This project aims to develop a predictive model to identify customers likely to churn for SyriaTel, a telecommunications company. Customer churn poses a significant challenge in the telecommunications industry, leading to revenue loss and affecting a company's market position. By accurately predicting churn, SyriaTel can implement proactive retention strategies to mitigate its financial impact and improve customer satisfaction.

## Project Phases:

### Business Understanding:
Identify the problem of customer churn in the telecommunications industry and its impact on SyriaTel's financial performance and market position. Define the objective of developing a classifier to predict customer churn and aid in implementing proactive retention strategies.

### Data Understanding:
Obtain a dataset from Kaggle consisting of 21 columns and 3333 rows, containing relevant information for predicting customer churn. Each row represents a customer, and each column represents features related to customer behavior, demographics, and interactions with SyriaTel's services.
The columns are as follows: 
- **state:** the state the user lives in
- **account length:** the number of days the user has this account
- **area code:** the code of the area the user lives in
- **phone number:** the phone number of the user
- **international plan:** true if the user has the international plan, otherwise false
- **voice mail plan:** true if the user has the voice mail plan, otherwise false
- **number vmail messages:** the number of voice mail messages the user has sent
- **total day minutes:** total number of minutes the user has been in calls during the day
- **total day calls:** total number of calls the user has done during the day
- **total day charge:** total amount of money the user was charged by the Telecom company for calls during the day
- **total eve minutes:** total number of minutes the user has been in calls during the evening
- **total eve calls:** total number of calls the user has done during the evening
- **total eve charge:** total amount of money the user was charged by the Telecom company for calls during the evening
- **total night minutes:** total number of minutes the user has been in calls during the night
- **total night calls:** total number of calls the user has done during the night
- **total night charge:** total amount of money the user was charged by the Telecom company for calls during the night
- **total intl minutes:** total number of minutes the user has been in international calls
- **total intl calls:** total number of international calls the user has done
- **total intl charge:** total amount of money the user was charged by the Telecom company for international calls
- **customer service calls:** number of customer service calls the user has done
- **churn:** true if the user terminated the contract, otherwise false

### Data Preparation:
Clean the dataset by handling missing values, encoding categorical variables, and scaling numerical features. Perform exploratory data analysis to understand the distribution of features and identify potential correlations with customer churn.

### Modeling:
Train multiple machine learning models, including Logistic Regression, Decision Trees, Random Forest, and XGBoost, to predict customer churn. Evaluate the performance of each model using metrics such as accuracy, precision, recall, F1-score, and AUC ROC.

### Evaluation:
XGBoost model is the best performing model for predicting customer churn. Evaluate its performance based on accuracy, precision, recall, F1-score, and AUC ROC, compared to other algorithms.

### Conclusion:
XGBoost is the most suitable model for predicting customer churn, exhibiting superior accuracy and AUC score compared to other algorithms. Emphasize the importance of rigorous evaluation and model selection in addressing the problem of customer churn.

### Recommendation:
Provide recommendations for SyriaTel to reduce customer churn, including implementing proactive retention strategies, improving service quality, enhancing communication channels, and leveraging data-driven decision-making.

### Next Steps:
refining models for better predictive performance, enriching data with additional relevant features, deploying the final model into production systems, and monitoring its performance over time.

This project focuses on predicting customer churn for SyriaTel, a telecommunications company, to aid in implementing proactive retention strategies. It involves data preparation, model training, evaluation, and recommendations for reducing customer churn. The XGBoost model is identified as the best performing model, with recommendations provided for SyriaTel to improve customer retention and leverage data-driven decision-making. Future steps include refining models, enriching data, deploying the final model, and monitoring its performance.



