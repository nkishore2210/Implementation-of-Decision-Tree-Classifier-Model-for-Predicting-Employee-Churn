# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required packages.
2.Read the data set. 
3.Apply label encoder to the non-numerical column inoreder to convert into numerical values. 
4.Determine training and test data set. 
5.Apply decision tree Classifier and get the values of accuracy and data prediction.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: N.Kishore
RegisterNumber: 212222240049 

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707090/db555cf9-2e00-410b-ad15-75b6c1613d53)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707090/5f8554c1-f2ee-45b6-8884-13df04e1685d)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707090/34734c62-c365-4ad9-a4ec-39c6ec2c2189)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707090/36085f9f-3313-4c98-b9d4-31e17db70216)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707090/4618ff86-838c-4ab1-b6c0-90ef1e446208)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707090/477141e1-1dd8-470c-becb-36580e52902c)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707090/55fba8ce-a272-41d0-a6fe-075c36f8c7b6)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
