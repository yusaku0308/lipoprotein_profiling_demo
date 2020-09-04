# lipoprotein_profiling_demo
# demonstration
import pandas as pd
import pandas_profiling as pdp

df = pd.read_excel("master_3.xlsx")
profile = pdp.ProfileReport(df)
profile.to_file("master_3.html")

from IPython.display import HTML
HTML(filename='master_3.html')
