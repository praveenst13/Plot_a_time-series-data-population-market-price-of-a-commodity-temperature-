# EXP-1-Plot-a-time-series-data for market price of a commodity
## AIM:
To Write a Program to Plot a timeseries data market price of a commodity 

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Procedure:
   1. import the matplotlib.pyplot and pandas
   2. read the datasets using pandas
   3. calculate the mean for dataset
   4. Plot the data according to need and can be altered monthly, or yearly.
      


## Program:
```
/*
Plot a timeseries data  market price of a commodity 
Developed by: Praveen s
RegisterNumber:  212222240077
*/

import matplotlib.pyplot as plt
import pandas as pd
df=pd.read_csv("Dataset.csv",parse_dates=["Date"],index_col="Date")
df.head()
df["2022-01"]
df["2022-01"].Close.mean()
df["2022-04-01":"2022-07-31"]
df.Close.resample('M').mean()
mean=df.Close.resample('M').mean().plot(kind="bar")
mean=df.Close.resample('Y').mean().plot(kind="bar")
```

## Output:

### df.head()
![img](https://user-images.githubusercontent.com/93427224/261832324-a683d975-99a1-4492-8c49-4dc55e2a97bf.png)


### Mean
![img](https://user-images.githubusercontent.com/93427224/261832330-8ecf6d96-3a31-455a-b79d-06b7186a5e1e.png)

### Monthly Graph
![img](https://user-images.githubusercontent.com/93427224/261832342-6ec20103-4a67-40b8-9eb6-c61b009db030.png)


### Yearly Graph

![img](https://user-images.githubusercontent.com/93427224/261832269-e34d281f-9228-443b-a413-dd7973a20966.png)
## Result:
Thus the program to implement to Plot a timeseries data market price of a commodity is written and verified using python programming.
