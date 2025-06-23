# AI-ML-Internshipimport pandas as pd
# AI & ML Internship - Task 1
### 🔍 Data Cleaning & Preprocessing using Titanic Dataset

This repository contains my first task for the AI & ML Internship, where I perform data cleaning and preprocessing on the Titanic dataset using Python and Jupyter Notebook.

## 📊 Dataset Used
**Titanic Dataset**  
Download link: [Titanic Dataset CSV](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv)

## 📌 Outcome
This task helped me learn:
- Real-world data cleaning
- Preprocessing techniques
- Basic exploratory data analysis (EDA)

code
# load the Titanic dataset 
url = "https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv"
df= pd.read_csv(url)

# display the first few rows of the dataset
print("Initial Dataset:")
print(df.head())

# check for missing values
missing_values = df.isnull().sum()
print("\nMissing Values:")
print(missing_values)

# Drop rows with missing values
df_cleaned = df.dropna()

# Display the cleaned dataset
print("\nCleaned Dataset:")
print(df_cleaned.head())
