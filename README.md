# AI-ML-Internshipimport pandas as pd
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
