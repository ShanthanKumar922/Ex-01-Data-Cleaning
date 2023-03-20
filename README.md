# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
# STEP 1
Read the given Data

# STEP 2
Get the information about the data

# STEP 3
Remove the null values from the data

# STEP 4
Save the Clean data to the file

# CODE
Name : Aakash H
Register Number : 212220040002
'''
/* 
**Data Cleaning - Data_set.csv**
import numpy as np
import pandas as pd
import io
from google.colab import files
uploaded + files.upload()

**Data Cleannig - Loan_data.csv**
data = pd.read_csv("/content/Loan_data.csv")
print(data)
data.head(5)
data.isnull()
data.isnull().sum()
data['Gender'] = data["Gender"].fillna(data['Gender'].mode()[0])
data['Dependents'] = data["Dependents"].fillna(data['Dependents'].mode()[0])
data['Self_Employed'] = data["Self_Employed"].fillna(data['Self_Employed'].mode()[0])
data['Credit_History'] = data["Credit_History"].fillna(data['Credit_History'].mode()[0])
data.head()
data['LoanAmount']=data['LoanAmount'].fillna(data['LoanAmount'].median())
data.head()
data['Loan_Amount_Term']=data['Loan_Amount_Term'].fillna(data['Loan_Amount_Term'].mean())
data.head()
data.info()
data.isnull().sum()
*/
OUPUT
