# SWYNEX Dataset Exploration & Preprocessing

## Internship Task – SWYNEX Technologies

This project focuses on exploring, cleaning, and preprocessing a dataset for machine learning.

## Objective

The objective of this task is to prepare a dataset for machine learning by performing exploratory data analysis, handling missing values, encoding categorical variables, and preparing numerical features.

## Dataset

The Titanic dataset is used for this task.

The dataset contains passenger-related information such as:

- Passenger class
- Age
- Gender
- Number of siblings/spouses
- Number of parents/children
- Fare
- Port of embarkation
- Survival status

## Tasks Performed

### 1. Dataset Exploration
- Dataset dimensions
- Column names
- Data types
- Statistical summary

### 2. Exploratory Data Analysis
- Survival distribution
- Age distribution
- Survival by gender
- Correlation analysis
- Missing-value visualization

### 3. Data Cleaning
- Missing-value analysis
- Removal of the `deck` column due to extensive missing values
- Removal of redundant and derived features

### 4. Train-Test Split
The dataset was divided into training and testing sets using an 80:20 ratio.

### 5. Preprocessing Pipeline

A `ColumnTransformer` based preprocessing pipeline was implemented.

#### Numerical Features
- Median imputation
- Standard scaling

#### Categorical Features
- Most-frequent imputation
- One-hot encoding
- Unknown-category handling

### 6. Data Leakage Prevention

The preprocessing pipeline was fitted only on the training data and subsequently applied to the test data.

This prevents information from the test dataset from influencing the preprocessing process.

### 7. Final Validation

The processed dataset was checked for:

- Missing values
- Numerical feature types
- Consistent training and testing feature structures

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- GitHub

## Repository Contents

| File | Description |
|---|---|
| `Dataset_Exploration_Preprocessing.ipynb` | Complete Python notebook containing exploration and preprocessing |
| `titanic_preprocessed.csv` | Final processed dataset |

## Outcome

The dataset was successfully explored and transformed into a machine-learning-ready format using a reusable preprocessing pipeline.
