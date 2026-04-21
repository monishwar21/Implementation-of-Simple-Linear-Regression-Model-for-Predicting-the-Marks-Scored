# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```

Program to implement the simple linear regression model for predicting the marks scored.
Developed by: K  MONISHWAR
RegisterNumber:  212225230188

import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression
X = np.array([1, 2, 3, 4, 5,6]).reshape(-1, 1)
Y = np.array([30, 40, 55, 60, 75,80])
model = LinearRegression()
model.fit(X, Y)
m = model.coef_[0]
b = model.intercept_
print("Slope (m):", m)
print("Intercept (b):", b)
x_input = float(input("Enter hours studied: "))
predicted_marks = model.predict([[x_input]])
print("Predicted Marks:", predicted_marks[0])
Y_pred = model.predict(X)
plt.scatter(X, Y, label="Actual Data")
plt.plot(X, Y_pred, label="Regression Line")
plt.xlabel("Hours Studied")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression")
plt.legend()
plt.show()

```

## Output:
<img width="923" height="537" alt="image" src="https://github.com/user-attachments/assets/9bf738d8-25a2-4719-b5ea-2bc735c060a1" />
<img width="1002" height="741" alt="image" src="https://github.com/user-attachments/assets/a2fd147c-2879-43e3-9bae-763689be00c4" />



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
