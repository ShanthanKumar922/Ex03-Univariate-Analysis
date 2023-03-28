# Ex03-Univariate-Analysis
# AIM
To perform Univariate EDA on the given data set.

# Explanation
Exploratory data analysis is used to understand the messages within a dataset. This technique involves many iterative processes to ensure that the cleaned data is further sorted to better understand the useful meaning.The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.


# ALGORITHM
## STEP 1
Import the built libraries required to perform EDA and outlier removal.

## STEP 2
Read the given csv file

## STEP 3
Convert the file into a dataframe and get information of the data.

## STEP 4
Return the objects containing counts of unique values using (value_counts()).

## STEP 5
Plot the counts in the form of Histogram or Bar Graph.

## STEP 6
Use seaborn the bar graph comparison of data can be viewed.

## STEP 7
Save the final data set into the file

# CODE
```
/* 
Name : O. Shanthan Kumar Reddy
Register Number : 212220040107
**Univariate EDA - SuperStore.csv**
import pandas as pd
import numpy as np
import seaborn as snb
df = pd.read_csv('/content/SuperStore.csv')
df.head(10)
df.info()
df.describe()
df.dtypes
df.isnull().sum()
df['Postal Code'] = df["Postal Code"].fillna(df['Postal Code'].mode()[0])
df.isnull().sum()
df['Postal Code'].value_counts()
snb.boxplot(x="Sales",data=df)
snb.countplot(x="Sales",data=df)
snb.distplot(df["Sales"])
snb.histplot(x="Sales",data=df)
df.skew()
df.kurtosis()
snb.histplot(x="Postal Code",data=df)
snb.displot(x="Postal Code",data=df)
snb.boxplot(x="Postal Code",data=df)
snb.boxplot(x="Row ID",data=df)
snb.histplot(x="Ship Mode",data=df)
snb.countplot(x="Category",data=df)
*/
```
# OUPUT
## EDA - SuperStore.csv
![EDA](/images/img.png)
## Displaying information about Dataset
![EDA](/images/img2.png)
![EDA](/images/img3.png)
## Finding null values and cleaning it
![EDA](/images/img4.png)
## Value counts of "Postal Code"
![EDA](/images/img5.png)
## Distribution of Data 
![EDA](/images/img8.png)
## Univariate Analysis
![EDA](/images/img6.png)
![EDA](/images/img7.png)
![EDA](/images/img9.png)
![EDA](/images/img10.png)
![EDA](/images/img11.png)

# RESULT
Thus the program to perform EDA on the given data set is successfully executed.
