# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import Important Libraries.
2. Load our Dataset.
3. Checking the information of the dataset.
4. Splitting our data into X and y..
5. Splitting our data into training and testing.
6. Converting text into integer using CountVectorizer().
7. Applying SVM algorithm.
8. Accuracy.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: SYED ADIL BASHA
RegisterNumber:  212221043008

import chardet
file='/content/spam.csv'
with open(file,'rb') as rawdata:
  result=chardet.detect(rawdata.read(100000))
result

import pandas as pd
data=pd.read_csv("/content/spam.csv",encoding='Windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values

y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:
## 1.Result Output:
![ex 9 1](https://github.com/SYEDADILBASHA1/Implementation-of-SVM-For-Spam-Mail-Detection/assets/134796157/e8a923b1-c8e0-4d99-9b7d-4b094fc82897)
## 2.data.head():
![ex 9 2](https://github.com/SYEDADILBASHA1/Implementation-of-SVM-For-Spam-Mail-Detection/assets/134796157/55336b88-6e9f-4d95-aa31-9f99464b5e0c)
## 3.data.info():
![ex 9 3](https://github.com/SYEDADILBASHA1/Implementation-of-SVM-For-Spam-Mail-Detection/assets/134796157/39aa1274-5797-40ab-8ed3-d0061f37ebd9)
## 4.data.isnull().sum()
![ex 9 4](https://github.com/SYEDADILBASHA1/Implementation-of-SVM-For-Spam-Mail-Detection/assets/134796157/b18db1da-7326-44f4-82d8-a0b861e85176)
## 5.Y_prediction value:
![ex 9 5](https://github.com/SYEDADILBASHA1/Implementation-of-SVM-For-Spam-Mail-Detection/assets/134796157/ac9ec0d6-fc2e-4059-8bca-672b8c82b1e3)
## 6.Accuracy value:
![ex 9 6](https://github.com/SYEDADILBASHA1/Implementation-of-SVM-For-Spam-Mail-Detection/assets/134796157/68c6ff1c-4f5b-4d01-8d21-c84725b348bc)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
