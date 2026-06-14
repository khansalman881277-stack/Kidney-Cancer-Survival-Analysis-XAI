# 🧬 Enhancing Clear-Cell Renal Cell Carcinoma Survival Prediction Using Explainable Machine Learning

Achieving **90.48% accuracy** on the external E-MTAB-1980 dataset and **85.05% accuracy** on TCGA-KIRC using advanced Machine Learning, Ensemble Learning, and Explainable AI (SHAP & LIME).

---

# 📌 Project Overview

Clear-Cell Renal Cell Carcinoma (ccRCC) is the most common subtype of kidney cancer, accounting for approximately 75–80% of all renal cancer cases.

Traditional clinical staging systems such as TNM, Fuhrman Grade, and UISS often fail to capture the complex molecular mechanisms responsible for disease progression.

This project introduces an **Explainable Machine Learning Framework** that combines:

- Multiple Machine Learning Models
- Ensemble Learning Techniques
- SHAP Explainability
- LIME Explainability
- External Dataset Validation

to improve survival prediction accuracy while maintaining clinical interpretability.

---

# 📊 Results Summary

| Metric | Value |
|----------|----------|
| ✅ Best Accuracy (TCGA-KIRC) | **85.05%** |
| ✅ Best Accuracy (E-MTAB-1980) | **90.48%** |
| ✅ Best Model | **XGBoost** |
| ✅ Ensemble Accuracy | **85.71%** |
| ✅ Datasets Used | **2** |
| ✅ Total Patients | **632** |
| ✅ Explainability Methods | **SHAP + LIME** |
| ✅ Machine Learning Models | **6** |

---

# 🎯 Project Objectives

### Objective 1
Improve survival prediction accuracy using machine learning and ensemble learning techniques.

### Objective 2
Provide transparent and interpretable predictions for healthcare professionals using Explainable AI.

---

# 🗂️ Datasets

## TCGA-KIRC

| Property | Value |
|-----------|-----------|
| Patients | 531 |
| Features | 22 |
| Data Type | RNA-Seq + Clinical Data |
| Purpose | Training & Internal Validation |

---

## E-MTAB-1980

| Property | Value |
|-----------|-----------|
| Patients | 101 |
| Features | 18 |
| Data Type | Microarray + Clinical Data |
| Purpose | External Validation |

---

# ⚙️ Data Preprocessing

The following preprocessing pipeline was applied:

- Missing Value Detection
- Median Imputation
- Feature Selection
- Correlation Analysis
- Categorical Encoding
- Feature Scaling
- Train/Test Split (80/20)

---

# 🤖 Machine Learning Models

Six Machine Learning models were implemented:

| Model | Type |
|---------|---------|
| Random Forest | Bagging Ensemble |
| Gradient Boosting | Boosting Ensemble |
| Logistic Regression | Linear Model |
| Support Vector Machine | Margin-Based |
| Multi-Layer Perceptron | Neural Network |
| XGBoost | Gradient Boosting |

---

# 🔥 Ensemble Learning

Three ensemble techniques were evaluated:

## Voting Ensemble
Combines probability outputs of all base models.

## Stacking Ensemble
Uses predictions from base models as input to a Logistic Regression meta-model.

## Averaging Ensemble
Computes average predictions across all models.

---

# 🏆 Model Performance

## TCGA-KIRC Results

| Model | Accuracy |
|---------|---------|
| Logistic Regression | 80.37% |
| SVM | 82.24% |
| Random Forest | 82.24% |
| Gradient Boosting | 83.18% |
| MLP | 83.18% |
| 🥇 XGBoost | **85.05%** |

---

## E-MTAB-1980 Results

| Model | Accuracy |
|---------|---------|
| Logistic Regression | 66.67% |
| SVM | 71.43% |
| Gradient Boosting | 74.19% |
| MLP | 76.19% |
| Random Forest | 85.71% |
| 🥇 XGBoost | **90.48%** |

---

# 🧠 Explainable AI (XAI)

To eliminate the "black-box" problem in healthcare AI, two explainability techniques were integrated.

## SHAP

Provides:

- Global Feature Importance
- Local Patient Explanations
- Waterfall Plots
- Summary Plots

### Top SHAP Features

1. Observation Period
2. Metastases During Observation
3. CDCA3
4. ANAPC5
5. ATP13A1
6. BRD9
7. MC1R
8. CCDC137
9. Age
10. IL20RB

---

## LIME

Provides patient-level explanations by identifying feature contributions toward:

- Alive Prediction
- Dead Prediction

This allows clinicians to understand why a patient was classified into a particular survival group.

---

# 📈 Key Findings

✅ XGBoost achieved the highest performance across both datasets.

✅ Ensemble models produced more balanced predictions.

✅ SHAP and LIME successfully explained model decisions.

✅ Observation Period was the most influential survival predictor.

✅ Top biological markers included:

- CDCA3
- ANAPC5
- ATP13A1
- BRD9

✅ Consistent feature rankings across TCGA and E-MTAB validated biological relevance.

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- SHAP
- LIME
- Matplotlib
- Seaborn
- Google Colab

---

# 📂 Project Structure

```text
Kidney-Cancer-Survival-Analysis-XAI
│
├── data
├── notebooks
├── models
├── results
├── figures
├── src
│   ├── preprocessing.py
│   ├── training.py
│   ├── evaluation.py
│   └── explainability.py
│
├── requirements.txt
├── README.md
└── LICENSE
```

# 🚀 Installation

```bash
git clone https://github.com/yourusername/Kidney-Cancer-Survival-Analysis-XAI.git

cd Kidney-Cancer-Survival-Analysis-XAI

pip install -r requirements.txt
```

# ▶️ Run Project

```bash
python preprocessing.py

python training.py

python evaluation.py

python explainability.py
```

# 🔮 Future Work

- Cox Proportional Hazards Models
- Random Survival Forests
- Deep Learning Survival Models
- Multi-Omics Integration
- Clinical Web Application
- Additional Dataset Validation

# 👨‍💻 Authors

### Salman Khan
### Syed Muhammad Shayal
### Syed Abdul Ahad

## Supervisor

Dr. Sahib Khan

---

⭐ If you find this project useful, consider giving it a star.
