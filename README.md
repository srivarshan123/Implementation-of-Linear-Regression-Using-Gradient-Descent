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
import numpy as np
import pandas as pd
import matplotlib.pyplot as py
data.head()
Hours	Scores
0	2.5	21
1	5.1	47
2	3.2	27
3	8.5	75
4	3.5	30
data.isnull().sum()
Hours     0
Scores    0
dtype: int64
x=data.Hours
x.head()
0    2.5
1    5.1
2    3.2
3    8.5
4    3.5
Name: Hours, dtype: float64
y=data.Scores
y.head()
0    21
1    47
2    27
3    75
4    30
Name: Scores, dtype: int64
n=len(x)
m=0
c=0
L=0.01
from typing import ChainMap
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
/*
Program to implement the linear regression using gradient descent.
Developed by: Srivarshan.S
RegisterNumber:  212221040163
*/

## Output:
![linear regression using gradient descent]()


## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
