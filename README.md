# KEI
## Air Pollution Analysis and Prediction

import os
for dirname, _, filenames in os.walk('/kaggle/input'):
    for filename in filenames:
        print(os.path.join(dirname, filename))

import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
import geopandas as gpd
import geoplot

df = pd.read_csv("/kaggle/input/india-air-quality-data/data.csv", encoding = "ISO-8859-1")
df.head()
