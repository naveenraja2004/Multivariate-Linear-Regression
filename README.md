# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import panda module as pd

### Step2
Import linear model from sklearn

### Step3
Read the file cars.csv

### Step4
Assign the values for x and y as required

### Step5
Create the linearRegression model and predict the output

## Program:
```
'''
Programmed by: Naveen Raja N.R
Register number: 212222230093
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))





```
## Output:


![WhatsApp Image 2023-06-11 at 16 06 44](https://github.com/naveenraja2004/Multivariate-Linear-Regression/assets/118707204/733493ed-89ab-40f6-abf5-64f355210a17)




## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
