# 💳 Credit-Risk-Prediction

## 📌 Project Overview & Task Objective

The `credit_risk_prediction.ipynb` focused on 
predicting loan application approvals based on demographic and financial features. The 
primary objective is to build a classification model that can accurately determine 
whether a loan application will be approved or rejected, leveraging the provided Loan 
Prediction Dataset.

## 📂 Dataset Information

The project utilizes the Loan Prediction Dataset, which includes `train.csv`  and `test.csv`
files. The dataset contains various features related to loan applicants and their financial 
status. The target variable is `Loan_Status`  (Y = approved, N = not approved).

**Key Issues Handled:**
- Missing values in several columns.
- Categorical data (e.g., gender, education) requiring conversion to numerical format.

## ✨ Features

- Data loading and initial inspection.
- Handling missing values through imputation.
- Encoding categorical variables.
- Exploratory Data Analysis (EDA) to understand feature distributions and their
  relationships with the target variable.
- Training and evaluating classification models (Logistic Regression, Decision Tree).
- Providing a usage example for predicting loan status for new applicants.

## 🛠️ Installation

To run this notebook locally, you will need Python installed along with the following 
libraries. You can install them using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
## 🚀 Approach

My approach to credit risk prediction involved the following steps:

- **Library Import**: Imported essential Python libraries for data manipulation
  (pandas, numpy), visualization (matplotlib, seaborn), and machine learning
  (sklearn).
  
- **Data Loading**: Loaded the `train.csv`  dataset into a pandas DataFrame.

- **Data Cleaning and Preparation**:
  - **Handle Missing Values**: Categorical features were imputed using the mode,
    and numerical features (like `LoanAmount` ) were imputed using the median.
  - **Encode Categorical Variables**: Binary categorical variables were transformed
    using `LabelEncoder` , while multiclass variables were converted using one-
    hot encoding ( `pd.get_dummies` ).
    
- **Exploratory Data Analysis (EDA)**: Analyzed feature distributions and their
    relationships with the `Loan_Status`  target variable. A key visualization included
    plotting `Credit_History`  against `Loan_Status`  to understand their correlation.
  
- **Model Training and Testing**:
    The dataset was split into training and testing sets (80/20 split).
  - **Random Forest Classifier**: A Random Forest model was trained with 
      `max_depth=5` .
  - **Logistic Regression**: A Logistic Regression model was trained for binary
      classification.
  - **Decision Tree**: A Decision Tree Classifier was trained.

- **Model Evaluation**: Evaluated the trained models using accuracy score, confusion
    matrices, and classification reports to assess their performance in predicting loan
    approval.

## 🧰 Technologies Used
- P Y T H ON
- P A N D A S
- NUMP Y
- MA T P L O T L I B
- S E A B O R N
- S C I K I T - L E A R N

## 📉 Visualizations

### 📈 Credit History vs Loan Status
![image](https://github.com/user-attachments/assets/781b35b3-22b1-4c25-83cf-304dcaf900db)

**Explanation**: This bar plot illustrates the relationship between an applicant's credit 
  history and their loan approval status. It clearly shows that applicants with a good credit 
  history (represented by '1') are significantly more likely to have their loans approved 
  compared to those with a bad credit history (represented by '0'). This highlights the 
  critical role of credit history in loan approval decisions.

### 🟩 Logistic Regression Confusion Matrix
![image](https://github.com/user-attachments/assets/1207859a-db42-4d95-b3a6-fe9efc1faf33)

**Explanation**: This confusion matrix visualizes the performance of the Logistic 
  Regression model. It shows the counts of true positives (correctly predicted approved 
  loans), true negatives (correctly predicted rejected loans), false positives (rejected loans 
  incorrectly predicted as approved), and false negatives (approved loans incorrectly 
  predicted as rejected). A good model aims for high true positive and true negative 
  counts, and low false positive and false negative counts. This matrix helps in 
  understanding the types of errors the model is making.

### 🟨 Decision Tree Confusion Matrix
![image](https://github.com/user-attachments/assets/59cb67f2-114e-4eb4-93ce-e0b54935de10)

**Explanation**: Similar to the Logistic Regression confusion matrix, this matrix displays 
  the performance of the Decision Tree model. By comparing this with the Logistic 
  Regression matrix, one can observe the differences in how each model handles true/
  false positives and negatives, providing a visual comparison of their predictive 
  capabilities and error patterns.

## 📊 Results and Insights

### Key Insights:
  - **Credit History Impact**: The analysis clearly showed that credit history is a strong 
      predictor of loan approval. Applicants with a good credit history (Credit_History = 1) had 
      a significantly higher chance of loan approval, while those with a bad credit history 
      (Credit_History = 0) were mostly rejected.
  - **Model Performance**: The Logistic Regression model achieved an accuracy of `(78.86%)`, 
      outperforming the Decision Tree model `(69.11%)`. This indicates that Logistic Regression 
      is more suitable for this dataset given the features and their relationships.
  - **Confusion Matrices**: The confusion matrices for both models provided a detailed 
      breakdown of `true positives`, `true negatives`, `false positives`, and `false negatives`, offering 
      insights into where each model performed well and where it struggled.
    
### Final Outcome:
  - The project successfully demonstrates a workflow for credit risk prediction, from data preprocessing to model evaluation.
  - The Logistic Regression model proved to be effective in predicting loan approval status based on the given features. 
  - Further improvements could involve hyperparameter tuning or exploring more advanced ensemble methods.

## 🧪 Usage

```bash
# 1. Clone the repository
git clone https://github.com/Shilpachhatani/Credit-Risk-Prediction.git

# 2. Navigate to the project directory
cd Credit-Risk-Prediction

# 3. Open the notebook
jupyter notebook Credit_Risk_Prediction.ipynb

```

## 🤝 Contributing

Contributions are welcome! If you have any suggestions or improvements, please open 
an issue or submit a pull request.

## 📬 Contact

For questions or collaboration:
- GitHub: `Shilpachhatani`
- Email: `shilpachhatani669@gmail.com`.

