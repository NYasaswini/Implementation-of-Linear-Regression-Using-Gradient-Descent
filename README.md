# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to predict the profit of a city using the linear regression model with gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.To implement the linear regression using the standard libraries in the python.

2.Use the .isnull() function to check the empty.

3.Use the default function.

4.pen the head() function.

5.Use the loop function for a linear equation.

6.Predict the value for the y.

7.Print the program.

8.Plot the graph by using scatters keyword.

End the program.

## Program:
```
/*
Program to implement the linear regression using gradient descent.
Developed by:N.Yasaswini
RegisterNumber:212220040095


import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv("/content/student_scores - student_scores.csv")
data.head()
data.isnull().sum()
x=data.Hours
x.head()
y=data.Scores
y.head()
n=len(x)
m=0
c=0
l=0.001
loss=[]
for i in range(10000):
    ypred=m*x+c
    MSE=(1/n)*sum((ypred-y)*2)
    dm=(2/n)*sum(x*(ypred-y))
    dc=(2/n)*sum(ypred-y)
    c=c-l*dc
    m=m-l*dm
    loss.append(MSE)
    #print(m,c)
    ypred=m*x+c
plt.scatter(x,y,color="blue")
plt.plot(x,ypred)
plt.xlabel("study hours")
plt.ylabel("scores")
plt.title("study hour vs scores")
plt.plot(loss)
plt.xlabel("iteration")
plt.ylabel("loss")
*/
```

## Output:

![image](https://github.com/NYasaswini/Implementation-of-Linear-Regression-Using-Gradient-Descent/blob/f5ea0f779b543e84d87fbc8a2be88b00a086fffc/WhatsApp%20Image%202022-10-13%20at%205.56.51%20PM.jpeg)

![image](https://user-images.githubusercontent.com/114219474/195596906-526e2777-fc6a-49a4-a29e-e8396d220363.png)

## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
