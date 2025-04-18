# Assignment 1 - Statistical Measures

## Overview
This Jupyter Notebook explores various *statistical measures* applied to a dataset using *Python*. It includes key statistical concepts such as central tendency, dispersion, and correlation to analyze the dataset effectively.

## Dataset Information
- The notebook processes a dataset containing multiple numerical and categorical features.
- It applies *statistical analysis* to extract insights from the data.

## Statistical Measures Covered
The following statistical methods are implemented and analyzed in this notebook:
1. Measures of Central Tendency* 
   - Mean  
   - Median  
   - Mode  

2. Measures of Dispersion 
   - Variance  
   - Standard Deviation  
   - Range  
   - Interquartile Range (IQR)  

3. Correlation Analysis  
   - Pearson Correlation  
   - Spearman Correlation  
   - Kendall Correlation  

4. Other Descriptive Statistics  
   - Skewness  
   - Kurtosis
  

# Assignment 2 - EDA and Preprocessing

## Overview
The main objective of this project is to design and implement a robust data preprocessing system that tackles common data challenges such as:

Missing values
Outliers
Inconsistent formatting

By performing effective preprocessing and EDA, we aim to enhance the dataset’s quality and prepare it for machine learning algorithms.

## EDA and Preprocessing Steps Done are :

1. Data Exploration 
   Listed unique values and length of each column.
   Statistical summary of numerical features.
   Renamed columns for consistency and readability.

2. Data Cleaning 
   Identified and treated missing and inappropriate values.
   Replaced age = 0 with NaN.
   Filled NaN with median (numeric) or mode (categorical).
   Removed duplicates.
   Detected outliers using IQR.

3. Data Analysis
   
   Filtered records where age > 40 and salary < 5000.
   Plotted scatter plot of Age vs Salary.
   Counted individuals by location and visualized with bar chart.

4. Data Encoding
   
   Applied Label Encoding for binary categorical columns.
   Applied One-Hot Encoding for multiclass categorical columns.

5. Feature Scaling
   
   Applied StandardScaler and MinMaxScaler on numeric features for ML readiness.


