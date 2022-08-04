# Linear Regression

## Running Linear Regression

[crayondata.com](https://www.crayondata.com/how-to-run-linear-regression-in-python-scikit-learn/)

Linear Regression is a linear approach for modelling the relationship between a scalar response and one or more explanatory variables. [Wikipedia](https://en.wikipedia.org/wiki/Linear_regression)

There are many ways to model linear regresssion such as numpy, scipy, and sckit learn.

Sckit-learn is a library for machine learning and contains functions for regression and many others.

step 1: import necessary Python libraries

```py
import numpy as np
import pandas as pd
import scipy.stats as stats
import matplotlib.pyplot as plt
imort sklearn
```

If the data set is available in scikit learn then:

```py
from sklearn.datasets import data_file
variable = data_file()
```

```py
from sklearn.linear_model import LinearRegression
```

functions to use:

- .keys()
- .feature_names
- .DESCR
- .data
- .target
- .drop()

Regression function:

b = predicted weights\
x = independent variables

`𝑓(𝐱) = 𝑏₀ + 𝑏₁𝑥₁ + ⋯ + 𝑏ᵣ𝑥ᵣ`

Sum of Squared Residuals(SSR)

`SSR = Σᵢ(𝑦ᵢ - 𝑓(𝐱ᵢ))²`

## Class

`df_salary = pd.read_csv("/kaggle/input/salary/Salary.csv")`
df_salary

```py
# plot data
import matplotlib.pyplot as plt

years_experience = df_salary.YearsExperience.values
salary = df_salary.["Salary"].values
plt.scatter(years_experiences, salary)
plt.show()
```

Now we need to convert data into a form that scikitlearn can read

```py
from sklearn.linear_model import LinearRegression

# Create a column vector
# .reshape(num_of_rows, num_of_columns)
years_experience_vector = years_experience_values.reshape(-1,1)
years_experience_vector
```

Make the model

```py
model = LinearRegression().fit(years_experience_vector, salary)

# make predictions
prediction = model.predict(years_experience_vector)
plt.scatter(years_experiences, salary)
plt.plot(years_experience_values, prediction, color="red")
plt.show()
# 
```

```py
num_years = 2
salary_predict = model.predict([[num_years]])[0]
print(f"After {num_years} years your salary is predicted to be ${int(salary_predict)}")
```

How can you test how accurate the model was?

### Train Test Split

```py
from skleanr.model_selection import train_test_split

# Train the model
x_train, x_test, y_train, y_test = train_test_split(years_experience_vector, salary, train_size=.8, test_size=.2)

print(f"X_train shape {x_train.shape}")
print(f"y_train shape {y_train.shape}")
print(f"X_train shape {x_test.shape}")
print(f"y_train shape {y_test.shape}")
```

plot the training data

```py
plt.scatter(x_train, y_train, color='red')
plt.xlabel('Years of experience')
plt.ylabel('Salary in Dollars')
plt.title('Training data')
plt.show()
```

plot testing data

```py
plt.scatter(x_test, y_test, color='blue')
plt.xlabel('Years of experience')
plt.ylabel('Salary in Dollars')
plt.title('Training data')
plt.show()
```

```py
lm = LinearRegression()
lm.fit(x_train, y_train)
y_predict = lm.predict(x_test)

print(f"Train accuracy {round(lm.score(x_train,y_train)*100,2)} %")
```

## Things I want to know more about

Machine learning and data science