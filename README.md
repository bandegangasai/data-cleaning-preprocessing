# Data Cleaning & Preprocessing with Pandas

## Task 03 – RabTech Academy

This project performs data ingestion, cleaning, validation, preprocessing, outlier analysis, and feature engineering on a retail sales dataset using Python and Pandas.

## Objectives

- Load and inspect the raw retail sales dataset
- Identify missing values
- Check duplicate records
- Standardize column names
- Convert columns to appropriate data types
- Handle missing categorical and numerical values
- Validate numeric values
- Perform IQR-based outlier analysis
- Extract date-based features
- Validate the cleaned dataset
- Export the cleaned dataset as CSV

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

## Dataset

The project uses a retail store sales dataset containing transaction-level information such as:

- Transaction ID
- Customer ID
- Category
- Item
- Price Per Unit
- Quantity
- Total Spent
- Payment Method
- Location
- Transaction Date
- Discount Applied

## Data Cleaning

The following preprocessing steps were performed:

1. Loaded the raw CSV dataset.
2. Inspected dataset dimensions, columns, data types, and missing values.
3. Standardized column names.
4. Converted numerical columns to numeric data types.
5. Converted transaction dates to datetime format.
6. Handled missing item values.
7. Handled missing numerical values using median imputation.
8. Handled missing discount values.
9. Checked for negative and zero numeric values.
10. Checked duplicate records.
11. Performed IQR-based outlier analysis.
12. Created date-based features.

## Feature Engineering

The following features were extracted from the transaction date:

- Year
- Month
- Month Name
- Day of Week

## Final Dataset Validation

After cleaning:

- Missing values: 0
- Duplicate rows: 0
- Rows retained: 12,575
- Columns after feature engineering: 15

## Outlier Analysis

IQR analysis identified:

- `price_per_unit`: 0 outliers
- `quantity`: 0 outliers
- `total_spent`: 157 outliers

The identified outliers were analyzed rather than automatically removed because they may represent legitimate high-value transactions.

## Output

The cleaned dataset is available as:

`clean_retail_sales.csv`

The complete preprocessing workflow is documented in:

`Task_03_Data_Cleaning_Preprocessing.ipynb`

## Project Structure

```text
data-cleaning-preprocessing/
│
├── Task_03_Data_Cleaning_Preprocessing.ipynb
├── clean_retail_sales.csv
└── README.md
