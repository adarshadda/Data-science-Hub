# Employee-Attrition-Classification

The dataset for this project originates from the Synthetic Employee Attrition Dataset

## Context
The Synthetic Employee Attrition Dataset is a simulated dataset designed for the analysis and prediction of employee attrition. It contains detailed information about various aspects of an employee's profile, including demographics, job-related features, and personal circumstances.

This dataset is ideal for HR analytics, machine learning model development, and demonstrating advanced data analysis techniques. It provides a comprehensive and realistic view of the factors affecting employee retention, making it a valuable resource for researchers and practitioners in the field of human resources and organizational development.

## Problem Statement:
The goal is to understand the factors contributing to attrition and develop predictive models to identify at-risk employees.


## Dataset
Number of Instances--> 74498
Number of Attributes--> 24
Numeric Features--> 8
Categorical Features--> 16

## Attribute Information
The dataset comprises **74,498** samples, split into training and testing sets to facilitate model development and evaluation. Each record includes a unique Employee ID and features that influence employee attrition.

**Input variables**:

1) **Employee ID**: A unique identifier assigned to each employee.

2) **Age**: The age of the employee, ranging from 18 to 60 years.

3) **Gender**: The gender of the employee

4) **Years at Company**: The number of years the employee has been working at the company.

5) **Monthly Income**: The monthly salary of the employee, in dollars.

6) **Job Role**: The department or role the employee works in, encoded into categories such as Finance, Healthcare, Technology, Education, and Media.

7) **Work-Life Balance**: The employee's perceived balance between work and personal life, (Poor, Below Average, Good, Excellent)

8) **Job Satisfaction**: The employee's satisfaction with their job: (Very Low, Low, Medium, High)

9) **Performance Rating**: The employee's performance rating: (Low, Below Average, Average, High)

10) **Number of Promotions**: The total number of promotions the employee has received.

11) **Distance from Home**: The distance between the employee's home and workplace, in miles.

12) **Education Level**: The highest education level attained by the employee: (High School, Associate Degree, Bachelor’s Degree, Master’s Degree, PhD)

13) **Marital Status**: The marital status of the employee: (Divorced, Married, Single)

14) **Job Level**: The job level of the employee: (Entry, Mid, Senior)

15) **Company Size**: The size of the company the employee works for: (Small,Medium,Large)

16) **Company Tenure**: The total number of years the employee has been working in the industry.

17) **Remote Work**: Whether the employee works remotely: (Yes or No)

18) **Leadership Opportunities**: Whether the employee has leadership opportunities: (Yes or No)

19) **Innovation Opportunities**: Whether the employee has opportunities for innovation: (Yes or No)

20) **Company Reputation**: The employee's perception of the company's reputation: (Very Poor, Poor,Good, Excellent)

21) **Employee Recognition**: The level of recognition the employee receives:(Very Low, Low, Medium, High)

**Output variable (desired target)**:
22) **Attrition**: Whether the employee has left the company, encoded as 0 (stayed) and 1 (Left).


## Conclusion

During the analysis the given problem of predicting the attrition we found that the problem is a binary classiffication problem and the dataset given is balanced with respect different categories of target feature (attrition).

We built different classifier for the given problem like ADA Boosting, Logistic Regression, Random Forest but ADA Boosting outperformed other classifiers with test accuracy of **75.5** and a f1-score of **75.4**.

The analysis of feature importance underscores that job-related factors, such as **job level** and **job satisfaction**, along with personal factors like **income** and **work-life balance**, are critical in understanding employee attrition. By focusing on these areas, organizations can implement strategies to improve retention and address key issues that may lead to higher employee turnover.



