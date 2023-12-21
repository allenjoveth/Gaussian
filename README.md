# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Use numpy and sys packages
3. Use nested loop through each row and column
4. End the program

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: Allen Joveth P
RegisterNumber: 23009582
import sys
import numpy as np
n=int(input())
matrix=np.zeros((n,n+1))
x=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        matrix[i][j]=int(input())
for i in range(n):
    if matrix[i][j]==0.0:
        sys.exit("Divide by zero error")
    for j in range(i+1,n):
        ratio=matrix[j][i]/matrix[i][i]
        for k in range(n+1):
            matrix[j][k]=matrix[j][k]-ratio*matrix[i][k]
x[n-1]=matrix[n-1][n]/matrix[n-1][n-1]
for i in range(n-2,-1,-1):
    x[i]=matrix[i][n]
    for j in range(i+1,n):
        x[i]=x[i]-matrix[i][j]*x[j]
    x[i]=x[i]/matrix[i][i]
for i in range(n):
    print("X%d = %0.2f" %(i,x[i]),end=" ")
*/
```

## Output:

Gausian Elimination

![Screenshot 2023-12-21 204405](https://github.com/allenjoveth/Gaussian/assets/139422287/c89e04bd-a591-45f3-97fe-4c929755c8c2)

## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

