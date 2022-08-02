# Pandas

## Pandas in 10

import numpy and pandas

```py
import numpy as np
import pandas as pd
```

Create an object such as

`s = pd.Series([1, 3, 5, 6, 7])`

Create a DataFrame:

`df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list(ABCD))`

- `df.head()`: view the top rows of the frame
- `df.tail()`: view the bottom rows of the frame
- `df.index()`: display the index
- `df.columns()`: display the columns
- `DataFrame.to_numpy()`: gives a NumPy a representation of the underlying data
- `df.describe()`: shows a summary of your data
- `df.T`: transpose data
- `df.sort_index()`: sort by an axis
- `df.sort_values()`: sort by values

more pandas functions found at [pandas.pydata.org](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

Additional Resources:

[Pandas](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/01_table_oriented.html)
[Pandas for Data Science](https://realpython.com/learning-paths/pandas-data-science/)