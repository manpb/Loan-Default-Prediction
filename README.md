# Loan Default Prediction

This project applies machine learning techniques to predict whether a borrower will default on a loan, supporting more informed lending decisions and risk mitigation.

## 🔍 Project Summary
- Historical loan dataset with 255k+ records and 18 features
- Key steps:
  - Data sampling for efficient modelling
  - Feature selection using SelectKBest + Chi-Square
  - Model training and evaluation using SVM and Random Forest

## 🧠 Models & Performance

| Model | Train Accuracy | Test Accuracy | Notes |
|------|---------------:|--------------:|------|
| Linear SVM | 0.879 | 0.881 | Good linear baseline |
| Random Forest | 0.999 | 0.889 | Best performance but slightly overfits |

➡️ Random Forest selected as the best model

Top predictors include: CreditScore, Income, LoanAmount, InterestRate, MonthsEmployed, Education, EmploymentType.

## 📌 Key Insights
- Target imbalance: ~11.6% defaults → requires targeted evaluation
- Financial stability indicators strongly influence credit risk
- Enhances lending decision accuracy and reduces exposure

## 🚀 How to Run
    git clone https://github.com/manpb/Loan-Default-Prediction.git
    cd Loan-Default-Prediction
    pip install numpy pandas seaborn scikit-learn
    jupyter notebook Loan_default_prediction.ipynb

## 📂 Project Structure
    Loan-Default-Prediction/
    │
    ├── Data/
    │   ├── train.csv     # Training dataset
    │   └── test.csv      # Testing dataset
    │
    ├── Loan_default_prediction.ipynb
    └── README.md

## 👤 Author
**Manuja Palamakumbura**  
MSc Information Technology Management (Distinction)  
Website: https://www.manujasprojects.co.uk/  
LinkedIn: https://www.linkedin.com/in/manuja-palamakumbura/
