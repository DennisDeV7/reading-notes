# Data Analysis

## Jupyter Lab

[jupyterlab.com](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html)

JupyterLab enables the user to work with notebooks, text editors, terminals, and custom components on the internet. Jupyter works with most file formats. All image formats are supported as well. Jupyter notebooks allows markdown syntax to create the notebook page.

## Numpy Tutorial

[dataquest.com](https://www.dataquest.io/blog/numpy-tutorial-python/)

NumPy is a data analysis package.

It can be used with different data types for example, csv. Accessing csv data requires the csv libarary. You can access the library with the simple line: `import csv` and open a csv file as you would any other file in Python: `with open('example.csv', 'r') as f:`

In order to use the numpy library: `import numpy as np`
example:

```py
import csv
with open("winequality-red.csv", 'r') as f:
    wines = list(csv.reader(f, delimiter=";"))
import numpy as np
wines = np.array(wines[1:], dtype=np.float)
```

NumPy can automatically convert data from a csv file into an array of floated numbers instead of text using the function `genfromtxt`

example: `wines = np.genfromtxt("winequality-red.csv", delimiter=";", skip_header=1)`

## Things I want to know more about

Working with NumPy and how to best use it and potentially make graphs and so forth with the data.