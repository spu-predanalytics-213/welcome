# welcome

![https://www.plutora.com/blog/predictive-modeling](predictive_modeling_diagram.png)

## Introduction

Predictive modeling is creating a mathematical model to accurately predict future events based on previous or historical data.

There are many successful use cases of predictive analytics. 

[Forbes magazine](https://www.forbes.com/sites/zinamoukheiber/2014/02/19/ibm-and-epic-apply-predictive-analytics-to-electronic-health-records/) reports that the use of data mining and predictive analytics has helped to identify patients who have been of the greatest risk of developing congestive heart failure. IBM collected 3 years of data pertaining to 350,000 patients, and including measurements on over 200 factors, including things such as blood pressure, weight, and drugs prescribed. Using predictive analytics, IBM was able to identify the 8500 patients most at risk of dying of congestive heart failure within 1 year.

[Dell](https://www.wsj.com/articles/BL-CIOB-1283) was interested in improving the productivity of its sales workforce. It therefore turned to data mining and predictive analytics to analyze its database of potential customers, in order to identify the most likely respondents. Researching the social network activity of potential leads, using LinkedIn and other sites, provided a richer amount of information about the potential customers, thereby allowing Dell to develop more personalized sales pitches to their clients. The number of prospects that needed to be contacted was cut by 50%, leaving only the most promising prospects, leading to a near doubling of the productivity and efficiency of the sales workforce, with a similar increase in
revenue for Dell.

Examples of the types of questions one would like to predict are:

- How many copies will this book sell?
- Will this customer move their business to a different company?
- How much will my house sell for in the current market?
- Does a patient have a specific disease?
- Based on past choices, which movies will interest this viewer?
- Should I sell this stock?
- Which people should we match in our online dating service?
- Is an e-mail spam?
- Will this patient respond to this therapy?

That indicates a desire to know the future, and to act upon this feature. To make a decision, we either have an intuition or we base on an information. Where a human cannot process information at large, a machine can and big companies like Microsoft, Google, WebMM, develop tools that can provide accurate estimations every day.


## Review Terminology

- The terms **sample**, **data point**, **observation**, or **instance** refer to a single, independent unit of data, such as a customer, patient, or compound. The term sample can also refer to a subset of data points, such as the training set sample. The text will clarify the appropriate context when this term is used.
- The **training set** consists of the data used to develop models while the test or validation sets are used solely for evaluating the performance of a final set of candidate models.
- The **predictors**, **independent variables**, **attributes**, or **descriptors** are the data used as input for the prediction equation.
- **Outcome**, **dependent variable**, **target**, **class**, or **response** refer to the outcome event or quantity that is being predicted.
- **Continuous data** have natural, numeric scales. Blood pressure, the cost of an item, or the number of bathrooms are all continuous. In the last case, the counts cannot be a fractional number, but is still treated as continuous data.
- **Categorical data**, otherwise known as nominal, attribute, or discrete data, take on specific values that have no scale. Credit status (“good” or “bad”) or color (“red,”“blue,” etc.) are examples of these data.
- **Model building**, **model training**, and **parameter estimation** all refer to the process of using data to determine values of model equations.

## Tools and Knowledge

### Statistics

Statistics is the science of collecting data and analyzing them to infer proportions (sample) that are representative of the population. In other words, statistics is interpreting data in order to make predictions for the population.

### Machine Learning

[Arthur Samuel](https://ieeexplore.ieee.org/abstract/document/5392560) coined the term `Machine Learning` in 1959 with the definition:

> Computers the ability to learn without being explicitly programmed. ~ Arthur Samuel

As said, nowadays the definition hasn't changed much. It is the study of computer science algorithms that can improve automatically through experience and by the use of data.

Machine learning algorithms are used in a wide variety of applications, such as in medicine, email filtering, speech recognition, and computer vision, where it is difficult or unfeasible to develop conventional algorithms to perform the needed tasks.

### Python

[Python](https://www.python.org/) is a programming language that lets you work quickly and integrate systems more effectively. It is developing to adjust latest changes and constantly growing by the powerful community that supports it. Using [PyPI](https://pypi.org/), any developer can publish and distribute python packages.

``` py
# Python 3: Fibonacci series up to n
def fib(n):
    a, b = 0, 1
    while a < n:
        print(a, end=' ')
        a, b = b, a+b
    print()
fib(1000)
0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 610 987
```

### Numpy, Pandas

Both of these packages are tools for computing and data analysis with python. 

[Numpy](https://numpy.org/) is a N-dimensional array object with lots of functionalites that base itself from linear algebra. Numpy arrays essentially come in two flavors: Vectors and Matrics. Vectors are strictly 1-d array whereas Matrices are 2-d but matrices can have only one row/column.

``` py
import numpy as np
np.array([1, 2, 3])         # Create a rank 1 array
np.arange(15)               # generate an 1-d array from 0 to 14
np.arange(15).reshape(3, 5) # generate array and change dimensions
```

[Pandas](https://pandas.pydata.org/) is a fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.

Pandas provides for many different kinds of data: tabular data, time-series data, arbitrary matrix data with row and column labels, and Any other form of observational/statistical data sets.

``` py
import numpy as np          #importing numpy
import pandas as pd         #importing pandas
arr=np.array([1,3,5,7,9])   #create arr array
s2=pd.Series(arr)           #create pandas series s2
```

Follow this [amazing introductory tutorial ](https://towardsdatascience.com/top-python-libraries-numpy-pandas-8299b567d955)on numpy and pandas modules.

### Visualizations

Data visualization gives crutial understanding of machine learning models and to understand our data well. There are many great packages that can help you with visualization.

- matplotlib
- seaborn
- plotly
- bokeh

And many many more for [scientific visualization in PyPI](https://pypi.org/search/?q=&o=-created&c=Topic+%3A%3A+Scientific%2FEngineering+%3A%3A+Visualization).

## Todo List

<!-- A list of items for student to follow -->

You may receive assignments that uses GitHub's autograding feature using unit testing. This is done through [GitHub Actions](https://docs.github.com/en/actions) and writing [unit tests](https://realpython.com/python-testing/). To get use to how this works, we will make a practice run.

1. Make a python file with name `my_code.py`.
2. Create at least 2 functions for practice.
3. Check out [test_my_code.py](test_my_code.py) file. This file will test your code once you upload to GitHub!
4. Upload to GitHub once you are done.
5. Go to your repository and check `Actions` tab. After every commit you make, GitHub runs `test_my_code.py` file to validate if your code is satisfactory. See example of an output in my [assignment-0-metinsenturk/actions](https://github.com/spu-bigdataanalytics-212/assignment-0-metinsenturk/actions).
6. Click the green button at the top of the repo, and do `Download ZIP`.
7. As a practice, **download your repository** and **upload it to blackboard** as your first assignment!
8. That's it.

## References

- [Applied Predictive Modeling](http://appliedpredictivemodeling.com/) is a book on the practice of modeling when accuracy is the primary goal written by Max Kuhn, Kjell Johnson
- [Descriptive Statistics](https://towardsdatascience.com/descriptive-statistics-f2beeaf7a8df)
- IBM and Epic Apply Predictive Analytics to Electronic Health Records, by Zina
Moukheiber, Forbes magazine, February 19, 2014.
- How Dell Predicts Which Customers Are Most Likely to Buy, by Rachael King, CIO Journal, Wall Street Journal, December 5, 2012.

## Conclusion

<!-- The takeaway of this repository and whats next. -->

That's it! To a wonderful semester, 

Happy coding!
