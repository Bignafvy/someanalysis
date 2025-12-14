# someanalysis
data analysis of Dataset 
import pandas as pd
import matplotlib.pyplot as plt

# Load dataset
df = pd.read_csv("data.csv")

# Preview data
print(df.head())

# Dataset information
print(df.info())

# Check for missing values
print("\nMissing values:")
print(df.isnull().sum())

# Basic statistics
print("\nDescriptive statistics:")
print(df.describe())

# Handle missing values (example)
df = df.dropna()

# Simple visualization
plt.figure()
df.hist(figsize=(10, 8))
plt.tight_layout()
plt.show()
