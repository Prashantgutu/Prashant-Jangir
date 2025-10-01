# Prashant-Jangir[README.md](https://github.com/user-attachments/files/22643788/README.md)
# Hi, I'm Prashant Jangir 👋

**Date of Birth:** 17 May 1997  
**Location:** Eckschanze 8, 13585 Berlin  
**Email:** prashantjangir123@gmail.com  
**Mobile:** +49 163 6439419

## 👨‍💻 Technical Skills
- Excel
- SQL
- Tableau
- Power BI
- Python

## 🤝 Soft Skills
- Team Player
- Analytical Thinking
- Problem Solver

## 🏏 Hobbies
- Playing Cricket
- Watching Sci-fi Movies

## 📂 Projects
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

## 🌐 Social Links
*To be added...*

---

Feel free to connect with me for collaboration or just to say hello!
