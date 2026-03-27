# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Import Pandas as pd and import linear_model fom sklearn

### Step2
<br>Initialize DataFrame df with the data in the csv file

### Step3
<br>Initialize X with "Weight" and "Volume" and y with "Co2"

### Step4
<br>Apply linear regression using regr

### Step5
<br>Print the predicted results

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv(r"C:\Users\acer\Downloads\car (1).csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)
```
## Output:

<img width="719" height="193" alt="image" src="https://github.com/user-attachments/assets/0ee3ff72-cc51-4719-8f42-a7dd126c08c3" />


<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
