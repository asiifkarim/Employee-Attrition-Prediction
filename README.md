# IBM HR Analytics: Employee Attrition Prediction

This project analyzes the IBM HR Analytics dataset to understand the key drivers behind employee attrition and to develop predictive models that can help organizations reduce turnover.

## 📊 Problem Statement

**Attrition** (employee departure) is a significant concern for HR departments. High attrition increases costs and affects team morale and productivity. This project aims to:

- Analyze attrition patterns and risk factors.
- Build predictive models to forecast attrition.
- Generate actionable business insights.

---

## 🔍 Dataset

- **Source**: [IBM HR Analytics Attrition & Performance](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Target Variable**: `Attrition` (Yes/No)

---

## 🛠️ Project Workflow

### 1. **Data Preprocessing**
- Handled missing values and encoded categorical variables.
- Addressed class imbalance using **SMOTE**.

### 2. **Exploratory Data Analysis (EDA)**
- Identified high-risk roles and departments.
- Analyzed correlations with job satisfaction, age, income, etc.

### 3. **Model Building**
- Built and evaluated:
  - **Random Forest Classifier**
  - **XGBoost Classifier**
- Used **stratified train-test split** for balanced evaluation.

### 4. **Model Evaluation**
- Metrics used:
  - Accuracy, Precision, Recall, F1-Score
  - Confusion Matrix
  - ROC-AUC Curve

### 5. **Feature Importance & Explainability**
- Identified top 5 drivers of attrition using feature importance plots.
- Focus on **OverTime**, **Job Satisfaction**, **Age**, **Income**, **Years at Company**.

---

## 🧠 Key Findings

- **OverTime** is the strongest indicator of attrition.
- Younger employees and those with low job satisfaction are more likely to leave.
- High attrition in the **Sales** and **Human Resources** departments.

---

## 💡 Business Recommendations

- Reduce excessive overtime and improve work-life balance.
- Prioritize satisfaction initiatives and surveys.
- Focus on early-tenure employees (first 1-3 years).
- Review compensation for fairness and competitiveness.

---

## 📁 Files in this Repository

| File | Description |
|------|-------------|
| `HR_Attrition_Analysis.ipynb` | Jupyter notebook with full analysis and modeling |
| `Business_Insight_Report.pdf` | PDF summary report with insights and recommendations |
| `README.md` | Project overview and setup instructions |

---

## 🚀 Getting Started

### Requirements
- Python 3.7+
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `imblearn`

### Run the Project
```bash
git clone https://github.com/your-username/hr-attrition-analysis.git
cd hr-attrition-analysis
jupyter notebook HR_Attrition_Analysis.ipynb
