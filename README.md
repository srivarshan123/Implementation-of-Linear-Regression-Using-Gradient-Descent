# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to implement the linear regression using gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import all the necessary libraries.
2. Introduce the variables needed to execute the function.
3. Using for loop apply the concept using formulae.
4.  End the program.

## Program:
'''
/*
Program to implement the linear regression using gradient descent.
Developed by: Srivarshan.S
RegisterNumber:  212221040163
*/
import numpy as np
import pandas as pd
import matplotlib.pyplot as py
data=pd.read_csv("student_scores .csv")
data.head()
data.isnull().sum()
x=data.Hours
x.head()
y=data.Scores
y.head()
n=len(x)
m=0
c=0
L=0.01
loss=[]
for i in range(10000):
  ypred=m*x+c
  MSE=(1/n)*sum((ypred-y)*2)
  dm=(2/n)*sum(x*(ypred-y))
  dc=(2/n)*sum(ypred-y)
  c=c-L*dc
  m=m-L*dc
  loss.append(MSE)
  print(m,c)
  y_pred=m*x+c
  py.scatter(x,y,color="red")
  py.plot(x,y_pred)
  py.xlabel("study hours")
  py.ylabel("scores")
  py.title("study hours vs scores")
  py.plot(loss)
  py.xlabel("iterations")
  py.ylabel("loss")
'''
## Output:
![linear regression using gradient descent](https://github.com/srivarshan123/Implementation-of-Linear-Regression-Using-Gradient-Descent/blob/main/WhatsApp%20Image%202022-05-09%20at%2011.30.25%20AM%20(1).jpeg)
![linear regression using gradient descent](https://github.com/srivarshan123/Implementation-of-Linear-Regression-Using-Gradient-Descent/blob/main/WhatsApp%20Image%202022-05-09%20at%2011.30.25%20AM%20(2).jpeg)
![linear regression using gradient descent](https://github.com/srivarshan123/Implementation-of-Linear-Regression-Using-Gradient-Descent/blob/main/WhatsApp%20Image%202022-05-09%20at%2011.30.25%20AM%20(3).jpeg)
![linear regression using gradient descent](https://github.com/srivarshan123/Implementation-of-Linear-Regression-Using-Gradient-Descent/blob/main/WhatsApp%20Image%202022-05-09%20at%2011.30.25%20AM.jpeg)


## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
