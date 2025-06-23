# AI-ML-Internshipimport pandas as pd
# AI & ML Internship - Task 1
### 🔍 Data Cleaning & Preprocessing using Titanic Dataset

This repository contains my first task for the AI & ML Internship, where I perform data cleaning and preprocessing on the Titanic dataset using Python and Jupyter Notebook.

---

## 📌 Objective
To clean and prepare raw data for Machine Learning using:
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn

---

## 📊 Dataset Used
**Titanic Dataset**  
Download link: [Titanic Dataset CSV](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv)

---

## ✅ Steps Performed

1. **Import the dataset**
2. **Explore data** – check missing values, data types, basic statistics
3. **Handle missing values** – using median/mode
4. **Drop irrelevant columns** – dropped `Cabin` due to many nulls
5. **Encode categorical variables** – `Sex` (Label encoding), `Embarked` (One-hot encoding)
6. **Normalize numeric features** – `Age` and `Fare` using StandardScaler
7. **Visualize outliers** – used boxplots
8. **Remove outliers** – using Z-score method

---

## 📎 Output Preview
- Cleaned dataset with no missing values
- Encoded and scaled numerical & categorical columns
- Outliers removed

---

## 📁 Files Included
- `Titanic_Data_Cleaning.ipynb` – Jupyter Notebook with full code
- `README.md` – This file

---

## 🤖 Tools Used
- Jupyter Notebook (via Anaconda)
- Python 3.x
- Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn

---

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
