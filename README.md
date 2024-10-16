# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 1. Import the necessary libraries
2. Read the dataset
3. From sklearn.tree import Decision TreeClassifier and use criterion as entropy.
4. Find the accuracy of the model and predict the required values by importing the required module from sklearn.


## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: ARAVIND G
RegisterNumber: 212223240011

import pandas as pd
data=pd, read_csv("Employee.csv")
data. head data.tailo data. info
data. isnull).sum()
data["left*]. value_counts()
from sklearn-preprocessing import LabelEncoder le= LabelEncoder ()
data[ "salary"]=le. fit_transform(data["salary"])
data.head
x=data[["satisfaction_level", "last_evaluation", "number _project", "average_montly_hours" , "tim
x. head ()
y=data["left"]
from sklearn. model_selection import train_test_split
x_train, x_test,y_train,y_test=train_test_split(x,y,test_size=0.2, random_state=42) from sklearn. tree import DecisionTreeClassifier dt-DecisionTreeClassifier (criterion="entropy")
dt. fit(x_train,y_train)
y_pred=dt. predict (x_test)
from sklearn import metrics
accuracy=metrics accuracy_score(y_test,y_pred)
[2:29 pm, 16/10/2024] Aravind♠️: accuracy
dt. predict ([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
![Screenshot 2024-10-16 143127](https://github.com/user-attachments/assets/408e438e-58f2-48d8-947a-4493db0440ee)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
