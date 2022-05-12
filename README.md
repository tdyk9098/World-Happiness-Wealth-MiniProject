# World-Happiness-Wealth-Plotly-Cufflinks-MiniProject
Exploring world GDP through interactive visualization and a machine learning application: linear regression model that predicts logged GDP through a variety of variables.

Dataset: World Happiness Report (data is included in the repository).

The objective was to showcase the powerful interactive visualization tools of Plotly and Cufflinks by looking at World Happiness and Wealth data.
Descriptive data findings are easy interpreted, while still only scratching the surface of the possible graph types.

The machine learning component is a model that takes in Ladder score, SE of ladder score, upper and lower whisker, social support, life expectancy, freedom to make choices, generosity, perceptions of corruption, and ladder score in dystopia.

# Observations:

- Life Expectancy and Logged GDP per capita have an R = .859 with a P Val = 1.09e^-44
- Social Support and Logged GDP per capita have an R = .785 with a P Val = 2.05e^-32
- Social Support and Life Expectancy have an R = .723 with a P Val = 2.09e^-25
- Machine Learning Linear Regression Model 1: MLLRM1 is a simple test-train linear regression model that aims to predict logged GDP per capita.
- MLLRM1 takes the following inputs: Ladder score, SE of ladder score, upper and lower whisker of ladder score, social support, life expectancy, freedom to make life choices, generosity, perceptions of corruption, and ladder score in dystopia.
- MLLRM1 had MAE = .402, MSE = .269, RMSE = .519, Relative RMSE = .053, and R2 Score = .775 (ON INITIAL RUN)
- Machine Learning Linear Regression Model 2: MLLRM2 is a simple test-train linear regression model that aims to predict logged GDP per capita.
- MLLRM2 takes the following inputs: Ladder score, social support, life expectancy, freedom to make life choices, generosity, perceptions of corruption, and ladder score in dystopia.
- MLLRM1 had MAE = .461, MSE = .327, RMSE = .572, Relative RMSE = .06, and R2 Score = .748 (ON INITIAL RUN)


# Install:

pip install numpy | conda install numpy

pip install pandas | conda install pandas

pip install matplotlib | conda install matplotlib

pip install seaborn | conda install seaborn

pip install plotly

pip install cufflinks

pip install chart-studio

pip install -U scikit-learn

# Import:
import pandas as pd

import numpy as np

import cufflinks as cf

from plotly.offline import download_plotlyjs, init_notebook_mode, plot, iplot

init_notebook_mode(connected = True)

cf.go_offline()

import chart_studio.plotly as py

import seaborn as sns

import matplotlib.pyplot as plt

import scipy.stats as st

from matplotlib import rcParams

from sklearn.model_selection import train_test_split

from sklearn.linear_model import LinearRegression

from sklearn import metrics
