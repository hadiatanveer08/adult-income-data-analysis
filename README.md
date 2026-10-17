# adult-income-data-analysis
# Adult Income Data Analysis and Preprocessing

## Project Overview
This project focuses on exploratory data analysis (EDA), data cleaning, feature engineering, and data preprocessing using the Adult Income dataset. The purpose is to prepare raw data for future machine learning tasks.

## Dataset Information
- **Dataset:** Adult Income (Census Income) Dataset
- **Source:** UCI Machine Learning Repository
- **Rows:** Approximately 32,561 before cleaning
- **Target column:** `income`
- **Target classes:** `<=50K` and `>50K`
- **Dataset link:** https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data

The dataset contains numerical and categorical features related to individuals' demographic information, education, employment, and income.

## Project Steps
1. Load the dataset and inspect its structure.
2. Perform exploratory data analysis using summary statistics and visualizations.
3. Identify and remove duplicate records.
4. Examine missing values and handle them during preprocessing.
5. Remove selected unnecessary or redundant columns.
6. Create new features, including `capital_total` and `is_married`.
7. Separate the features (`X`) from the target (`y`).
8. Split the data into training and testing sets using an 80/20 ratio.
9. Impute missing values, scale numerical features, and encode categorical features.

## Data Preprocessing
- Duplicate rows are removed.
- The `fnlwgt` and `education` columns are dropped for this assignment.
- Missing numerical values are handled using median imputation.
- Missing categorical values are handled using most-frequent imputation.
- Numerical features are standardized using `StandardScaler`.
- Categorical features are encoded using `OneHotEncoder`.
- Preprocessing is fitted on the training data only to prevent data leakage.

## Final Results
After preprocessing, the training feature matrix contains **26,029 rows and 90 columns**, while the testing feature matrix contains **6,508 rows and 90 columns**. The final feature matrices contain no missing numerical values.

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## How to Run
1. Open the notebook in Google Colab.
2. Run the notebook cells from top to bottom.
3. The notebook downloads the dataset from the UCI Machine Learning Repository.

## Author
Student project for data preparation and preprocessing.
