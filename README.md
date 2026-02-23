
# ITAI-1371 Mid Term Project  
## Exploratory Data Analysis & Data Preparation  
### Group ML_19179_3

---

## 📌 Project Overview

This repository contains the Midterm Project for ITAI-1371.

The objective of this project is to perform:

- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- Feature engineering
- Preparation of a machine learning ready dataset

The selected dataset is from Kaggle:
<TODO>

This project follows proper machine learning workflow standards, including training and testing separation to prevent data leakage.

---

## 🎯 Project Objectives

This project satisfies the following requirements:

- Select a raw dataset from Kaggle
- Split dataset into 70% Training and 30% Testing
- Perform EDA only on training data
- Handle missing values appropriately
- Encode categorical variables
- Scale numeric features
- Apply normalization to skewed distributions
- Perform feature engineering
- Train a baseline classification model
- Export cleaned datasets for future modeling

---

## 📊 Dataset Description

### 🎯 Target Variable 

### 🔢 Numeric Features

### 🔠 Categorical Features

### 🔍 Missing Values

## 🧠 Machine Learning Problem

---

## 🔬 Machine Learning Workflow

1. Data Splitting (70/30)
2. EDA on training data only
3. Missing value handling
4. One-hot encoding
5. Scaling numeric features
6. Normalization (log transformation)
7. Feature engineering
8. Baseline model training

---

## 📂 Repository Structure

ITAI-1371_Mid_Term_EDA_Group_ML_19179_3/

│
├── README.md
├── data/
│   ├── raw/
│   │   └── raw.csv
│   ├── processed/
│   │   ├── train_clean.csv
│   │   └── test_clean.csv
├── notebooks/
│   └── midterm_eda_pipeline.ipynb
├── docs/
│   ├── dataset_proposal.pdf
│   └── detailed_project_report.pdf
└── requirements.txt

---

## ⚠️ Important Notes

- The original dataset remains unchanged.
- All preprocessing steps were executed using Python code.
- The testing dataset was not used during training.
- No data leakage occurred.

---

## 🚀 How to Run

1. Clone the repository
2. Install required packages:

pip install -r requirements.txt

3. Open:
notebooks/midterm_eda_pipeline.ipynb

---

## 📌 Conclusion

This project demonstrates the complete data preparation lifecycle required for supervised machine learning, including responsible preprocessing, feature engineering, and baseline modeling.
