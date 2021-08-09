# **Linear Regression in Python:**

### **What Is Regression?**

- Regression searches for relationships among variables.

- For example, you can observe several employees of some company and try to understand how their salaries depend on the features, such as experience, level of education, role, city they work in, and so on.

- Typically, you need regression to answer whether and how some phenomenon influences the other or how several variables are related. For example, you can use it to determine if and to what extent the experience or gender impact salaries.

# **Linear Regression:**

Linear regression is probably one of the most important and widely used regression techniques. It’s among the simplest regression methods. One of its main advantages is the ease of interpreting results.


### **Simple Linear Regression**

- Simple or single-variate linear regression is the simplest case of linear regression with a single independent variable, 𝐱 = 𝑥.

![](https://files.realpython.com/media/fig-lin-reg.a506035b654a.png)

### **Implementing Linear Regression in Python:**

- There are several ways in which you can do that, you can do linear regression using numpy, scipy, stats model

- we will use **scikit** learn to perform linear regression.

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Prices.png)

- Scikit-learn is a powerful Python module for machine learning. It contains function for regression, classification, clustering, model selection and dimensionality reduction. Today, I will explore the sklearn.linear_model module which contains “methods intended for regression in which the target value is expected to be a linear combination of the input variables”.


# **Exploring Boston Housing Data Set:**

-  import the required Python libraries into Ipython Notebook.

    ![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Explore-1.png)

- This data set is available in sklearn Python module, so I will access it using scikitlearn. I am going to import Boston data set into Ipython notebook and store it in a variable called boston.

    ![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/sklearn.png)

-The object boston is a dictionary, so you can explore the keys of this dictionary.

    ![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/boston-keys.png)
    ![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/boston-data-shape1.png)

- print the feature names of boston data set.

    ![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/boston-features.png)

- see the description of this data set to know more about it.

    ![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/boston-description.png)

    ![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Attribution.png)

- convert boston.data into a pandas data frame.

    ![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Pandas-DataFrame.png)

## Important functions while fitting a linear regression model are:

1) lm.fit() -> fits a linear model

2) lm.predict() -> Predict Y using the linear model with estimated coefficients

3) lm.score() -> Returns the coefficient of determination (R^2). A measure of how well observed outcomes are replicated by the model, as the proportion of total variation of outcomes explained by the model.

## Residual Plots
- Residual plots are a good way to visualize the errors in your data. If you have done a good job then your data should be randomly scattered around line zero. If you see structure in your data, that means your model is not capturing some thing.

    ![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Residual-plot.png)

## More about Linear Regression type
Simple linear regression 1 dependent variable (interval or ratio), 1 independent variable (interval or ratio or dichotomous)

- Multiple linear regression 1 dependent variable (interval or ratio) , 2+ independent variables (interval or ratio or dichotomous)

- Logistic regression 1 dependent variable (dichotomous), 2+ independent variable(s) (interval or ratio or dichotomous)

- Ordinal regression 1 dependent variable (ordinal), 1+ independent variable(s) (nominal or dichotomous)