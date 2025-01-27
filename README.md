# High-Dimensional Predictive Analytics for Academic Performance Using Machine Learning
<div align="center">
  <img src="https://github.com/user-attachments/assets/30286c6b-5359-4390-b91b-24f83da58d33" alt="Image" width="500">
</div>


## Project Description
This project explores the development of advanced machine learning models to predict academic performance based on high-dimensional datasets. The goal is to analyze multivariate student data and build robust regression and classification models for predicting key academic outcomes, such as grades (G1, G2, G3).

The dataset used contains 30 categorical features and 3 target variables representing student grades. The workflow includes feature engineering, feature selection, statistical analysis, and model building using ensemble methods like Random Forest and Decision Tree models.

---

## Objectives
1. Predict academic grades (G1, G2, G3) using machine learning.
2. Perform feature selection to identify significant predictors.
3. Evaluate both regression and classification models for accurate performance forecasting.
4. Address class imbalances and multicollinearity for optimized results.

---

## Dataset
- The dataset consists of 30 categorical features and 3 target variables (G1, G2, G3).
- All features are categorical.
- The target variables are analyzed as both continuous and categorical data for regression and classification purposes.

---

## Methodology

### Data Preprocessing
1. **Handling Missing Values:**
   - Verified that there are no missing values in the dataset.

2. **Feature Encoding:**
   - Applied label encoding to all categorical features to make them suitable for machine learning models.

3. **Class Balancing:**
   - Addressed imbalanced data using random oversampling to ensure fair training and evaluation.

### Feature Selection
1. **Chi-Square Test:**
   - Performed chi-square tests to identify the most significant features influencing each target variable (G1, G2, G3).
   - Selected features with the lowest p-values for model building.

2. **Handling Multicollinearity:**
   - Investigated multicollinearity among features to ensure minimal redundancy.
   - Random Forest models inherently handle multicollinearity well, so it was retained during training.

### Model Building
1. **Regression Models:**
   - Built models treating G1, G2, G3 as continuous variables.
     - **Random Forest Regressor**
     - **Decision Tree Regressor**
   - **Evaluation Metrics:**
     - Mean Squared Error (MSE)
     - R-squared (R²)

2. **Classification Models:**
   - Built models treating G1, G2, G3 as categorical variables.
     - **Random Forest Classifier**
   - **Evaluation Metrics:**
     - Accuracy
     - Confusion Matrix
     - Classification Report

---

## Results
### Random Forest Regressor
- **G3:** MSE = 5.81, R² = 0.80 (80%)
- **G1:** MSE = 4.68, R² = 0.80 (80%)
- **G2:** MSE = 8.15, R² = 0.70 (70%)

### Decision Tree Regressor
- **G3:** MSE = 8.30, R² = 0.72 (72%)
- **G1:** MSE = 6.54, R² = 0.73 (73%)
- **G2:** MSE = 13.10, R² = 0.53 (53%)

### Random Forest Classifier
- **G3:** Accuracy = 74%
- **G1:** Accuracy = 67%
- **G2:** Accuracy = 65%

The Random Forest Regressor consistently outperformed other models in predicting continuous outcomes, while the Random Forest Classifier delivered strong results for categorical targets.

---

## Conclusion
1. Chi-Square tests effectively identified the most significant predictors for G1, G2, and G3.
2. Random Forest Regressor demonstrated robust performance with high R-squared values and minimal errors.
3. The project showcases the power of ensemble learning models in handling high-dimensional categorical data for academic performance prediction.
