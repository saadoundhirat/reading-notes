# **pandas:**

- ```
        import numpy as np
        import pandas as pd
  ```

- pandas used to handle our data.
- When working with tabular data, such as data stored in spreadsheets or databases, pandas is the right tool for you. pandas will help you to explore, clean, and process your data. In pandas, a data table is called a DataFrame.
- pandas is an open source, BSD-licensed library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming

- Pandas library is one of the most preferred tools for data scientists to do data manipulation and analysis, next to matplotlib for data visualization and NumPy, the fundamental library for scientific computing in Python on which Pandas was built.

- The fast, flexible, and expressive Pandas data structures are designed to make real-world data analysis significantly easier, but this might not be immediately the case for those who are just getting started with it. Exactly because there is so much functionality built into this package that the options are overwhelming.

    ![](https://pandas.pydata.org/pandas-docs/stable/_images/01_table_dataframe.svg)
    
    ![](https://media.geeksforgeeks.org/wp-content/uploads/finallpandas.png)
### **Object creation:**

1. Creating a Series by passing a list of values, letting pandas create a default integer index:

```
    In [3]: s = pd.Series([1, 3, 5, np.nan, 6, 8])

    In [4]: s
    Out[4]: 
    0    1.0
    1    3.0
    2    5.0
    3    NaN
    4    6.0
    5    8.0
    dtype: float64
```

### **Creating a DataFrame:**

```
In [5]: dates = pd.date_range("20130101", periods=6)

In [6]: dates
Out[6]: 
DatetimeIndex(['2013-01-01', '2013-01-02', '2013-01-03', '2013-01-04',
               '2013-01-05', '2013-01-06'],
              dtype='datetime64[ns]', freq='D')

In [7]: df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list("ABCD"))

In [8]: df
Out[8]: 
                   A         B         C         D
2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
2013-01-02  1.212112 -0.173215  0.119209 -1.044236
2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
2013-01-04  0.721555 -0.706771 -1.039575  0.271860
2013-01-05 -0.424972  0.567020  0.276232 -1.087401
2013-01-06 -0.673690  0.113648 -1.478427  0.524988
```

### **Plotting**
- We use the standard convention for referencing the matplotlib API:

```
    In [131]: import matplotlib.pyplot as plt

    In [132]: plt.close("all")
```

```
    In [133]: ts = pd.Series(np.random.randn(1000), index=pd.date_range("1/1/2000", periods=1000))

    In [134]: ts = ts.cumsum()

    In [135]: ts.plot();
```

- On a DataFrame, the plot() method is a convenience to plot all of the columns with labels:
```
In [136]: df = pd.DataFrame(
   .....:     np.random.randn(1000, 4), index=ts.index, columns=["A", "B", "C", "D"]
   .....: )
   .....: 

In [137]: df = df.cumsum()

In [138]: plt.figure();

In [139]: df.plot();

In [140]: plt.legend(loc='best');
```

![](https://pandas.pydata.org/pandas-docs/stable/_images/frame_plot_basic.png)



recourse      | links
------------- | -------------
Pandas | [Link](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)