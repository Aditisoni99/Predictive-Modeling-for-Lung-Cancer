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

## Data Visualization
![image](https://github.com/user-attachments/assets/9172cf11-5a59-4d64-94d1-efa9f14164f9)
![image](https://github.com/user-attachments/assets/96f81e00-199b-4120-a051-702b750e3ff5)
![image](https://github.com/user-attachments/assets/da9a983f-a820-454a-9c69-a1cb9fc66d1f)
![image](https://github.com/user-attachments/assets/9fd36f7f-4533-46fd-bca7-a17b85f54159)
![image](https://github.com/user-attachments/assets/b530634c-90db-4b3e-b8fb-82f45f419a49)
![image](https://github.com/user-attachments/assets/e5e95303-d2f6-49c2-a0e0-eb45f89acfb1)

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
![image](https://github.com/user-attachments/assets/d752842a-e588-40eb-9c8f-bb798537ae18)

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

