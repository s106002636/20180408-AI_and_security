import numpy as np
import pandas as pd
from pandas import Series, DataFrame

df = pd.read_clipboard()
-->https://pandas.pydata.org/pandas-docs/stable/io.html

# 轉成CSV
df.to_csv('df_io.csv',index=False)

# 轉成json
df_json = df.to_json()

