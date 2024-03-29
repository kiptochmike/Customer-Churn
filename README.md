# Telecommunications Customer Churn Prediction Project
#Author : MIKE KIPTOCH

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
### Modeling

#### Logistic Regression
- **Description**: Logistic Regression is a statistical method for analyzing a dataset in which there are one or more independent variables that determine an outcome.
- **Advantages**: It's a simple and interpretable model that provides probabilities for outcomes.
- **Disadvantages**: It assumes a linear relationship between the independent variables and the log odds of the outcome.
- **Implementation**:used the Logistic Regression model from the scikit-learn library.

#### Decision Trees
- **Description**: Decision Trees are a type of supervised learning algorithm that is used for classification and regression tasks.
- **Advantages**: They are easy to understand and visualize, and they can handle both numerical and categorical data.
- **Disadvantages**: They are prone to overfitting, especially with complex datasets.
- **Implementation**:  utilized the DecisionTreeClassifier from the scikit-learn library.

#### Random Forest
- **Description**: Random Forest is an ensemble learning method that operates by constructing multiple decision trees during training and outputting the mode of the classes as the prediction of individual trees.
- **Advantages**: It reduces overfitting by averaging multiple decision trees and provides high accuracy.
- **Disadvantages**: It can be computationally expensive and may not perform well on very large datasets.
- **Implementation**: employed the RandomForestClassifier from the scikit-learn library.

#### XGBoost
- **Description**: XGBoost (Extreme Gradient Boosting) is an efficient implementation of the gradient boosting framework, designed for speed and performance.
- **Advantages**: It achieves state-of-the-art results on a variety of machine learning tasks and is highly customizable.
- **Disadvantages**: It may require careful tuning of hyperparameters to prevent overfitting.
- **Implementation**:  utilized the XGBClassifier from the XGBoost library.


### Evaluation:


- **Logistic Regression**: Achieves moderate accuracy and precision, but relatively lower recall compared to other models. The AUC-ROC score indicates good overall performance, suggesting that it's effective at distinguishing between classes.

- **Decision Tree**: Exhibits lower accuracy, precision, and recall compared to Logistic Regression. The AUC-ROC score is also lower, indicating suboptimal performance. Decision Tree may not generalize well to unseen data.

- **Random Forest**: Shows improvement in accuracy, precision, and recall compared to the Decision Tree model. However, its AUC-ROC score remains relatively low, suggesting that it may not be as effective in distinguishing between classes.

- **XGBoost**: Emerges as the best-performing model with the highest accuracy, precision, recall, F1-score, and AUC-ROC score among all models evaluated. XGBoost demonstrates superior predictive capability and is the most suitable model for predicting customer churn in this context.

In summary, while all models provide some level of predictive capability, XGBoost stands out as the most effective model for accurately predicting customer churn. Its superior performance across various evaluation metrics makes it the preferred choice for deployment in practical applications.

### Conclusion:
XGBoost is the most suitable model for predicting customer churn, exhibiting superior accuracy and AUC score compared to other algorithms. Emphasize the importance of rigorous evaluation and model selection in addressing the problem of customer churn.

### Recommendation:
Provide recommendations for SyriaTel to reduce customer churn, including implementing proactive retention strategies, improving service quality, enhancing communication channels, and leveraging data-driven decision-making.

### Next Steps:
refining models for better predictive performance, enriching data with additional relevant features, deploying the final model into production systems, and monitoring its performance over time.

This project focuses on predicting customer churn for SyriaTel, a telecommunications company, to aid in implementing proactive retention strategies. It involves data preparation, model training, evaluation, and recommendations for reducing customer churn. The XGBoost model is identified as the best performing model, with recommendations provided for SyriaTel to improve customer retention and leverage data-driven decision-making. Future steps include refining models, enriching data, deploying the final model, and monitoring its performance.



