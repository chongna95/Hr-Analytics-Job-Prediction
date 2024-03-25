# Hr Analytics Job Prediction
Data Set of Hr Department to Predict Employees Behaviour

# Overview 
The goal of this project was to create a logistic regression or tree-based machine learning model to predict whether or not an employee will leave the company. This project utilized employee satisfaction levels taken from The HR department at Salifort Motors company. The final random forest model performed with 94.4% AUC, 86.9% precision, 92% recall , 89.1% f1-score, and 96.3% accuracy determining what features had most impact on employee retention. Based on the model, last_evaluation, number_project, tenure and overworked were most influential in determining a employee left or not left the company.

# Business Understanding 
For HR Department, It is time-consuming and expensive to find, interview, and hire new employees. It is important to understand what factors make the employee leave the company in order to increase employee retention which will be beneficial to the company.

# Data Understanding
The HR dataset came from [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv). The data consisted of 15,000 employee and 10 features listed below. The bar chart below shows the breakdown of how many generous tippers (>20%) versus non-generous tippers that exist in the data set. 
Variable  |Description |
-----|-----|
satisfaction_level|Employee-reported job satisfaction level [0&ndash;1]|
last_evaluation|Score of employee's last performance review [0&ndash;1]|
number_project|Number of projects employee contributes to|
average_monthly_hours|Average number of hours employee worked per month|
time_spend_company|How long the employee has been with the company (years)
Work_accident|Whether or not the employee experienced an accident while at work
left|Whether or not the employee left the company
promotion_last_5years|Whether or not the employee was promoted in the last 5 years
Department|The employee's department
salary|The employee's salary (U.S. dollars)


# Modeling and Evaluation 
# Conclusion
