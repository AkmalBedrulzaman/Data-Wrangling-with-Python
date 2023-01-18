# Data Wrangling with Python at Google Colaboratory by using Used Car Ads Dataset


## 1) Setting up Google Colaboratoy 

#### Load Dataset to Google BigQuery
    go to colab.research.google.com - login with google account - click new notebook - click file - upload to session storage - upload used car ads dataset - rename it
#### Query to Import Pandas
    import pandas as pd
#### Query to Make DataFrame 
    df = pd.read_csv("/content/used_car_ads.csv")
#### Query to Preview Dataset for the First 5 Rows
    df.head()
#### Query to Show Series of manufacture_year Column
    df.manufacturer_year

---
 
## 2) Inspecting Data with Python

#### Query to Preview Dataset for the First 10 Rows
    df.head(10)
#### Query to Show All Available Columns Header
    df.columns
#### Query to Show First Value of maker Column
    df.maker[0]
#### Query to Show First Row and First Column Value
    df.iloc[0, 0]
#### Query to Show First Row at maker Column
    df.loc[0, "maker"]
#### Query to Show All Values at maker Column
    df.loc[:, "maker"]
#### Query to Show First 10 Rows (0,1,2,..,10) at maker and model Column
    df.loc[0:10, ["maker", "model"]] 
#### Query to Show First 10 Rows (0,1,2,..,9) at First 2 Column 
    df.iloc[0:10, :2]
    
#### Query to Give Quick Summary of Numeric Column Variables Within Table (Count,Mean,Std,Min,25%,50%,75%,Max)
    df.describe()
#### Query to Show Each Column and Their Data Types (Float,Object)
    df.info()
#### Query to Know How Many Row and Column
    df.shape
#### Query to Show First 5 Rows at maker Column 
    df.maker.head()
#### Query to Show Quick Summary  at maker Column (Count,Unique,Top,Freq)
    df.maker.describe()
#### Query to Show First 10 Rowa at maker Column
    df.maker.head(10)
#### Query to Show All Unique Value at maker Column
    df.maker.unique()
#### Query to Show How Many Unique Value at maker Column
    df.maker.nunique()
#### Query to Show Values Each maker Row
    df.maker.value_counts()
#### Query to See Maximum Value at mileage Column
    df.mileage.max()
#### Query to  See Minimum Value at mileage Column
    df.mileage.min()
#### Query to See Mean Value at mileage Column
    df.mileage.mean()
#### Query to Show True if Have skoda
    df.maker == "skoda"
#### Query to Show All Table That Only Have skoda at maker Column
    df.loc[df.maker == "skoda"]
#### Query to Show All Table that Have skoda or ford Only
    df.loc[(df.maker == "skoda") | (df.maker == "ford")]
#### Query to Show All Table that Have skoda or ford Only (More clean)
    df[df.maker.isin(["skoda","ford"])]
    
---


##

#### Query to 
