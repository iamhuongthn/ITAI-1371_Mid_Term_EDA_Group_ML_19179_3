
# ITAI-1371 Mid Term Project
## Exploratory Data Analysis and Data Preparation
## Group ML_19179_3
Professor Viswanatha Rao  
March 18, 2026  

---

## Project overview

This project focuses on Exploratory Data Analysis (EDA) and data preprocessing using the **HR Analytics Job Change of Data Scientists dataset** from Kaggle.

The goal is to transform raw, inconsistent data into a clean, structured, and machine learning–ready dataset. Instead of building a model, this project emphasizes building a **robust, reproducible data preprocessing pipeline** aligned with real-world data engineering practices.

---

## Dataset

- **Source:** Kaggle  
- **Dataset:** HR Analytics Job Change of Data Scientists  
- **URL:** Included in `/docs/original_dataset_url.pdf`  

The dataset contains both categorical and numerical features such as:
- City
- Gender
- Education level
- Company size and type
- Years of experience
- Last new job
- Training hours  

The target variable indicates whether a candidate is looking for a job change.

---

## Problem Statement

The dataset contains multiple real-world data quality issues:
- Missing values across several features
- Inconsistent formatting (e.g., company size)
- High-cardinality categorical variables
- Skewed numerical distributions
- Different feature scales

The objective is to **prepare this dataset for machine learning** by applying proper preprocessing techniques while avoiding data leakage.

---

## How This Project Satisfies Midterm Requirements

This project strictly follows all midterm guidelines:

- The dataset was sourced from Kaggle and included with a URL reference  
- The dataset was split into **70% training and 30% testing** using Python  
- All exploratory data analysis (EDA) was performed **ONLY on the training dataset**  
- The test dataset remained untouched during EDA to prevent **data leakage**  
- Missing values were handled using:
  - Median imputation (numerical features)
  - Mode imputation (categorical features)  
- Categorical variables were encoded using **one-hot encoding**  
- Numerical features were scaled using **StandardScaler**  
- Skewed features were normalized using **log transformation**  
- Feature engineering was applied:
  - Conversion of ordinal variables to numeric
  - Cleaning company size format
  - Derived features (e.g., training per experience)  
- The final cleaned dataset was exported for both training and testing sets  

This ensures the pipeline is **reproducible, leakage-safe, and aligned with industry best practices**.

---

## Data Processing Pipeline

The preprocessing pipeline includes the following steps:

1. **Train/Test Split**
   - Dataset split into 70% training and 30% testing
   - Test set remains untouched during EDA and preprocessing fitting

2. **Handling Missing Values**
   - Numerical features → Median imputation  
   - Categorical features → Mode imputation  

3. **Encoding Categorical Variables**
   - One-hot encoding applied to all categorical features  
   - Each category converted into binary columns  

4. **Feature Scaling**
   - StandardScaler applied to numerical features  
   - Ensures zero mean and unit variance  

5. **Normalization**
   - Log transformation applied to skewed features  

6. **Feature Engineering**
   - Convert ordinal variables (experience, last new job) to numeric  
   - Clean inconsistent company size values  
   - Create derived features (e.g., training per experience)  

---

## Before vs After Data Processing

The notebook demonstrates the transformation from raw data to clean data:

### Before:
- Missing values across multiple features  
- Inconsistent formats (e.g., company size)  
- Categorical variables not usable by machine learning models  
- Skewed distributions in numerical features  

### After:
- All missing values handled  
- Cleaned and standardized categorical values  
- One-hot encoded feature matrix  
- Scaled and normalized numerical features  
- Additional engineered features  

This transformation makes the dataset **fully ready for machine learning modeling**.

---

## Repository structure

```
ITAI-1371_Mid_Term_EDA_Group_ML_19179_3/
│
├── data/
│   ├── raw/   
│   │   ├── aug_train.csv
│   │   ├── HR Analytics Job - Change of Data Scientists.zip
│   │   └── url.txt              
│   ├── processed/     
│       ├── hr_jobchange_train_clean.csv
│       └── hr_jobchange_test_clean.csv      
│
├── docs/
│   ├── original_dataset_url.pdf
│   ├── one_page_project_proposal.pdf
│   └── reflection_journal.pdf
│
├── notebooks/
│   └── job_change_of_data_scientists.ipynb
│
│
├── README.md
└── requirements.txt
```

---

## Important Notes

- The original dataset is **not modified manually**  
- All preprocessing steps are performed programmatically  
- The pipeline is designed to be **reusable and reproducible**  
- The test dataset is strictly separated to **avoid data leakage**  

---

## Future Work

This dataset is now fully prepared for machine learning tasks such as:
- Logistic Regression  
- Decision Trees  
- Random Forest  
- Gradient Boosting  

---

## Conclusion

This project demonstrates the full lifecycle of data preparation, from raw data to a clean, machine learning–ready dataset. It highlights the importance of proper preprocessing, avoiding data leakage, and building reproducible pipelines that reflect real-world data science practices.
