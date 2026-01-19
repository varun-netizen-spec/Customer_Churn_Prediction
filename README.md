# Customer Churn Prediction – Data Preprocessing & EDA

## Objective
Prepare a machine-learning–ready dataset for customer churn prediction through data cleaning, encoding, scaling, and exploratory data analysis.

---

## Dataset
- Customer Churn Prediction Dataset
- Records: 7,043
- Target Variable: `Churn` (Binary Classification)

---

## Data Preprocessing

### Data Cleaning
- Converted `TotalCharges` to numeric datatype
- Handled non-numeric values using coercion (`NaN`)
- Imputed missing values using median strategy
- Removed unique identifier column `customerID`

### Target Encoding
- Encoded `Churn` column:
  - Yes → 1
  - No → 0

### Categorical Feature Encoding
- Identified categorical (`object`) features
- Applied One-Hot Encoding
- Dropped first category to prevent multicollinearity
- Converted categorical features to boolean indicators

### Feature Scaling
- Applied StandardScaler to numerical features:
  - SeniorCitizen
  - tenure
  - MonthlyCharges
  - TotalCharges
- Ensured zero mean and unit variance

---

## Exploratory Data Analysis (EDA)

### Target Distribution Analysis
- Computed class distribution and percentage
- Identified class imbalance in target variable

### Numerical Feature Analysis
- Generated histograms for numerical features
- Verified feature distributions after scaling

### Boolean Feature Analysis
- Analyzed distribution of binary service-related features
- Assessed service usage patterns

---

## Final Dataset Summary
- Total Rows: 7,043
- Total Features: 31
- Data Types:
  - Boolean: 26
  - Integer: 3
  - Float: 2
- Missing Values: None
- Data Leakage: None

---

## Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## Output
- Cleaned and encoded dataset
- Scaled numerical features
- Dataset suitable for supervised ML classification models

