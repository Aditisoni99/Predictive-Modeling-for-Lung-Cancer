# Predictive-Modeling-for-Lung-Cancer
End-to-end healthcare data science project featuring EDA, preprocessing, and ML models (LogReg, Random Forest, Gradient Boosting). Built to extract insights, evaluate performance, and drive real-world impact in clinical decision-making.

This project applies end-to-end data science methodology to predict lung cancer using patient lifestyle and symptom data. With rigorous preprocessing, modeling, and evaluation, it aims to demonstrate how AI can support clinical decision-making and early diagnosis.

---

## 📊 Dataset Overview

- **Total Samples**: 309
- **Features**: 15 (symptoms, behavior, demographics)
- **Target**: `LUNG_CANCER` (Yes/No)

Key features include:
- Smoking, Yellow Fingers, Anxiety, Peer Pressure
- Symptoms: Coughing, Chest Pain, Wheezing, Fatigue
- Demographics: Gender, Age

---

## 🔍 Exploratory Analysis

- All data columns are complete (no missing values).
- Class imbalance detected — more YES (lung cancer) than NO.
- Visuals and correlation heatmaps indicated strong associations between **chest pain**, **age**, and **swallowing difficulty** with lung cancer.

---

## 🔁 Preprocessing Steps

- Label Encoding for categorical features
- Applied **SMOTE** to balance class distribution
- Train-Test split (80-20)

---

## 🧠 Models Applied

- Logistic Regression
- Decision Tree
- Random Forest ✅ (Top Performer)
- Gradient Boosting

---

## 📈 Evaluation Metrics

**Best Model**: Random Forest

```
Accuracy: 91.4%
Confusion Matrix:
[[ 5  2]
 [ 6 80]]

Classification Report:
Class 0 (No Lung Cancer): Precision=0.45, Recall=0.71, F1=0.56
Class 1 (Lung Cancer):    Precision=0.98, Recall=0.93, F1=0.95
```

---

## 📌 Correlation Insights

| Feature                   | Correlation with Lung Cancer |
|--------------------------|------------------------------|
| AGE                      | +0.91 ✅ Strongest predictor |
| GENDER (Male)            | +0.67                        |
| SWALLOWING DIFFICULTY    | +0.67                        |
| CHEST PAIN               | +0.61                        |
| SMOKING                  | +0.17 (weaker than expected) |

---

## 📊 Confusion Matrix Visualization

A heatmap clearly shows high True Positives (80), meaning the model is effective at identifying lung cancer cases.

---

## 🧠 Statistical Modeling & Recommendations

- Logistic Regression can be expanded with **odds ratios** and **p-values**.
- Explore **SHAP** for feature contribution explanations.
- Perform **survival analysis** if time-series or progression data is added.

---

## ⚙️ Tech Stack

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- imbalanced-learn (SMOTE)

---

## 🚀 Run the Project

1. Clone the repo
2. Install dependencies:
```bash
pip install -r requirements.txt
```
---

