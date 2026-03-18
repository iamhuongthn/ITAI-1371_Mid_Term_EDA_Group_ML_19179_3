
# ITAI-1371 Mid Term Project
## Exploratory Data Analysis and Data Preparation
### Group ML_19179_3

## Project overview

This repository contains our ITAI-1371 midterm project using the Kaggle dataset:

**HR Analytics: Job Change of Data Scientists**
https://www.kaggle.com/datasets/arashnic/hr-analytics-job-change-of-data-scientists/data

The goal of this project is to prepare a raw dataset for a future machine learning exercise by following the class requirements:
- split the dataset into 70 percent training and 30 percent testing
- perform EDA only on the training set
- clean missing values
- encode categorical features
- scale numeric features
- normalize skewed numeric data
- engineer new features
- export final clean datasets

## Machine learning problem

This dataset supports a binary classification problem:

> Predict whether a candidate is looking for a job change (`target = 1`) or not (`target = 0`).

A future model would learn patterns from features such as education, training hours, experience, company size, city development index, and company type, then predict whether a candidate is likely to search for a new job.

## Files included for the midterm

- `docs/original_dataset_url.pdf` - document showing the original dataset URL
- `docs/one_page_project_proposal.pdf` - one-page dataset summary and machine learning proposal
- `docs/reflection_journal.pdf` - reflection journal with individual contribution sections
- `notebooks/job_change_of_data_scientists.ipynb` - Jupyter notebook that demonstrates before and after processing
- `data/processed/hr_jobchange_train_clean.csv` - final clean training dataset
- `data/processed/hr_jobchange_test_clean.csv` - final clean testing dataset

## Dataset files

- `data/raw/aug_train.csv` - original raw Kaggle dataset used for this project
- `data/raw/HR Analytics Job - Change of Data Scientists.zip` - original Kaggle zip download kept for reference
- `data/raw/url.txt` - plain text copy of the dataset URL

## Notebook summary

The notebook shows:
1. raw dataset loading
2. 70/30 train-test split
3. training-only EDA
4. missing-value analysis
5. feature engineering
6. normalization and scaling
7. one-hot encoding
8. before-versus-after comparison
9. export of final clean train and test datasets
10. an optional baseline model to show the processed data is machine-learning ready

## Repository structure

```text
ITAI-1371_Mid_Term_EDA_Group_ML_19179_3/
├── README.md
├── requirements.txt
├── prepare_dataset.py
├── data/
│   ├── raw/
│   │   ├── aug_train.csv
│   │   ├── HR Analytics Job - Change of Data Scientists.zip
│   │   └── url.txt
│   └── processed/
│       ├── hr_jobchange_train_clean.csv
│       └── hr_jobchange_test_clean.csv
├── docs/
│   ├── original_dataset_url.pdf
│   ├── one_page_project_proposal.pdf
│   ├── reflection_journal.pdf
└── notebooks/
    └── job_change_of_data_scientists.ipynb
```

## Important notes

- The original raw dataset was not edited manually.
- All cleaning and preprocessing were done in Python code.
- The preprocessing pipeline is fit on the training split only.
- The testing split remains untouched by EDA and is transformed only with the training-fitted pipeline.
- The reflection journal includes individual contribution sections that can be edited further if your instructor wants different wording or a different set of team names.
