### DEVELOPED BY : KULASEKARAPANDIAN K
### REGISTER NO : 212222240052
###  Date: 

# Ex.No: 01A PLOT A TIME SERIES DATA
## AIM :
To develop a Python program to plot time series data, such as the market price of a commodity, using historical Ethereum price data.

## ALGORITHM :
1. Import the required packages like pandas and matplotlib.
2. Read the dataset using the pandas library.
3. Calculate the mean for the relevant column in the dataset.
4. Plot the data as required, with options to modify the view monthly or yearly.
5. Display the final graph.
   
## PROGRAM:
```python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

df=pd.read_csv("ETH10M.csv")
print(df)

df = pd.read_csv("ETH15M.csv", parse_dates=["dateTime"], index_col="dateTime")

df.head()

df.tail()

plt.xlabel("DateTime")
plt.ylabel("Closing Price")
plt.title("Ethereum Price Over Time")
plt.plot(df.index, df["close"], label="Closing Price")
plt.legend()
plt.show()
```
## OUTPUT:
![OUTPUT](https://github.com/user-attachments/assets/0337e7be-6f5d-4400-ae03-22ad2e199131)

## RESULT:
Thus, we have successfully created a Python program for plotting the time series of the given data.
