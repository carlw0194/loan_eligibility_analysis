# loan_eligibility_analysis

# 📊 Loan Eligibility Analysis Dashboard

This project explores historical loan application data to uncover key factors influencing loan approvals. By combining data preparation, feature engineering, exploratory data analysis (EDA), and dashboard design, the project aims to provide financial institutions with a transparent, interactive tool for assessing loan eligibility. It is designed as a portfolio-worthy, end-to-end data analysis solution.

---

## 🔍 Project Objectives

- Understand which applicant attributes (e.g., income, credit history, dependents) most influence loan approval decisions.
- Clean and prepare real-world loan application data for analysis and modeling.
- Engineer new features such as total income, income per dependent, and debt-to-income ratio to improve analytical depth.
- Build a dashboard that communicates findings clearly to non-technical stakeholders.
- Train and evaluate a Random Forest classifier to predict loan approvals with feature importance analysis.
- Export enriched data with predictions and confidence scores for comprehensive Power BI visualization.

---

## 🧰 Tools & Technologies

- **Python** (Pandas, NumPy, Seaborn, Matplotlib)
- **Power BI / Streamlit** (Dashboard and visualization)
- **Scikit-learn** (Optional: classification model)
- **GitHub** (Version control and project hosting)

---

## 📁 Key Components

| Folder / File                     | Description                                                      |
| --------------------------------- | ---------------------------------------------------------------- |
| `laondata/`                       | Raw datasets (`loan-train.csv`, `loan-test.csv`)                 |
| `loan_eligibility_analysis.ipynb` | Complete analysis notebook with EDA, feature engineering, and ML |
| `loan_analysis_results.xlsx`      | Processed data with predictions for Power BI import              |
| `models/` _(optional)_            | ML scripts and evaluation results                                |
| `README.md`                       | Project overview and documentation                               |

---

## 💡 Business Questions Answered

1. **Who is more likely to be approved for a loan?**
   → Based on credit history, income, dependents, and property area.

2. **How do applicant attributes affect approval rates?**
   → Visual breakdowns by gender, education, credit history, etc.

3. **What role does income play in eligibility?**
   → Analysis of total income, loan amount ratios, and dependents.

---

## 🤖 Machine Learning Module

### Model Selection & Rationale

**Random Forest Classifier** was chosen for loan approval prediction because:

- **Interpretability**: Provides clear feature importance rankings for business insights
- **Robustness**: Handles mixed data types (numerical and categorical) effectively
- **Performance**: Excellent baseline performance with minimal hyperparameter tuning
- **Feature Relationships**: Captures non-linear relationships and feature interactions

### Key Features Used

- **Original Attributes**: Credit history, loan amount, income, education, demographics
- **Engineered Features**: Total income, income-per-dependent, EMI-to-income ratio, debt ratios
- **Missing Value Indicators**: Flags for originally missing data points

### Model Performance

- **Cross-validation accuracy**: ~80%+ (varies by data split)
- **Feature Importance**: Credit history and engineered income ratios are top predictors
- **Export**: All predictions include confidence scores for risk assessment

---

## 📈 Dashboard Features

- **Overview Page**:

  - KPIs: Approval Rate, Avg Loan Amount, Avg Applicant Income, Model Accuracy
  - Trends by Property Area, Credit History, and Education
  - Feature Importance Chart from ML Model

- **Applicant Analysis**:

  - Filters: Gender, Marital Status, Dependents, Employment
  - Income distributions for approved vs rejected applicants
  - Predicted vs Actual Approval Comparison

- **Credit & Risk Insights**:

  - Heatmaps showing credit history impact
  - Prediction confidence distribution
  - Risk segmentation based on model scores

- **ML Model Performance**:
  - Feature importance rankings
  - Prediction accuracy metrics
  - Confidence score analysis by approval status

---

## 🚀 Outcome

This project delivers a powerful, interactive tool to help financial institutions and analysts understand loan approval patterns, streamline decision-making, and improve transparency with applicants. It also showcases end-to-end data handling, from raw CSVs to a polished dashboard, making it ideal for a professional portfolio.

data source- https://www.kaggle.com/code/vikasukani/loan-eligibility-prediction-machine-learning/input
