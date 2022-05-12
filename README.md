# World-Happiness-Wealth-Plotly-Cufflinks-MiniProject
Exploring world GDP through interactive visualization and a machine learning application: linear regression model that predicts logged GDP through a variety of variables.

Dataset: World Happiness Report (data is included in the repository).

The objective was to showcase the powerful interactive visualization tools of Plotly and Cufflinks by looking at World Happiness and Wealth data.
Descriptive data findings are easy interpreted, while still only scratching the surface of the possible graph types.

The machine learning component is a model that takes in Ladder score, SE of ladder score, upper and lower whisker, social support, life expectancy, freedome to make choices, generosity, perceptions of corruption, and ladder score in dystopia.


# Install:

pip install numpy | conda install numpy

pip install pandas | conda install pandas

pip install matplotlib | conda install matplotlib

pip install seaborn | conda install seaborn

pip install plotly

pip install cufflinks

pip install chart-studio

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

from sklearn.model_selection import train_test_split

from sklearn.linear_model import LinearRegression
