# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
## STEP 1
Read the given Data

## STEP 2
Get the information about the data

## STEP 3
Remove the null values from the data

## STEP 4
Save the Clean data to the file

# CODE
Name:O.Shanthan Kumar Reddy
Reg. No: 212220040107

Data_set:
!!!
import numpy as np
import pandas as pd
import io
from google.colab import files
uploaded = files.upload()
dd = pd.read_csv(io.BytesIO(uploaded['Data_set.csv']))
print(dd)
dd.tail()
dd.info()
dd.isnull()
dd.isnull().sum()
#mode
dd['show_name'] = dd['show_name'].fillna(dd['aired_on'].mode()[0])
dd['aired_on'] = dd['aired_on'].fillna(dd['aired_on'].mode()[0])
dd['original_network'] = dd['original_network'].fillna(dd['aired_on'].mode()[0])
dd.head()
#mean
dd['rating'] = dd['rating'].fillna(dd['rating'].mean())
dd['current_overall_rank'] =dd['current_overall_rank'].fillna(dd['current_overall_rank'].mean())
dd.head()
#median
dd['watchers'] = dd['watchers'].fillna(dd['watchers'].median())
dd.head()
dd.info()
dd.isnull().sum()
!!!
# OUPUT
