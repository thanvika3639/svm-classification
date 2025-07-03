# svm-classification

# 📘 SVM Classification on Breast Cancer Dataset

## 🧠 Objective

This project demonstrates how to perform *binary classification* using *Support Vector Machines (SVM)* with both *Linear* and *RBF kernels* on the *Breast Cancer Wisconsin dataset*. It includes preprocessing, visualization, hyperparameter tuning, and model evaluation.

---

## 🗂 Dataset

- *Source*: Breast Cancer Wisconsin (Diagnostic) Dataset
- *Format*: CSV file
- *Target Column*: diagnosis (M = Malignant, B = Benign)
- *Features*: 30 numeric medical measurements (e.g., radius, texture, area, etc.)

## 🔧 Tools and Libraries Used

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Scikit-learn


## 🪜 Workflow Overview

### ✅ 1. Load and Prepare Data
- Read dataset from CSV
- Drop unnecessary columns like id
- Encode diagnosis (M → 1, B → 0)
- Split into features X and target y
- Standardize features using StandardScaler

### ✅ 2. Train SVM Models
- SVM with *linear kernel*
- SVM with *RBF (Radial Basis Function) kernel*

### ✅ 3. Visualize Decision Boundary
- Use *PCA* to reduce data to 2 dimensions
- Plot SVM decision boundary on 2D PCA-projected space

### ✅ 4. Tune Hyperparameters
- Perform grid search using GridSearchCV with 5-fold cross-validation
- Parameters tuned:
  - C: Regularization parameter
  - gamma: RBF kernel coefficient

### ✅ 5. Evaluate Performance
- Use:
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-score, Accuracy)

## 📊 Outputs

- Decision boundary plots (after PCA reduction)
- Best hyperparameters from GridSearchCV
- Classification reports for both SVM models
- Confusion matrices for test data

