# 🔐 Password Strength Checker using Machine Learning

A machine learning project that predicts the strength of a password (**Weak / Medium / Strong**) using character-level TF-IDF features and classification models — built and trained entirely with `scikit-learn`.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-yellow)

---

## 📌 Overview

This project builds a text-classification pipeline that analyzes passwords character-by-character and predicts their strength category. It uses **TF-IDF vectorization** to convert passwords into numerical features, then trains and compares two classifiers:

- **Logistic Regression**
- **Gradient Boosting Classifier**

---

## 📂 Dataset

- File: `Password Strength.csv`
- ~670,000 unique passwords collected online
- Each password is labeled with a strength category:
  - `0` → Weak
  - `1` → Medium
  - `2` → Strong
- Labels are rule-based (length, digits, special characters, etc.)

---

## ⚙️ Feature Engineering

Passwords are converted into numerical vectors using a **character-level TF-IDF Vectorizer**, which captures how important each character is within a password — allowing the model to learn patterns like digit usage, special symbols, and character diversity.

---

## 🧠 Model Training & Evaluation

The dataset is split into training and testing sets. Two models are trained and evaluated:

| Model | Notes |
|---|---|
| Logistic Regression | Fast, simple baseline model |
| Gradient Boosting Classifier | Higher accuracy, ensemble-based |

**Test Accuracy (Gradient Boosting): ~93.2%**

Evaluation metrics used: Accuracy, Precision, Recall, F1-score.

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/Checking-Password-Strength-using-Machine-Learning.git
cd Checking-Password-Strength-using-Machine-Learning
```

### 2. Install dependencies
```bash
pip install pandas numpy seaborn scikit-learn jupyter
```

### 3. Run the notebook
```bash
jupyter notebook
```
Open `Checking Password Strength.ipynb` and run all cells.

> ⚠️ Make sure `Password Strength.csv` stays in the same folder as the notebook.

### 4. Test your own password
When prompted at the end of the notebook, enter any password — the model will predict its strength (0 = Weak, 1 = Medium, 2 = Strong).

---

## 🛠️ Tech Stack

- Python
- pandas, numpy
- seaborn (visualization)
- scikit-learn (TF-IDF, Logistic Regression, Gradient Boosting)
- Jupyter Notebook

---

## 📄 License

This project is licensed under the [Apache License 2.0](LICENSE).

---

## 🙏 Acknowledgements

Inspired by the Kaggle dataset on password strength prediction. Thanks to the open-source Python/ML community for the tools used in this project.
