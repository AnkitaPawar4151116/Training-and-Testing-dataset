# Training-and-Testing-dataset
A basic data preprocessing pipeline implemented in Python using pandas and scikit-learn. Includes encoding, scaling, and splitting steps for preparing a dataset for ML modeling.

# 🧠 Data Preprocessing Project

This project demonstrates how to prepare raw structured data for machine learning models using Python.

## 📁 Dataset
The dataset contains information about individuals, including:
- Name
- Gender
- City
- Education
- Age
- Income
- Purchase decision (Yes/No)

## 🛠️ Preprocessing Steps

The following preprocessing techniques were applied:

1. **Label Encoding**  
   - Applied on binary columns like `Gender` and `Purchased`.

2. **Ordinal Encoding**  
   - Used for the `Education` column with logical order:
     `Highschool < Graduate < Postgraduate`

3. **One-Hot Encoding**  
   - Performed on the `City` and `Name` columns to handle nominal categorical data.

4. **Feature Scaling**  
   - Used `StandardScaler` to normalize `Age` and `Income` columns.

5. **Train-Test Split**  
   - Data was split using `train_test_split()` from `sklearn` with a test size of 40%.

## 📂 Files Included

- `Train_Test.ipynb` – Jupyter Notebook containing full preprocessing code.
- `mock_customer_data.csv` – Sample dataset used in the notebook.

## 🧪 Requirements

Install the following libraries before running the notebook:
```bash
pip install pandas scikit-learn
