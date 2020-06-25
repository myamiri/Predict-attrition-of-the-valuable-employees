# Predicting-Employee-Attrition


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

![attrition1](https://user-images.githubusercontent.com/33470542/85738958-6d361300-b6ce-11ea-8fc0-985dfbb73c3c.png)



- There is a tension between probability threshold and the number of employees who are accurately predicted as potential churners. A high probability threshold would end in a high number of errors. From a business perspective, it's more valuable to predict attrition than it is to predict non-attrition.
- The confusion matrix shows that of all the people who are going to leave the company, our algorithm can lable 70% of them correctly. On the other hand, there is a cost of wrongly identifying attrition of non-leaving employees resulting in inefficiencies in resource allocation.


![attrition2](https://user-images.githubusercontent.com/33470542/85739099-84750080-b6ce-11ea-974e-cb7efb7249c6.png)


- The best overall model is a Ridge Classifier, as it predicts a higher area under the Precision & Recall curve. It is worth noting though, that the Gaussian Naive Bayes did identify a higher percentage of the churning employees accurately.


![attrition6](https://user-images.githubusercontent.com/33470542/85757093-3ddad280-b6dd-11ea-90e3-f55cfe1a3896.png)

![attrition5](https://user-images.githubusercontent.com/33470542/85754880-724d8f00-b6db-11ea-963f-eaa3f535f65e.png)
   




# Solution

In this context, the use of classification models to predict if an employee is likely to quit could increase HR’s ability to mitigate attrition. 
While this model can be routinely run to identify employees who are most likely to quit, the key driver of success would be the human element of reaching out the employee, understanding the current situation of the employee and taking action to remedy controllable factors that can prevent their departure.
In other words, predictive models could help raise flags, but the ultimate solution to this business problem is a function of the organization's culture: the quality of the relationships between HR and any given employee.
