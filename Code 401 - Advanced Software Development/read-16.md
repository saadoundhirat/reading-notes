# **Readings: Machine Learning Intro:**

- Machine learning is a field of computer science that studies the ways in which computers can learn without being explicitly programmed.
- Machine learning is the practice of teaching computers how to learn patterns from data, often for making decisions or predictions.
- Machine learning is a comprehensive approach to solving problems...

- **Topics in machine learning**
- Model - a set of patterns learned from data.
- Algorithm - a specific ML process used to train a model.
- Training data - the dataset from which the algorithm learns the model.
- Test data - a new dataset for reliably evaluating model performance.
- Features - Variables (columns) in the dataset used to train the model.
- Target variable - A specific variable you're trying to predict.
- Observations - Data points (rows) in the dataset.

### **Tasks**

- A task is a specific objective for your algorithms.

### **categories of tasks:**

1.Supervised Learning:

- Supervised learning includes tasks for "labeled" data (i.e. you have a target variable).
- In practice, it's often used as an advanced form of predictive modeling.
- Each observation must be labeled with a "correct answer."
- Only then can you build a predictive model because you must tell the algorithm what's "correct" while training it (hence, "supervising" it).
- Regression is the task for modeling continuous target variables.
- Classification is the task for modeling categorical (a.k.a. "class") target variables.

2.Unsupervised Learning:

- Unsupervised learning includes tasks for "unlabeled" data (i.e. you do not have a target variable).

- In practice, it's often used either as a form of automated data analysis or automated signal extraction.
- Unlabeled data has no predetermined "correct answer."
- You'll allow the algorithm to directly learn patterns from the data (without "supervision").
- Clustering is the most common unsupervised learning task, and it's for finding groups within your data.

![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/Types-of-Machine-Learning-algorithms-1200x675.jpg)

## **The 3 Elements of Great Machine Learning:**

1. human guidance
2. clean, relevant data
3. avoid over fitting

## **The Blueprint:**

1.Exploratory Analysis

- First, "get to know" the data. This step should be quick, efficient, and decisive.

2. Data Cleaning

- Then, clean your data to avoid many common pitfalls. Better data beats fancier algorithms.

3. Feature Engineering

- Next, help your algorithms "focus" on what's important by creating new features.

4. Algorithm Selection

- Choose the best, most appropriate algorithms without wasting your time.

5. Model Training

- Finally, train your models. This step is pretty formulaic once you've done the first 4.

![](https://elitedatascience.com/wp-content/uploads/2018/05/What-Goes-Into-a-Successful-Model.jpg)

#### Exploratory Analysis:**

- Which is just fancy-talk for “getting to know” your data.
- The goal is to get a sense of the data and see if it’s what you expect,doing this upfront helps you save time and avoid wild goose chases

- The purpose of exploratory analysis is to "get to know" the dataset. Doing so upfront will make the rest of the project much smoother, in 3 main ways:

1. You’ll gain valuable hints for Data Cleaning (which can make or break your models).
2. You’ll think of ideas for Feature Engineering (which can take your models from good to great).
3. You’ll get a "feel" for the dataset, which will help you communicate results and deliver greater impact.

#### Data Cleaning

- Data cleaning is the process of fixing or removing incorrect, corrupted, incorrectly formatted, duplicate, or incomplete data within a dataset. When combining multiple data sources, there are many opportunities for data to be duplicated or mislabeled..

- Data cleaning steps :
  Remove Unwanted observations from datasets : This includes duplicate or irrelevant observations.

1. Fix Structural Errors : Structural errors are those that arise during measurement, data transfer, or other types of "poor housekeeping."For instance, you can check for typos or inconsistent capitalization. This is mostly a concern for categorical features, and you can look at your bar plots to check.

2. Filter Unwanted Outliers : Outliers can cause problems with certain types of models. For example, linear regression models are less robust to outliers than decision tree models.In general, if you have a legitimate reason to remove an outlier, it will help your model’s performance.However, outliers are innocent until proven guilty. You should never remove an outlier just because it’s a "big number." That big number could be very informative for your model.

3. Handle Missing Data : Missing data is a deceptively tricky issue in applied machine learning.First, just to be clear, you cannot simply ignore missing values in your dataset. You must handle them in some way for the very practical reason that most algorithms do not accept missing values.

#### Feature Engineering

- Feature engineering is about creating new input features from your existing ones, In general, you can think of data cleaning as a process of subtraction and feature engineering as a process of addition.

- This is often one of the most valuable tasks a data scientist can do to improve model performance, for 3 big reasons:

1. You can isolate and highlight key information, which helps your algorithms "focus" on what’s important.
2. You can bring in your own domain expertise.
3. Most importantly, once you understand the "vocabulary" of feature engineering, you can bring in other people’s domain expertise!

#### Combine Sparse Classes

Sparse classes (in categorical features) are those that have very few total observations. They can be problematic for certain machine learning algorithms, causing models to be overfit.

- There's no formal rule of how many each class needs.
- It also depends on the size of your dataset and the number of other features you have.
- As a rule of thumb, we recommend combining classes until each one has at least ~50 observations. As with any "rule" of thumb, use this as a guideline.


#### Algorithm Selection

- we have 5 very effective machine learning algorithms for regression tasks.

1. Linear Regression is Flawed
2. Regularization in Machine Learning : is a technique used to prevent over fitting by artificially penalizing model coefficients It can discourage large coefficients (by dampening them).
3. Regularized Regression Algos : it has many types such as : Lasso Regression / Ridge Regression / Elastic-Net
4. Decision Tree Algos : Decision trees model data as a "tree" of hierarchical branches. They make branches until they reach "leaves" that represent predictions.
5. Tree Ensembles : Ensembles are machine learning methods for combining predictions from multiple separate models. There are a few different methods for ensembling

---

#### Training the Model

- datasets should be split such that the largest portion is used for training the model, and the remaining smaller portion is used to test the model.
- It is important to mention that models are tested for their ability to predict new, unseen data. Therefore, different data sets should be used for the purpose of testing, as to have reliable models and avoid having overfit models.

#### Hyperparameter

- Tuning "training" the model basically means tuning the hyperparameter
- hyperparameter are different from model parameters, in the fact that they cannot be learned directly from the training data.
- **Model parameters:**
  * learned attributes that define individual models.
- **Hyperparameter**
  * express "higher-level" structural settings for algorithms.

#### Cross-Validation

- a method for getting a reliable estimate of model performance using only your training data.

#### Select Winning Model

Selecting the best performing model using testing datasets, according to performance metrics: - For regression tasks, we recommend Mean Squared Error (MSE) or Mean Absolute Error (MAE). (Lower values are better) - For classification tasks, we recommend Area Under ROC Curve (AUROC). (Higher values are better)



