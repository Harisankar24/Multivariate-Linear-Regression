# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
```
1.Import libraries and load data
2.Select features and target variable
3.Initialize and train the model
4.Display model parameters
5.Predict CO2 emission
```
## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('coefficients:',regr.coef_)
print('intercept:',regr.intercept_)
predictedCO2=regr.predict([[2300,1300]])
print('predicted CO2 for the corresponding weight and volume',predictedCO2)





```
## Output:

![Screenshot 2025-04-30 114200](https://github.com/user-attachments/assets/837aef16-a522-481b-9b83-1d7ebdcd350e)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
