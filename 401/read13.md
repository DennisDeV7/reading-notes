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

## Things I want to know more about

Machine learning and data science