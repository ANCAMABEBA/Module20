# Module20
Initial Report and Exploratory Analysis (EDA)
## Baseline Credit Default Model — Summary of Findings

This project implements a baseline logistic regression model to predict credit default risk and establish an initial performance benchmark.

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
