# Breast Cancer Prediction Using Machine Learning

## Project Overview

Breast cancer is one of the most commonly diagnosed life-threatening cancers in women worldwide. Early detection significantly improves treatment outcomes and survival rates.

This project investigates which tumor characteristics are most predictive of malignancy using machine learning models applied to diagnostic imaging data.

**Research Question:**  
What tumor features are the most predictive of malignancy in breast cancer using U.S. diagnostic data?

---

## Project Preview

This project analyzes tumor morphology features from the Breast Cancer Wisconsin dataset and applies multiple machine learning models to predict whether tumors are malignant or benign.

Models implemented:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random Forest

Best Model Performance:
- Logistic Regression Accuracy: **98.25%**

---

## Dataset

This project uses the **Breast Cancer Wisconsin (Diagnostic) Dataset** from the UCI Machine Learning Repository.

Dataset characteristics:

- **569 patient samples**
- **31 variables**
- **Binary classification target**
- **No missing values**

Each record represents measurements extracted from digitized images of breast tumor biopsies.

### Feature Groups

The dataset includes three primary feature categories.

**Mean Features**
- Average measurements of tumor cell nuclei such as radius, texture, perimeter, area, and smoothness.

**Worst Features**
- The most abnormal observed value for each measurement.

**Target Variable**

| Value | Meaning |
|------|------|
| 0 | Malignant |
| 1 | Benign |

---

## Methods

Three machine learning models were implemented and compared.

### Logistic Regression

A statistical classification model used to estimate the probability of malignancy based on tumor features.

Results:

- Accuracy: **98.25%**
- AUC: **0.9977**

Important predictive features include:

- Worst concavity
- Worst compactness
- Worst symmetry
- Mean radius

---

### K-Nearest Neighbors (KNN)

A non-parametric algorithm that classifies tumors based on similarity to nearby data points.

Results:

- Accuracy: **97.08%**

Important predictive features include:

- Worst perimeter
- Worst area
- Worst concavity
- Mean radius

---

### Random Forest

An ensemble learning method that combines multiple decision trees to capture nonlinear relationships between tumor features.

Results:

- Accuracy: **94.15%**

---

## Model Performance

| Model | Accuracy |
|------|------|
| Logistic Regression | 98.25% |
| K-Nearest Neighbors | 97.08% |
| Random Forest | 94.15% |

---

## Key Findings

Important insights from the analysis include:

- Tumor size and irregularity are strong predictors of malignancy.
- **"Worst" measurements consistently outperform average measurements.**
- Larger values of radius, perimeter, area, and concavity are strongly associated with malignant tumors.
- Simple imaging-derived features already provide strong predictive signals for diagnostic models.

These findings support the hypothesis that **tumor morphology is a powerful indicator of malignancy.**

---

## Limitations

### Dataset Limitations

- Dataset includes only **morphological imaging features**
- Missing clinical variables such as:
  - age
  - race
  - hormone receptor status (ER/PR)
  - HER2 status

### Methodological Constraints

- Correlation does not imply causation
- Many features are mathematically related (radius, perimeter, area), which introduces redundancy

### Generalizability

- Dataset size is relatively small
- Data originates from a **U.S. population**, which may introduce population bias

---

## Technologies Used

- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook


## Contributors

- Linh  
- Leah  
- Jules  
- Eric  
- Kannasicho  

---

## References

Wolberg, W., Mangasarian, O., Street, N., & Street, W. (1993).  
*Breast Cancer Wisconsin (Diagnostic) Dataset.* UCI Machine Learning Repository.

Pavani Chalasani (2025).  
*Breast Cancer Clinical Presentation.*