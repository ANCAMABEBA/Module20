# Module20

## Initial Report: EDA and Baseline Credit Default Model — Summary of Findings
The purpose of this notebook is to perform an end-to-end exploratory data analysis (EDA) and develop a baseline predictive model to understand the key drivers of loan default risk.
The analysis focuses on:
- Understanding borrower, loan, and credit characteristics
- Identifying variables that differentiate default vs non-default behavior
- Establishing a robust, interpretable baseline model to serve as a benchmark for further refinement

The Jupiter Notebook can be found here: [InitialReportEDA.ipynb](https://github.com/ANCAMABEBA/Module20/blob/main/InitialReportEDA.ipynb)

Dataset ("loan.csv") is from kaggle ("Lending Club Loan Data"): https://www.kaggle.com/datasets/saurabh13nov/lending-club-loan-data

### Analytical Approach
The analysis follows a structured workflow:
- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Feature Selection
- Baseline Modeling

### Model Performance
- Achieved an **ROC–AUC of 0.708**, indicating **moderate discriminatory power**.
- Confirms the presence of meaningful credit risk signal and provides a solid reference point for further model development.

### Key Risk Drivers
- **Higher default risk** is associated with:
  - Higher interest rates
  - Higher loan-to-income ratios
  - Prior delinquencies
- **Lower default risk** is associated with:
  - Higher income
  - Lower DTI
  - Longer employment history
  - Home ownership

### Model Quality and Limitations
- Coefficient signs are economically intuitive, supporting **interpretability and stability**.
- Logistic regression’s linear assumptions may limit its ability to capture nonlinear risk patterns.
- ROC–AUC alone does not reflect business impact; additional metrics are needed.

### Next Steps
- Evaluate more advanced models to capture nonlinear effects.
- Assess precision–recall, lift, and calibration to translate performance into business value.
- Review feature inclusion (e.g., interest rate) based on the modeling objective.

**Conclusion:**  
The baseline model provides a reliable, interpretable foundation for advancing toward more sophisticated credit risk models.
