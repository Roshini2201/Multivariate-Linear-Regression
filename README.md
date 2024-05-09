# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the csv file.

### Step3
Get the value of X and y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 1000kg, and the volume is 1390cm3.

## Step6
Print the predicted output.

## Program:
```
\*
#Multivariate Linear Regression
#Developed by : ROSHINI S
#Register Number : 212223240142
\*
import pandas as pd
from sklearn import linear_model

df=pd.read_csv('/content/cars (1) (1).csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient",regr.coef_)
print("Intercept",regr.intercept_)
print("Amount",regr.predict([[3300,1300]]))
```
## Output:

![Screenshot 2024-05-09 195536](https://github.com/Roshini2201/Multivariate-Linear-Regression/assets/154105318/4ab932ac-1d76-48ba-b3a4-01175aee4674)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
