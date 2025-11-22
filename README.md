# Loan Default Prediction  
*(Notebook: `Loan_default_prediction.ipynb`)*

## Project Overview  
This project presents an end-to-end workflow for predicting loan default risk using historical borrower and loan data. The aim is to help a lending institution better assess which applicants are likely to default, thereby reducing financial risk and improving decision-making.

Key steps include:

- Data ingestion, cleaning and exploratory analysis  
- Feature engineering & transformation  
- Handling class imbalance  
- Model training, evaluation and comparison  
- Interpretation of results and insights

## Motivation  
Loan defaults pose a significant cost to financial institutions — both in direct losses and in opportunity cost from rejected creditworthy applicants. By leveraging machine learning and data analytics, the model aims to:

- **Improve predictive accuracy** of identifying defaulters.  
- **Reduce false negatives** (approving a loan to someone who will default).  
- **Provide interpretability** around why decisions/predictions are made, supporting transparency and trust in credit processes.

## Dataset & Features  
The notebook uses a dataset containing borrower demographic, employment, loan attributes and payment history. Typical variables include:

- Loan amount, interest rate, term  
- Employment length, annual income  
- Home ownership status, verification status  
- Target variable: default vs non-default

> **Note**: Please update this section with the actual dataset description (number of records, how many features, source, how cleaned) for full accuracy.

## Methodology  

### 1. Exploratory Data Analysis (EDA)  
- Investigated missing values, outliers, data distributions.  
- Visualised key relationships (e.g., interest rate vs default, term vs default).  
- Checked class balance between default vs non-default outcomes.

### 2. Data Preprocessing & Feature Engineering  
- Cleaned and imputed missing values (e.g., employment length, income).  
- Transformed categorical features (e.g., home ownership, verification status) via encoding.  
- Created derived features (e.g., debt-to-income ratio, loan to income ratio).  
- Scaled/normalized numerical features where appropriate.  
- Addressed class imbalance using techniques like oversampling (SMOTE) or class weighting.

### 3. Model Training & Evaluation  
- Split the data into training and test (or validation) sets.  
- Compared multiple modelling approaches (for example: logistic regression, random forest, XGBoost).  
- Performed hyperparameter tuning (grid search / random search) if included.  
- Evaluated models using metrics including: accuracy, precision, recall, F1-score, ROC-AUC, and possibly cost-sensitive metrics given the context.  
- Selected the best performing model according to the business objective (typically high recall on defaulters while maintaining reasonable precision).

### 4. Model Interpretation & Insights  
- Identified most important features influencing default risk (e.g., interest rate, term, income).  
- Utilised model‐interpretability techniques (SHAP values, feature importance) to explain predictions.  
- Generated actionable insights: for instance, borrowers with low income + high term + high interest rate have elevated default risk; or employment length correlates with risk.  
- Discussed trade-offs (false positives vs false negatives) and business implications (cost of approving defaulters vs rejecting good applicants).

## Results & Business Implications  
- The best model achieved (insert key metrics: recall, precision, AUC, etc).  
- Feature importances highlight [list top 3-5 features].  
- Business recommendations:  
  - Prioritise reducing false negatives to minimise financial loss from defaulted loans.  
  - Consider adjusting credit approval policies (e.g., stricter terms for high‐risk profiles) or dynamic pricing (higher interest for higher risk).  
  - Use interpretability outputs to support decision‐makers and regulatory compliance.

## Usage Instructions  
To run or reproduce this notebook:

1. Clone the repository:  
   ```bash
   git clone https://github.com/manpb/Loan-Default-Prediction.git
