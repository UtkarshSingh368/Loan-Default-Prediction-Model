# Loan-Default-Prediction-Model
# 🏦 Loan Default Prediction using Random Forest

## 📌 Problem Statement

Financial institutions often face challenges in identifying potential defaulters when issuing loans. The goal of this project is to build a machine learning model that can predict whether a customer is likely to default on a loan, based on historical data. This predictive capability will help institutions make more informed lending decisions, reduce financial risk, and improve portfolio quality.

---

## 🧪 Methodology

### 1. **Data Upload & Preparation**
- The dataset is uploaded interactively using `google.colab.files`.
- The data is read into a pandas DataFrame and the first few rows are printed for inspection.
- An unnecessary identifier column `LoanID` is dropped if it exists.

### 2. **Encoding Categorical Features**
- All categorical features (object data types) are encoded using `LabelEncoder` from scikit-learn.
- A dictionary of label encoders is stored in case decoding is required later.

### 3. **Feature and Target Separation**
- The target variable is `Default`, which indicates whether a customer has defaulted.
- Features (`X`) are all remaining columns after removing `Default`.

### 4. **Data Sampling (Optional)**
- For faster training and demonstration purposes, a 20% random sample of the full dataset is used.
- This helps reduce computational load during experimentation.

### 5. **Model Training**
- The data is split into training and testing sets (80/20 split).
- A `RandomForestClassifier` is trained using:
  - 100 estimators
  - Maximum tree depth of 10
  - Fixed random state for reproducibility

### 6. **Model Evaluation**
- The trained model is evaluated using the following metrics:
  - Accuracy
  - Precision
  - Recall
- A confusion matrix is also generated and visualized using Seaborn heatmap for a clear understanding of prediction results.

---

## 📊 Results

| Metric      | Score    |
|-------------|----------|
| Accuracy    | *e.g., 0.8421* |
| Precision   | *e.g., 0.7895* |
| Recall      | *e.g., 0.6521* |

> **Note:** The above values are sample outputs. Actual results may vary based on the uploaded dataset.

A confusion matrix heatmap was also generated to visually assess model performance in terms of true positives, false positives, true negatives, and false negatives.

---

## 📎 Requirements

- Python 3.x
- Libraries: `pandas`, `seaborn`, `matplotlib`, `sklearn`, `google.colab`

To run this notebook, simply upload your CSV file with loan data when prompted.

---

## ✅ Conclusion

The model provides a useful starting point for identifying potential defaulters using machine learning. With further tuning and data cleaning, its accuracy and robustness can be improved for real-world applications.
![Screenshot 2025-04-18 151200](https://github.com/user-attachments/assets/b25ea9b5-4906-47d1-82d0-d0570a1843c4)

