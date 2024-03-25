# Hr Analytics Job Prediction
Data Set of Hr Department to Predict Employees Behaviour

# Overview 
The goal of this project was to create a logistic regression or tree-based machine learning model to predict whether or not an employee will leave the company. This project utilized employee satisfaction levels taken from The HR department at Salifort Motors company. The final random forest model performed with 94.4% AUC, 86.9% precision, 92% recall , 89.1% f1-score, and 96.3% accuracy determining what features had most impact on employee retention. Based on the model, last_evaluation, number_project, tenure and overworked were most influential in determining a employee left or not left the company.

# Business Understanding 
For HR Department, It is time-consuming and expensive to find, interview, and hire new employees. It is important to understand what factors make the employee leave the company in order to increase employee retention which will be beneficial to the company.

# Data Understanding
The HR dataset came from [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv). The data consisted of 15,000 employee and 10 features listed below. 

Variable  |Description |
-----|-----|
satisfaction_level|Employee-reported job satisfaction level [0&ndash;1]
last_evaluation|Score of employee's last performance review [0&ndash;1]
number_project|Number of projects employee contributes to
average_monthly_hours|Average number of hours employee worked per month
time_spend_company|How long the employee has been with the company (years)
Work_accident|Whether or not the employee experienced an accident while at work
left|Whether or not the employee left the company
promotion_last_5years|Whether or not the employee was promoted in the last 5 years
Department|The employee's department
salary|The employee's salary (U.S. dollars)

### Outliers
The boxplot below shows distribution of `tenure` and detect any outliers exist in dataset.

![alt text](https://github.com/chongna95/Hr-Analytics-Job-Prediction/blob/main/images/Boxplot%20of%20Tenure.png)

- For Logistic Regression Model: Remove Outliers
- For Tree-based Machine Learning Model: Robust to Outliers

### Feature Engineering
In this case, it's likely that the company won't have satisfaction levels reported for all of its employees. It's also possible that the average_monthly_hours column is a source of some data leakage. If employees have already decided upon quitting, or have already been identified by management as people to be fired, they may be working fewer hours. Represent Feature Engineering by dropping redundant columns and creating new features from existing features.

# Modeling and Evaluation 
A random forest model comprising 500 decision trees was used to determine feature importance in employee would left or not. The below plot shows that  last_evaluation, number_project, tenure and overworked were the Top 4 most important factors in determining whether or not an employee will leave the company. The overall model performed with 4.4% AUC, 86.9% precision, 92% recall , 89.1% f1-score, and 96.3% accuracy.

![alt text](https://github.com/chongna95/Hr-Analytics-Job-Prediction/blob/main/images/Random%20Forest%20Feature%20Importance.png)

# Conclusion
This model can benefit HR Department in knowing if an employee will leave the company or not. In the future, try building a K-means model on this data and analyzing the clusters may also be beneficial in helping the stakeholder address their business problem. 
