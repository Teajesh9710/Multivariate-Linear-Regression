# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas library and linear_model from sklearn using import statement.
<br>

### Step2
Read the given csv file using read_csv()
<br>

### Step3
Create two arrays, indenpendent array x withtwo classes and dependent array y with one class. Find the regression of x and y using linear_model. Linear Regression() method and fit x and y using .fit() method.
<br>

### Step4
Find the coefficients using coef_and intercept using intercept.
<br>

### Step5
Predict the linear regression using regr.predict()method and display the result.
<br>

## Program:
```
#Developed by: TEAJESH R
#Register number: 25009069
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('PredictedCO2 for the corresponding Weight and Volume : ',predictedCO2)

```
## Output:
<img width="678" height="86" alt="image" src="https://github.com/user-attachments/assets/cf033c94-f7a3-4bd5-845b-dd6116bc0fea" />


### Insert your output
<img width="1060" height="495" alt="image" src="https://github.com/user-attachments/assets/a98587ef-d30e-4852-a492-da0fe98b47a6" />

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
