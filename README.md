# woe-credit-scoring
This project implements a credit scoring model to predict the probability of default (PD) using:

WOE (Weight of Evidence) transformation for feature engineering.

Logistic regression as the scoring model.

Validation tests to assess model robustness (Gini, stability, multicollinearity, etc.).

Key Steps
Data Preprocessing

Handle missing values, outliers, and categorical encoding.

Descriptive analysis (tr_for_students.csv).

WOE Transformation

Numerical features: Discretized into bins (like decision trees).

Categorical features: Regrouped (if needed) and mapped to WOE values.

Optional: Custom WOE function (+2 extra points).

Model Training

Logistic regression (statsmodels/sklearn) on WOE-transformed features.

Regularization tuning (optimizing Gini).

Validation

Out-of-time testing (vl_for_students.csv).

10 validation tests (ranking efficiency, Gini dynamics, factor stability, etc.).

Output

Scorecard: Factor buckets, WOE values, coefficients, DR, Gini, p-values, VIF.

Report: Modeling logic, assumptions, and test results (traffic-light colored).
