import pandas as pd
df=pd.read_csv("Data_set.csv")
df=pd.read_csv("/content/Loan_data.csv")
print(df)
df.head(10)
df.tail()
df.info()
df.isnull()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['show_name'].mode()[0])
df['rating']=df['rating'].fillna(df['rating'].mean())
df['watchers']=df['watchers'].fillna(df['watchers'].median())
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
df['original_network']=df['original_network'].fillna(df['original_network'].mode()[0])
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].median())
df['Loan_ID']=df['Loan_ID'].fillna(df['Dependents'].mode()[0])
df['Dependents']=df['Dependents'].fillna(df['Dependents'].mode()[0])
df['Education']=df['Education'].fillna(df['Dependents'].mode()[0])
df.head()
df['ApplicantIncome']=df['ApplicantIncome'].fillna(df['ApplicantIncome'].mean())
df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean())
df.head()
df['Credit_History']=df['Credit_History'].fillna(df['Credit_History'].median())
df.head()
df.info()
df.isnull().sum()
```
# OUPUT

## DATA:
![D1](https://user-images.githubusercontent.com/93427345/189853010-ece586db-7278-40ce-bb06-c3daa5124589.PNG)
![D2](https://user-images.githubusercontent.com/93427345/189853155-7123b879-8a57-404c-8425-1dcd18e15079.PNG)

## NON NULL BEFORE:
![D3](https://user-images.githubusercontent.com/93427345/189853227-eac7d433-1ce2-48fe-b5d5-ccdc942217b7.PNG)
![D4](https://user-images.githubusercontent.com/93427345/189853244-77163773-533d-41f6-8fd7-8cf29d196659.PNG)
![D5](https://user-images.githubusercontent.com/93427345/189853268-3be3b328-36a2-460e-ac64-99c007a46b26.PNG)

## MODE:
![D6](https://user-images.githubusercontent.com/93427345/189853307-74a8bb98-8e83-4387-85f9-af7f1450f44c.PNG)

## MEAN:
![D7](https://user-images.githubusercontent.com/93427345/189853343-dcd1ba3c-c326-48a6-aece-385d9182479f.PNG)

## MEDIAN:
![D8](https://user-images.githubusercontent.com/93427345/189853367-176af084-ac3c-4e10-b96c-a0ae21a5ce63.PNG)

## NON NULL AFTER:
![D9](https://user-images.githubusercontent.com/93427345/189853390-627fd2bf-81b5-4c9f-9807-a8100af1e2ee.PNG)
![D10](https://user-images.githubusercontent.com/93427345/189853415-97baa3de-7c06-4c4d-b673-10d9f91fc30a.PNG)

# RESULT

Thus, the given data is read, cleansed and the cleansed data is saved into the file.
