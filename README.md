# module_14 - Machine Learning Trading Bot

## An algorithmic trading bot that learns and adapts to new data and evolving markets using machine learning.

---
## Technologies

* Python 3.9

---
## Imports and Dependencies 

* import pandas as pd
* import numpy as np
* from pathlib import Path
* import hvplot.pandas
* import matplotlib.pyplot as plt
* from sklearn import svm
* from sklearn.preprocessing import StandardScaler
* from pandas.tseries.offsets import DateOffset
* from sklearn.metrics import classification_report

---
## Usage

After importing and preparing the data for machine learning use the SVC classifier model is used from SKLearn's support vector machine (SVM) learning method to fit the training data and make predictions based on the testing data. Then a dataframe was created to contain columns for “Predicted” values, “Actual Returns”, and “Strategy Returns.”

The plot of the basecase:
![basecase plot](/Starter_Code/Resources/cumulative_return_plot_baseline.png)

Then the algorithym was tuned to include the calendar year 2016 and the short and long windows were set to 6 and 75, respectively. 
![tuned plot](/Starter_Code/Resources/cumulative_return_plot_Tuned.png)

As shown, decreasing the time period and adjusting the short and long windows produced lower rates of return for both the actual and strategy. 

To improve the Strategy returns, the short and long windows were both cut in half from the baseline windows. For the improved returns, the short window is set to 2 and long set to 50.
![tuned plot](/Starter_Code/Resources/cumulative_return_plot_Tuned2.png)

---
## Contributors

Ryan Svendson
rsvendson@gmail.com