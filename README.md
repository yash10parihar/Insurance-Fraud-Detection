# Insurance Fraud Detection

This project predicts fraudulent first-party physical damage claims using structured insurance data. It was completed as part of the *Data Science Using Python (OPIM 5512)* course at the University of Connecticut and is based on the 2023 NESS Statathon competition dataset.

## 🧠 Project Objective

- Develop a classification model to detect fraudulent insurance claims
- Identify the most influential features contributing to fraud
- Ensure robust model performance while maintaining interpretability

## 📊 Dataset

- **Source**: 2023 NESS Statathon (Travelers Insurance)
- **Target Variable**: `fraud` (1 = fraudulent, 0 = legitimate)
- **Features Include**:
  - Driver attributes (age, income, marital status)
  - Claim characteristics (estimated payout, accident site)
  - Vehicle details (price, age, category)
  - Past claim history, reporting patterns, etc.

## ⚙️ Tools & Libraries

- `pandas`, `matplotlib`, `seaborn`
- `scikit-learn`, `imbalanced-learn`
- `pycebox`, `pulp` for PDP and interpretability

## 🔍 Methodology

- **Preprocessing**: Categorical encoding, missing value imputation, feature engineering
- **Train-Test Split**: 80/20 with stratification to address class imbalance
- **Resampling**: Used `SVMSMOTE` to handle minority fraud class
- **Models Tested**:
  - Logistic Regression
  - Decision Tree, Random Forest
  - Gradient Boosting
  - SVM, KNN

## 🧪 Evaluation

- Weighted F1 Score and Confusion Matrix on test set
- Feature importance using permutation importance
- Partial Dependence Plots (PDPs) for interpretability

## 💡 Key Insights

- Features such as **claim_est_payout**, **past_num_of_claims**, and **accident_site** had high influence on fraud detection.
- Oversampling significantly improved recall on the fraud class.
- Interpretability tools helped bridge technical results with actionable business recommendations.

## 👨‍💻 Team Members

- Yash Parihar  
- Rohit Akole

## 📅 Date

May 27, 2024

## 📜 License

This project is academic and for educational use only.
