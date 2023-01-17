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
#### Query to 
#### Query to 
#### Query to 
#### Query to 
#### Query to 
