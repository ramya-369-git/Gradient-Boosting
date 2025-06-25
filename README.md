# Credit Card Fraud Detection using Gradient Boosting

This project demonstrates the application of **Gradient Boosting** to detect fraudulent transactions in a real-world credit card dataset. Gradient Boosting is a powerful ensemble method that builds models sequentially, optimizing for errors made by previous models.

---

## 📌 Overview

Credit card fraud detection is a critical issue due to the high financial impact of fraudulent transactions. Given the **highly imbalanced** nature of such data (fraud cases are extremely rare), this project applies Gradient Boosting, an ensemble learning technique known for its predictive accuracy and robustness.

---

## 📂 Dataset

- **Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Samples**: 284,807 transactions
- **Features**: 30 (28 anonymized `V` features + `Time` + `Amount`)
- **Target**:
  - `0` = Legitimate transaction
  - `1` = Fraudulent transaction
- **Imbalance**: Only ~0.17% of the data represents fraud.

> ⚠️ The dataset is not included in the repository due to size (≈150 MB). Download it from the Kaggle link above and place it in your working directory.

---

## 🧠 Model: Gradient Boosting Classifier

- **Algorithm**: Gradient Boosting (via `sklearn.ensemble.GradientBoostingClassifier`)
- **Key Features**:
  - Builds models in sequence to minimize errors from previous iterations.
  - Effective on small to medium-sized datasets.
  - Can handle class imbalance with proper parameter tuning or resampling techniques.
- **Workflow**:
  1. Load and preprocess data
  2. Handle imbalance 
  3. Train Gradient Boosting model
  4. Evaluate model performance

---

## 📈 Evaluation Metrics

Because the dataset is imbalanced, we rely on:
- **Accuracy**

These metrics provide a better understanding of how well the model detects fraud without being biased by the overwhelming number of legitimate transactions.

---

## 🛠️ Technologies Used

- Python 3.x
- Jupyter Notebook
- pandas, numpy
- scikit-learn

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ramya-369-git/Gradient-Boosting.git
   cd gradient-boosting-creditcard
