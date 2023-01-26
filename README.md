# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Inport pandas as pd and inport linear model from sklean

### Step2
Read the csv file

### Step3
Get the values of 'x' and 'y' variable

### Step4
Create the linear regression model and fit

### Step5
Print the predicted output

## Program:
```
# Program for Multivariate linear regression using the least squares method.
# Developed by:R Manojkarthik
# RegisterNumber:22003728
import pandas as pd
from sklearn import linear_model
data=pd.read_csv("cars.csv")
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
![image](https://user-images.githubusercontent.com/119560395/214843325-5bdf16bf-68b8-4d01-82b8-5fe40ed4e40e.png)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
