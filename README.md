# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.

## Equipment’s required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import panda as pd

### Step2
import linear model from sk learn

### Step3
read the csv file

### Step4
find the multivariate regression

### Step5
display the output

Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv('/content/cars (1).csv')
X=df[['Weight','Volume']]
Y=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(X,Y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("predicted CO2 for the corresponding weight and volume",predictedCO2)
```
## Output:
![image](https://github.com/Saravana-kumar369/Multivariate-Linear-Regression/assets/117925254/6e134364-f66f-4267-bb06-f7e488ac0e35)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
