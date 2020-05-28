# Predicting-Attrition-of-Valuable-Employees


# Problem

Attrition is a problem that impacts all businesses, irrespective of geography, industry and size of the company. 
Employee attrition leads to significant costs for a business, including the cost of business disruption, hiring new staff and training new staff. 
As such, there is great business interest in understanding the drivers of, and minimizing staff attrition.




# Data

This data set presents an employee survey from IBM, indicating if there is attrition or not. 
The data set contains approximately 1500 entries. Given the limited size of the data set, the model should 
only be expected to provide modest improvement in indentification of attrition vs a random allocation of probability of attrition.
IBM has gathered information on employee satisfaction, income, seniority and some demographics. It includes the data of 1470 employees. 
To use a matrix structure, we changed the model to reflect the followin data




# Solution

In this context, the use of classification models to predict if an employee is likely 
to quit could greatly increase the HR’s ability to intervene on time and remedy the situation to prevent attrition. 
While this model can be routinely run to identify employees who are most likely to quit, the key driver of success would be 
the human element of reaching out the employee, understanding the current situation of the employee and taking action to remedy controllable factors that can prevent attrition of the employee.


# Modeling

We plan to run : 
Support Vecror Machine
Logestic Regression
Quadratic Discriminant Analysis
Extra Tree Classifier
Xgboost classifier
Light GBM
CatBoost Classifier
AdaBoost Classifier
Bagging Classifier
RandomForest Classifier
Stacking Classifier
Voting Classifier
Gaussian Naive Bayes (GaussianNB)
Gaussian Process Classifier
Ridge Classifier
Decision Tree Classifier
KNeighbors Classifier
models  to determine the probability of a certain employee to fall into the condition of Attrition and thus its high risk of leaving the company.
We will then test different parameters and probability threshold using confusion Matrixes, precision recall curve and ROC curve to determine which of the models is the best predictor and will reccommend its use in practice






# Result

- Model is biased towards predicting non attrition.
- There is a tension between probability threshold and the number of employees who are accurately predicted as potential churners. A high probability threshold would end in a high number of errors. The business relevance is predict attrition well, rather than non attrition hence a lower probability threshold is chosen.
- The confusion matrix shows that of all the people who are going to leave the company, our algorithm identifies about 43% of them accurately. On the other hand, there is a cost of wrongly identifying attrition of non-leaving employees resulting in inefficiencies in resource allocation.
- Ridge Classifier is the best model, as it predictS a higher area under the roc curve while Gaussian Naive Bayes is the best model, as it identifies higher percent of employees are leaving the company accurately.
