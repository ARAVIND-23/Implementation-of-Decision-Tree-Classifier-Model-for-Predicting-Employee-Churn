# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas module and import the required data set.
2. Find the null values and count them.
3. Count number of left values.
4. From sklearn import LabelEncoder to convert string values to
numerical values.
5. From sklearn.model_selection import train_test_split.
6. Assign the train dataset and test dataset.
7. From sklearn.tree import DecisionTreeClassifier.
8. Use criteria as entropy.
9. From sklearn import metrics.
10. Find the accuracy of our model and predict the require values.

## Program & Output:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: ARAVIND G
RegisterNumber: 212223240011

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
```
![Screenshot 2024-10-16 151808](https://github.com/user-attachments/assets/a5222402-5282-4ce5-a3e9-0406b55ca386)
```
data.info()
```
![Screenshot 2024-10-16 151952](https://github.com/user-attachments/assets/f208cc7c-03bb-4827-ba7c-f60cfef7fd12)
```
data.isnull().sum()
```
![Screenshot 2024-10-16 152139](https://github.com/user-attachments/assets/63a39c28-8df7-4198-85ec-8a19d5ba7793)
```
data["left"].value_counts()
```
![Screenshot 2024-10-16 152414](https://github.com/user-attachments/assets/b084e8b1-de2f-4695-9872-e32160046378)
```
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
```
![Screenshot 2024-10-16 152530](https://github.com/user-attachments/assets/56a84ace-ca90-40de-a84b-1445ce1e499b)
```
x=data[["satisfaction_level","last_evaluation","number_project"
x.head()
```
![Screenshot 2024-10-16 152707](https://github.com/user-attachments/assets/3147bea1-d7d0-4e79-b6b6-2e79df8a791c)
```
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
```
![Screenshot 2024-10-16 152848](https://github.com/user-attachments/assets/65417e16-3ca3-4ce2-a52b-e83b2a25b305)
```
dt.predict([[0.5,0.8,9,260,6,0,1,]])
```
![Screenshot 2024-10-16 152952](https://github.com/user-attachments/assets/f52acf0a-9856-4476-89ea-c7fab0515f09)
```
*/
```

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
