# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee
### Name: Shashin prasad S
### Ref no: 212222230144
## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1.Import pandas
2.Import Decision tree classifier
3.Fit the data in the model
4.Find the accuracy score

## Program:
```
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Shashin prasad s
RegisterNumber:212222230144
```
```
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
x.head()
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred) 
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
```
## Output:
data.head()
![image](https://github.com/Loshini2301/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/150007305/30d5e0dd-3b8e-4a09-a19c-c1fe5cafb341)

data.info()
![image](https://github.com/Loshini2301/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/150007305/fcbca096-a889-4dcc-b90b-ecff666ea9c4)

isnull() and sum()
![image](https://github.com/Loshini2301/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/150007305/872d7256-c134-4b8e-a139-66a2f8df9739)

data.head() for salary
![image](https://github.com/Loshini2301/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/150007305/e4fa7263-7f94-480e-91f5-89677b3cbf07)

MSE value
![image](https://github.com/Loshini2301/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/150007305/b5ed4766-9036-4279-b06a-0aa89d6f9f95)

r2 value
![image](https://github.com/Loshini2301/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/150007305/3941f20a-ef83-43d5-b989-60513a62c039)

data prediction
![image](https://github.com/Loshini2301/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/150007305/2beb5cc3-d7de-4537-a36e-3a9cac3de71a)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
