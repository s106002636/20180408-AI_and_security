import numpy as np

import pandas as pd

from pandas import Series,DataFrame

##### 呼叫並啟動瀏覽器

link = 'https://www.tiobe.com/tiobe-index/'

import webbrowser

webbrowser.open(link)

##### 貼上語法並暫不執行，在至數據反白複製後再執行

df = pd.read_clipboard()

df.Ratings (帶入Ratings list)

df.columns (帶入df欄位名稱)

" 帶入Programming Language及Oct 2017 "

df_new = DataFrame(df, columns=['Programming Language','Oct 2017'])  



df_new['Oct 2018'] = Series([100,200], index=[2,3]) 
