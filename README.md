# Synthetic Student Dropout Dataset

## Project Description

This repository contains a **synthetic dataset** designed to simulate a university student dropout scenario.

The main objective is to support a **Machine Learning classification problem** where the target variable indicates whether a student is likely to **drop out** or **not drop out** during the first academic year.

The dataset was generated in **Python using Google Colab** and includes:

- Student identification variables
- Demographic variables
- Academic variables
- Financial variables
- A binary target variable: `dropout`
- Missing values
- Outliers
- Categorical variables

This dataset is intended for educational and analytical purposes.

---

## Dataset Structure

The dataset contains **500 records** and the following variables:

| Variable | Type | Description | Range / Categories |
|---------|------|-------------|-------------------|
| `student_id` | Categorical | Unique student identifier | CUC-1000 onward |
| `student_name` | Categorical | Synthetic student full name | Generated names |
| `age` | Numerical | Student age | 16 to 30, with outliers up to 60 |
| `gender` | Categorical | Student gender | Male, Female, Other |
| `origin` | Categorical | City or place of origin | Barranquilla, Soledad, Cartagena, Santa Marta, Monteria, Other |
| `high_school_avg` | Numerical | High school average grade | 0 to 100 |
| `admission_score` | Numerical | Admission test score | 0 to 100 |
| `first_cut_grade` | Numerical | First academic cut grade | 0.0 to 5.0 |
| `second_cut_grade` | Numerical | Second academic cut grade | 0.0 to 5.0 |
| `third_cut_grade` | Numerical | Third academic cut grade | 0.0 to 5.0 |
| `first_semester_grade` | Numerical | Final first-semester grade | 0.0 to 5.0, with outliers |
| `socioeconomic_level` | Numerical / Ordinal | Socioeconomic level | 1 to 6 |
| `scholarship` | Categorical | Scholarship status | Yes, No |
| `loan` | Categorical | Loan status | Yes, No |
| `financial_aid` | Categorical | Financial aid status | Yes, No |
| `dropout` | Categorical | Target variable | Yes, No |

---

## University Grading Scale

The academic grades were generated using the **University of the Coast grading system**, which uses a scale from **0.0 to 5.0** in undergraduate programs. The minimum passing grade is **3.0**. :contentReference[oaicite:3]{index=3}

---

## Missing Values

Missing values were intentionally introduced in selected columns to simulate real-world incomplete records.

The following columns may contain null values:
- `gender`
- `origin`
- `high_school_avg`
- `loan`
- `second_cut_grade`

---

## Outliers

Outliers were manually inserted to simulate unusual or extreme observations.

Examples:
- `age` values such as `45`, `50`, `52`, and `60`
- `first_semester_grade` values such as `0.0`, `0.2`, `5.6`, and `6.0`

---

## Files Included

- `student_dropout_dataset.csv`
- `student_dropout_dataset.xlsx`
- `README.md`
- `notebook.ipynb`

---

## Requirements

The dataset was generated using the following Python libraries:

- `numpy`
- `pandas`
- `matplotlib`
- `openpyxl`

---

## How to Use

1. Download the dataset files from this repository.
2. Load the CSV or Excel file into Python, Excel, or any data analysis tool.
3. Use the `dropout` column as the prediction target for classification tasks.

---

## Notes

This is a **synthetic dataset**, meaning it does not come from real students.
It was created only for academic and machine learning practice purposes.