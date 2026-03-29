# EX13
Nikunj Deep Upadhyay
ENTC B1

THEORY-

Data Wrangling (also called data cleaning or preprocessing) is the process of transforming raw, messy data into a clean and structured format suitable for analysis.


Key Concepts Used in Your File
1. Handling Missing Values
isna() → Detect missing values
notna() → Detect non-missing values
sum() → Count missing values
dropna() → Remove missing values
fillna() → Replace missing values

Example:

Replace with constant: fillna(0)
Replace with mean/median: fillna(df.mean())
2. Row-wise and Column-wise Operations
axis=0 → Column-wise
axis=1 → Row-wise
3. Data Cleaning
Replace invalid entries (like " - ") with NaN

Convert columns to numeric using:

pd.to_numeric(errors='coerce')
4. Handling Inconsistent Data

Standardizing text:

df['Department'].str.upper()
5. Date Formatting

Convert string to datetime:

pd.to_datetime()
Purpose of This Experiment
Identify missing data
Clean inconsistent values
Convert data types
Prepare dataset for analysis

ALGORITHM: Data Wrangling Process

Step 1: Import Libraries
Import required libraries:
Pandas
NumPy
Step 2: Create Dataset
Create a DataFrame using sample data.
Step 3: Detect Missing Values
Use:
isna()
isna().sum()
isna().sum(axis=1)
Step 4: Handle Missing Values
Apply methods:
dropna() → Remove missing rows/columns
fillna() → Replace missing values with:
Constant (0)
Mean
Median
Step 5: Replace Invalid Values

Replace symbols like " - " with NaN using:

df.replace("-", np.nan)
Step 6: Convert Data Types

Convert columns to numeric:

pd.to_numeric(errors='coerce')
Step 7: Fill Remaining Missing Values
Replace missing values:
Age → Mean
Marks → Median
Step 8: Standardize Text Data

Convert text to consistent format:

df['Department'].str.upper()
Step 9: Convert Date Format

Convert date column into datetime format:

pd.to_datetime()
Step 10: Final Clean Dataset
Display cleaned dataset ready for analysis.

CONCLUSION-

Data wrangling ensures:

Clean and structured data
Accurate analysis
Better decision-making

If you want, I can convert this into a perfect exam answer format or short viva notes 👍
