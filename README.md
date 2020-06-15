# Predicting-Attrition-of-Valuable-Employees


# Problem

Attrition is a problem that impacts all businesses, irrespective of geography, industry or size. 
Employee attrition leads to significant costs for a business, including the cost of business disruption, hiring new staff and training new staff. 
As such, there is great business interest in understanding the drivers of, and minimizing staff attrition.




# Data

This data set presents an employee survey from IBM, indicating if there is attrition or not. 
The data set contains approximately 1500 entries. Given the limited size of the data set, the model should 
only be expected to provide modest improvement in indentification of attrition vs a random allocation of probability of attrition.
IBM has gathered information on employee satisfaction, income, seniority and some demographics. It includes the data of 1470 employees. 
To use a matrix structure, we changed the model to reflect the following data.







# Modeling

We plan to run: Support Vector Machine, Logistic Regression, Quadratic Discriminant Analysis, Extra Tree Classifier, Xgboost Classifier, Light GBM, CatBoost Classifier, AdaBoost Classifier, Bagging Classifier, RandomForest Classifier, Stacking Classifier, Voting Classifier, Gaussian Naive Bayes (GaussianNB), Gaussian Process Classifier, Ridge Classifier, Decision Tree Classifier, KNeighbors Classifier models to determine the probability that a certain employee will leave the company.
We will then test different parameters and probability thresholds using Confusion Matrices, Precision & Recall curves and ROC/AUC curves to determine which of the models has the most predictive power.






# Result

- Model is biased towards predicting non attrition.
- There is a tension between probability threshold and the number of employees who are accurately predicted as potential churners. A high probability threshold would end in a high number of errors. From a business perspective, it's more valuable to predict attrition than it is to predict non-attrition.
- The confusion matrix shows that of all the people who are going to leave the company, our algorithm identifies about 43% of them accurately. On the other hand, there is a cost of wrongly identifying attrition of non-leaving employees resulting in inefficiencies in resource allocation.
- The best overall model is a Ridge Classifier, as it predicts a higher area under the ROC curve. It is worth noting though, that the Gaussian Naive Bayes did identify a higher percentage of the churning employees accurately.



# Solution

In this context, the use of classification models to predict if an employee is likely to quit could increase HR’s ability to mitigate attrition. 
While this model can be routinely run to identify employees who are most likely to quit, the key driver of success would be the human element of reaching out the employee, understanding the current situation of the employee and taking action to remedy controllable factors that can prevent their departure.
In other words, predictive models could help raise flags, but the ultimate solution to this business problem is a function of the organization's culture: the quality of the relationships between HR and any given employee.
