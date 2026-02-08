# Feature Engineering and Performance Improvement

## Objective
The objective of this project is to demonstrate the impact of feature engineering on model performance using the Wine Quality (Red Wine) dataset. The focus is on improving model understanding and interpretability rather than using complex models.

---

## Dataset
- Dataset: Wine Quality (Red Wine)
- Source: Kaggle
- Target Variable: Wine quality

The original quality scores were converted into a binary classification problem:
- Quality ≥ 6 → Good wine (1)
- Quality < 6 → Bad wine (0)

This conversion reduces class imbalance and improves model interpretability.

---

## Data Cleaning
- Checked for missing values (none found)
- Removed duplicate rows
- All features were numerical, so encoding was not required

---

## Baseline Model
- Model Used: Logistic Regression
- Features: Original chemical properties only
- Evaluation Metrics:
  - Accuracy
  - Precision
  - Recall

This baseline establishes initial performance before feature engineering.

---

## Feature Engineering
The following engineered features were created:

1. **Combined Acidity**
   - Combines fixed, volatile, and citric acidity
2. **Sulfur Ratio**
   - Ratio of free sulfur dioxide to total sulfur dioxide
3. **Residual_Sugar_Ratio**
   - Ratio of residual sugar to density

These features capture domain knowledge related to wine chemistry and fermentation quality.

---

## Models Used
1. Logistic Regression (linear baseline)
2. Decision Tree Classifier (non-linear model)

Decision Trees were used to better exploit non-linear feature interactions.

---

## Performance Comparison
Model performance was evaluated before and after feature engineering using accuracy, precision, and recall. Feature engineering showed limited improvement for the linear model but provided clearer gains when using the Decision Tree model.

---

## Conclusion
Feature engineering improved model interpretability and allowed non-linear models to better capture relationships between chemical properties and wine quality. Even when accuracy remained unchanged, engineered features helped create more meaningful and robust representations.

---

## How to Run
1. Clone the repository
2. Install required libraries:
   - pandas
   - numpy
   - scikit-learn
3. Run the notebook or Python script

---

## Author
Prisha Kushwaha
