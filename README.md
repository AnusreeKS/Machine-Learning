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


# Assignment 3 :  Regression

## Overview 
This project explores various regression techniques in supervised machine learning using the California Housing dataset.
The goal is to predict median house values based on features like income, location, and population.

## Processing Steps 

1) Loading and Preprocessing
    Loaded dataset using `fetch_california_housing(). Converted data to a pandas DataFrame.Checked for missing values (none found).Scaled features using `StandardScaler` (important for SVR and Linear Regression)
    Split data into 80% training and 20% testing using `train_test_split`.



2) Models Implemented

| Model                      | Description |
|---------------------------|-------------|
| `LinearRegression`        | Fits a linear model to the data |
| `DecisionTreeRegressor`   | Tree-based model that splits data on feature thresholds |
| `RandomForestRegressor`   | Ensemble of multiple decision trees (bagging) |
| `GradientBoostingRegressor` | Builds trees sequentially to correct errors |
| `SVR` (Support Vector Regressor) | Attempts to fit a regression within a margin; sensitive to feature scaling |

---

3) Evaluation Metrics

    Each model was evaluated using:

         Mean Squared Error (MSE)
         Mean Absolute Error (MAE)
         R² Score (coefficient of determination)



4) Model Comparison Results

      | Model                  | MSE    | MAE    | R² Score |
      |------------------------|--------|--------|----------|
      | Random Forest Regressor| lowest | lowest | highest  |
      | SVR                    | highest| highest| lowest  |


      Best Performer**: `RandomForestRegressor` — High accuracy, low error.
      Worst Performer**: `SVR` — Struggled with scale and complexity of the data.



# Assignment 4 : Classification 

## Overview :
   
   This project applies multiple supervised classification algorithms to the **Breast Cancer Wisconsin** dataset using `scikit-learn`. 
   The objective is to accurately classify tumors as malignant or benign based on various features.

## Processing Steps :

   ###Loaded dataset using `load_breast_cancer()`
      - Converted data to pandas DataFrame
      -  Checked and confirmed no missing values
      -  Applied **StandardScaler** to normalize features (important for SVM and KNN)
      -  Split dataset into **training (80%)** and **testing (20%)** using `train_test_split'


  ###  Classification Models Implemented

      | Algorithm             | Description |
      |----------------------|-------------|
      | Logistic Regression  | Models probabilities using the sigmoid function |
      | Decision Tree        | Recursive tree structure for feature-based splits |
      | Random Forest        | Ensemble of decision trees (bagging) |
      |*Support Vector Machine (SVM)| Maximizes margin between classes |
      | k-Nearest Neighbors (k-NN)| Classifies based on closest neighbors |

Each model was trained on the preprocessed dataset and evaluated using performance metrics.


   ### Evaluation Metrics

      - Accuracy
      - Classification Report (Precision, Recall, F1-score)
      - Confusion Matrix


   ### Model Performance Comparison

      | Model                  | Accuracy Score |
      |------------------------|----------------|
      | Random Forest          | Highest accuracy |
      | Logistic Regression    | High |
      | SVM                    | High |
      | Decision Tree          | Moderate |
      | k-NN                   | Lower (may vary depending on `k`) |


   #### Best Model: Random Forest (balanced, robust performance)
   #### Worst Model: k-NN (performance can vary depending on scaling and `k`)


# Assignment 5 : Clustering

## Overview

This Jupyter Notebook explores unsupervised learning using **KMeans clustering** on a structured dataset, most likely the **Iris dataset**. It demonstrates clustering techniques along with visualization and evaluation strategies.

## Contents

      Loading and Preprocessing: Initial data loading and basic exploration.
      * KMeans Clustering: 
           - Explanation of the KMeans algorithm.
           - Application of KMeans to partition the dataset into clusters.
      * Elbow Method: 
           - Used to determine the optimal number of clusters (`k`) by plotting Within-Cluster-Sum-of-Squares (WCSS).

## Highlights

- Clear explanation of how KMeans works.
- Practical demonstration using real-world structured data.
- Visualizations of clustering results (e.g. scatter plots).
- Use of the Elbow Method to justify choice of `k`.


# Module End Assignment : Car Price Prediction

## Overview : 
   This project is developed for analyzing car price dynamics in the US market using machine learning. It is designed for a Chinese automobile company entering the US market and aims to help management understand which factors significantly impact car pricing.

## Objective :

   To model car prices using regression techniques and identify which features most affect price — enabling better business and design strategies for the US market.

## Steps Performed

1. Data Preprocessing
   - Cleaned and corrected car brand names
   - Converted categorical features to numerical using one-hot encoding
   - Scaled features using `StandardScaler`

2. Model Training
   - Trained 5 regression models:
     - Linear Regression
     - Decision Tree Regressor
     - Random Forest Regressor
     - Gradient Boosting Regressor
     - Support Vector Regressor (SVR)

3. Model Evaluation
   - Compared using:
     - R² Score
     - Mean Squared Error (MSE)
     - Mean Absolute Error (MAE)
   - Visualized predicted vs actual prices

4. Feature Importance
   - Extracted top contributing features using Random Forest

5. Hyperparameter Tuning
   - Performed grid search on Random Forest to improve performance

## Key Metrics

- Best Model: Random Forest Regressor (after tuning)
- Top Features: Engine size, horsepower, curb weight, car width, brand







