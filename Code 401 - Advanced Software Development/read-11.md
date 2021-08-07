# **Readings: Data Analysis:**

## **Jupyter Lab:**

- What is jupyter-lab?
  answer: jupyter lab is a web-based notebook that enables interactive data analysis.
  
- What is jupyter-notebook?
  answer: jupyter notebook is a web-based notebook that enables interactive data analysis.

## **About JupyterLab:**

- is a next-generation web-based user interface for Project Jupyter.

- JupyterLab enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner.

![](https://ipython-books.github.io/pages/chapter03_notebook/06_jupyterlab_files/home.png)

- You can arrange multiple documents and activities side by side in the work area using tabs and splitters. Documents and activities integrate with each other, enabling new workflows for interactive computing, for example:

- Code Consoles provide transient scratchpads for running code interactively
- Kernel-backed documents enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.
- Notebook cell outputs can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.
- Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers.

### **NumPy Tutorial: Data Analysis with Python:**

- NumPy is a commonly used Python data analysis package. By using NumPy, you can speed up your workflow, and interface with other packages in the Python ecosystem, like scikit-learn, that use NumPy under the hood. NumPy was originally developed in the mid 2000s, and arose from an even older package called Numeric. This longevity means that almost every data analysis or machine learning package for Python leverages NumPy in some way

![](https://miro.medium.com/max/831/1*R0wH6D43-rzG7ivvEhSFkA.png)

### **Numpy 2-Dimensional Arrays With NumPy:**

1- we work with multidimensional arrays. We’ll dive into all of the possible types of multidimensional arrays later on, but for now, we’ll focus on 2-dimensional arrays.

2-dimensional array is also known as a matrix, and is something you should be familiar with. In fact, it’s just a different way of thinking about a list of lists. A matrix has rows and columns. By specifying a row number and a column number, we’re able to extract an element from a matrix.

### **Creating A NumPy Array**

- We can create a NumPy array using the numpy.array function. If we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns. Because we want all of the elements in the array to be float elements for easy computation

### Import the numpy package

Pass the list of lists wines into the array function, which converts it into a NumPy array.
Exclude the header row with list slicing.
Specify the keyword argument dtype to make sure each element is converted to a float. We’ll dive more into what the dtype is later on.

```
import csv
with open("winequality-red.csv", 'r') as f:
    wines = list(csv.reader(f, delimiter=";"))
import numpy as np
wines = np.array(wines[1:], dtype=np.float)
```

### **Using NumPy To Read In Files:**

- It’s possible to use NumPy to directly read csv or other files into arrays. We can do this using the numpy.genfromtxt function. We can use it to read in our initial data on red wines.

- In the below code, we:

- Use the genfromtxt function to read in the winequality-red.csv file.
- Specify the keyword argument delimiter=";" so that the fields are parsed properly.
- Specify the keyword argument skip_header=1 so that the header row is skipped.

```
wines = np.genfromtxt("winequality-red.csv", delimiter=";", skip_header=1)
```

recourse      | links
------------- | -------------
Jupyter Lab| [Link](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html)
NumPy| [Link](https://www.dataquest.io/blog/numpy-tutorial-python/)
