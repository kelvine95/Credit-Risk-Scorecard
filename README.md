# Credit Risk Model Development

## 1. Data Preparation

### Data Exploration and Cleaning
- **Dataset Overview**: 30,000 records divided for model training and out-of-sample validation.
- **Default Distribution**: Specified percentages for Good and Bad in both training and validation sets.
- **Data Integrity**: Ensured with no missing values and correct data types.
- **Categorical Variables**: Identified specific variables as categorical.

### Feature Transformation
- **Outliers Handling**: Addressed using the Interquartile Range method.

## 2. Feature Selection

### Categorical Feature Selection Using Chi-square Test
- **Test Application**: Evaluated the association with the target variable.

### Continuous Feature Selection Using Mann-Whitney Test
- **Test Application**: Selected top features based on p-values.

### Multi-collinearity and Contingency Coefficient
- **Analysis**: Spearman correlation heatmap used; certain variables dropped due to high correlation or contingency coefficients.

### Information Value (IV) and Weight of Evidence (WoE)
- **WoE Calculation**: Assisted in binarization.
- **Feature Selection**: Selected features based on IV, creating binary variables.

## 3. Model Evaluation and Validation

### Machine Learning Modelling
- **Model Training**: Logistic Regression and Random Forest with different feature sets.
- **Addressing Data Imbalance**: Adjusted class weights in models.
- **Model Performance Metrics**: Used AUC and Gini Coefficient.
- **Model Selection**: Based on performance metrics; preferred model selected.

### Model Discriminatory Power
- **Analysis**: Assessed using probability distribution and performance scores.

## 4. Scorecard Development and Calibration

### Scorecard Development
- **Transformation**: Adjusted to align with typical credit scoring range.

### Scorecard Calibration
- **Process**: Adjusted coefficients to match credit scoring practices and risk levels.

## Conclusion
- **Overview**: Effective combination of predictive accuracy and practical applicability in the credit risk model and scorecard.
