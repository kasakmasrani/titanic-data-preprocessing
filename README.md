# titanic-data-preprocessing
# Titanic Data Cleaning & Preprocessing

## Overview
This repository contains a complete data preprocessing pipeline applied to the Titanic dataset as part of the AI & ML Internship - Task 1. The goal is to prepare raw data for machine learning by applying essential data cleaning steps.

---

## Objectives
- Handle missing values efficiently
- Encode categorical variables
- Normalize numerical features
- Detect and remove outliers
- Export a clean dataset ready for modeling

---

## Dataset
- **Source:** [Kaggle Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)
- **File Used:** `titanic.csv`

---

## Tools & Libraries
- Python 3
- Pandas
- NumPy
- Seaborn & Matplotlib (for visualization)
- Scikit-learn (for preprocessing)

---

## Preprocessing Steps
1. **Data Inspection**  
   - Shape, data types, null values, and summary statistics.

2. **Handling Missing Data**  
   - `Age`: Imputed with median  
   - `Embarked`: Imputed with mode  

3. **Encoding Categorical Variables**  
   - `Sex` and `Embarked` encoded using One-Hot Encoding (with `drop_first=True` to avoid multicollinearity).

4. **Feature Scaling**  
   - `Age` and `Fare` scaled using `StandardScaler`.

5. **Outlier Removal**  
   - Outliers in `Fare` detected and removed using the IQR method.

6. **Exporting**  
   - Cleaned dataset saved as `titanic_cleaned.csv`.

---

## Folder Structure
titanic_preprocessing/
│
├── titanic.csv # Original dataset
├── titanic_cleaned.csv # Final cleaned data
├── titanic_cleaning.ipynb # Jupyter Notebook with all steps
└── README.md # This file


---

## How to Run
1. Clone this repository
2. Install requirements (`pip install pandas numpy matplotlib seaborn scikit-learn`)
3. Open `titanic_cleaning.ipynb` in Jupyter Notebook
4. Run all cells sequentially

---

## Outcomes
- Cleaned and preprocessed dataset ready for ML modeling
- Improved understanding of real-world data wrangling

---

## Author
Kasak Masrani | B.E. Computer Engineering Student  
AI & ML Internship Task | May 2025
