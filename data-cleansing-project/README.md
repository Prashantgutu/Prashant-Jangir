# Data Cleansing Project

This project contains scripts and datasets for data cleansing tasks.
import pandas as pd

# Load the raw data
data = pd.read_csv('data.csv')

# Display basic info
print("Original Data:")
print(data.info())
print(data.head())

# Remove duplicates
data = data.drop_duplicates()

# Fill missing values (forward fill as example)
data = data.fillna(method='ffill')

# Drop columns with too many missing values (threshold: 80%)
threshold = 0.8
data = data.loc[:, data.isnull().mean() < threshold]

# Save the cleaned data

data.to_csv('cleaned_data.csv', index=False)
print("Cleaned data saved to cleaned_data.csv")
id,name,age,score
1,John,25,88
2,Jane,30,92
3,Bob,,85
4,Alice,28,92
2,Jane,30,92
5,Tom,22,
