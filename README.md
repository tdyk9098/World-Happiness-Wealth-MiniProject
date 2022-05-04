# World-Happiness-Wealth-Plotly-Cufflinks
A quick showcase of basic Plotly and Cufflinks plots- a powerful visualization tool!

Dataset: World Happiness Report (data is included in the repository).

The objective was to showcase the powerful interactive visualization tools of Plotly and Cufflinks by looking at World Happiness and Wealth data.
Descriptive data findings are easy interpreted, while still only scratching the surface of the possible graph types.


# Install:
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
