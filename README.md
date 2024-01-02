# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1:
Import pandas as pd.
<br>

### Step 2:
Read the csv file.
<br>
### Step 3:
Get the value of X and y variables.
<br>
### Step 4:
Create the linear regression model and fit.
<br>
### Step 5:
Predict the CO2 emission of a car where the weight is 3300kg, and the volume is 1300cm3.
<br>

## Program:
```
#Developed by: Priyadharshini.P
#Registration no: 23013604

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('cars.csv')
a=df[['Weight', 'Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("coefficient",regr.coef_)
print("Intercept:", regr.intercept_)
print("Amount:", regr.predict([[3300,1300]]))

```
## Output:
![Screenshot 2024-01-02 155258](https://github.com/priyadharshini210/Multivariate-Linear-Regression/assets/148514638/861d4f66-f5f8-404a-9d88-a3208adec932)
<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
