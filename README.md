# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import required packages and read the data file.
2.Use LabelEncoder to convert categorical data into numerical data.
3.Split data into testing data and training data.
4.Apply Decision Tree Regressor.
5.Calculate mean squared error and R2.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: M Sanjay
RegisterNumber:  212222240090
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.head()
data.isnull()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:
![Screenshot 2023-05-17 104323](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119830477/e393e213-4a69-4eb0-9a19-46e28d7b524f)

![Screenshot 2023-05-17 104332](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119830477/dc8fcc34-f9a2-4a19-b98b-42e90ef165da)

![Screenshot 2023-05-17 104339](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119830477/8e12bbfb-15bb-4ef1-b638-c7ee50135c6c)

![Screenshot 2023-05-17 104347](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119830477/6a33c69d-2f4c-401b-9e78-5c142b00ead8)

![Screenshot 2023-05-17 104354](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119830477/6570517a-7068-44f8-8c68-b29c8f319fff)

![Screenshot 2023-05-17 104503](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119830477/4abf5eec-1e42-4ea1-a2c4-b28e73826ff3)

![Screenshot 2023-05-17 104511](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119830477/ddeac5b4-7d57-47ea-aca6-4cb72cde2257)

![Screenshot 2023-05-17 104518](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119830477/b27cbc1d-3f2c-4a10-83fa-ed791655bc07)




## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
