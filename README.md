# Titanic Dataset - Data Cleaning & Preprocessing

This project focuses on data cleaning and preprocessing of the Titanic dataset using Python in Google Colab. The objective is to prepare the raw dataset for machine learning models by handling missing values, encoding categorical variables, scaling numerical features, and removing outliers.

## Dataset
- Source: Kaggle Titanic Dataset
- File used: train.csv

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn (StandardScaler)

## Steps Performed

### 1. Load Dataset & Initial Exploration
- Loaded the Titanic dataset (train.csv) into a Pandas DataFrame.
- Explored data types, checked for null values, and viewed sample records.

### 2. Handling Missing Values
- Dropped the 'Cabin' column due to excessive missing values.
- Filled missing 'Age' values using median imputation.
- Filled missing 'Embarked' values using mode imputation.

### 3. Encoding Categorical Variables
- Applied label encoding to 'Sex' (male = 0, female = 1).
- Applied label encoding to 'Embarked' (S = 0, C = 1, Q = 2).
- Dropped 'Name' and 'Ticket' columns as they are not useful for modeling directly.

### 4. Scaling Numerical Features
- Standardized 'Age' and 'Fare' columns using Z-score normalization.
- This ensures both features have a mean of 0 and standard deviation of 1.

### 5. Outlier Detection and Removal
- Visualized outliers in 'Age' and 'Fare' using boxplots.
- Removed outliers using the IQR (Interquartile Range) method.
- Dataset reduced from 891 rows to 718 rows after outlier removal.

## Result
Final cleaned dataset:
- 9 columns
- 718 records
- All missing values handled
- Categorical features encoded numerically
- Numerical features standardized
- Outliers removed

## Folder Structure
