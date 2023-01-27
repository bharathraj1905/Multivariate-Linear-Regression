# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd

### Step2
Read the csv



### Step3
get the value of

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3.



## Program:
```
# Program for Multivariate linear regression using the least squares method.
# Developed by: b.barathraj
# RegisterNumber:22008848
import pandas as pd
from sklearn import linear_model
data=pd.read_csv("cars1.csv")
x=data[['Weight','Volume']]
y=data['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('coefficient: ',regr.coef_)
print('Intercept: ',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('Predicted CO2 fot the corresponding weight and volume',predictCO2)

```
## Output:
![Multivariate Linear Regression](https://user-images.githubusercontent.com/121490575/215154921-64c1cc5b-23c2-4562-b69f-05cfd854fb51.png)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
