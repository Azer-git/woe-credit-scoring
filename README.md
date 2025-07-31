# woe-credit-scoring
### Overview
This project implements a **Probability of Default (PD) scoring model** using:
- **WOE (Weight of Evidence)** transformation for feature engineering
- **Logistic Regression** for binary classification (default/non-default)
- Comprehensive validation tests (Gini, stability, multicollinearity, etc.)

### Key Features
1. **Data Processing**
   - Handles missing values and outliers
   - Descriptive analysis of `tr_for_students.csv`

2. **WOE Transformation**
   - Numerical features: Discretized into optimized bins
   - Categorical features: Regrouped and mapped to WOE values
   - *Optional*: Custom WOE implementation (+2 extra points)

3. **Model Development**
   - Logistic regression (statsmodels/sklearn)
   - Regularization tuning (Gini optimization)

4. **Validation**
   - 10 validation tests on `vl_for_students.csv`:
     - Ranking efficiency, factor stability, Gini dynamics, etc.
   - Traffic-light results reporting

