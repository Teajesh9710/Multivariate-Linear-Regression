# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.
<br>

### Step2
Read the csv file.
<br>

### Step3
Get the value of X and y variables
<br>

### Step4
Create the linear regression model and fit.
<br>

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
<br>

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
predictedCO2 = regr.predict(pd.DataFrame([[3300, 1300]], columns=['Weight', 'Volume']))
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)


```
## Output:
<img width="678" height="86" alt="image" src="https://github.com/user-attachments/assets/18209057-9145-4d1a-9480-1083bbe76a8b" />

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
