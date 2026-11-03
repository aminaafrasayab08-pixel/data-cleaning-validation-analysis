# data-cleaning-validation-analysis
Data cleaning and validation using python, pandas, matplotlib-house price dataset
# House Price Data Cleaning & Validation

## Project Overview
Cleaned and validated a large-scale real estate dataset with **4600 rows and 18 columns** for a Data Quality Analyst role.

## Tools Used
- Python, Pandas, SQL
- Data Validation: isnull(), filtering
- Data Presentation: Matplotlib, Seaborn
- Excel / Google Sheets concepts

## Steps Performed

### STEP 1: Reading Large-Scale Dataset
Used `pd.read_csv()` to handle CSV with 4600 records.

### STEP 2: Data Validation - Null Check
Used `pd.isnull().sum()` to confirm no null values. (See screenshot in notebook)
This is core requirement: handling large-scale CSV/JSON.

### STEP 3: Investigating Discrepancies Thoroughly
Used `df.describe()` and found invalid entries:
- `price` minimum = 0.0 (Invalid)
- `bedrooms` minimum = 0.0 (Invalid)
Fixed by filtering: `df[df['price'] > 0]`

This matches the job requirement: "investigating thoroughly when discrepancies found"

### STEP 4: Data Presentation
Created histogram using Matplotlib & Seaborn to show distribution of `yr_built`.
This makes data quality issues easy to understand for stakeholders.

## Key Result
- Validated 4600 records
- Found and fixed invalid price entries
- Presented insights with charts
