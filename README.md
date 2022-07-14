# Data-cleaning
import pandas as pd 
df=pd.read_csv("/content/loan_data_set.csv") 
df
df.shape
df.isnull().sum()
df.dtypes #Display number of rows and columns
df['Gender'].fillna(df['Gender'].mode()[0], inplace=True) 
df
df.isnull().sum() 
df['Married'].fillna(df['Married'].mode()[0], inplace=True) 
df['Dependents']. fillna(df['Dependents'].mode()[0], inplace=True) 
df['Self_Employed'].fillna(df[ 'Self_Employed'].mode() [0], inplace=True) 
df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean(), inplace=True) 
df['LoanAmount'].fillna(df['LoanAmount'].mean(), inplace=True) 
df['Credit_History'].fillna(df['Credit_History'].mode() 
[0],inplace=True)
df
df["Self_Employed"].replace(to_replace="Yes", value=1, inplace=True) 
df["Self_Employed"].replace(to_replace="No", value=0, inplace=True) 
df
