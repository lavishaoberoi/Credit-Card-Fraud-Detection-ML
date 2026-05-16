# Credit Card Fraud Detection using Machine Learning

## Overview
This project focuses on detecting fraudulent credit card transactions using multiple Machine Learning classification algorithms. The objective is to compare different ML models and identify which model performs best for fraud detection on highly imbalanced transaction data.

The project includes:
- Data preprocessing
- Exploratory Data Analysis (EDA)
- Feature scaling using StandardScaler
- Class imbalance handling using SMOTE
- Model training and evaluation
- ROC-AUC analysis
- Accuracy comparison of multiple classifiers
- Confusion matrix visualization

## Dataset
The dataset used is the popular **Credit Card Fraud Detection Dataset** containing anonymized transaction features.
The dataset can be downloaded from Kaggle:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

After downloading, place `creditcard.csv` in the project directory.


### Dataset Features
- Numerical transaction features
- Transaction amount
- Time feature
- Target column:
  - `0` → Normal Transaction
  - `1` → Fraudulent Transaction

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)

## Machine Learning Models Implemented
- Logistic Regression
- Linear Discriminant Analysis (LDA)
- Naive Bayes
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)


## Workflow

### 1. Data Preprocessing
- Loaded dataset using Pandas
- Checked dataset shape and missing values
- Separated features and target labels

### 2. Feature Scaling
- Applied `StandardScaler` to normalize feature values
- Improved performance of distance-based models like SVM and KNN

### 3. Handling Class Imbalance
- Used **SMOTE (Synthetic Minority Oversampling Technique)** to balance fraud and normal transaction samples
- Improved fraud detection capability on minority class transactions

### 4. Exploratory Data Analysis
- Visualized fraud vs normal transactions
- Analyzed dataset imbalance

### 5. Model Training
- Split dataset into training and testing sets
- Trained multiple Machine Learning classification models

### 6. Model Evaluation
Models were evaluated using:
- Accuracy Score
- Confusion Matrix
- Classification Report
- ROC-AUC Score

## Results
## Model Performance Comparison

| Rank |             Model                   | Performance     |
|------|-------------------------------------|-----------------|
| 🥇 1 | Random Forest Classifier            | 99.94% Accuracy |
| 🥈 2 | Linear Discriminant Analysis (LDA)  | 99.91% Accuracy |
| 🥉 3 | Decision Tree Classifier            | 99.89% Accuracy |
| 4    |  Logistic Regression                 | 99.85% Accuracy |
| 5    | K-Nearest Neighbors (KNN)            | 99.79% Accuracy |
| 6    |  Support Vector Machine (SVM)        | 99.79% Accuracy |
| 7    |  Naive Bayes Classifier              | 98.50% Accuracy |


### 🏆 Best Performing Model
**Random Forest Classifier** achieved the highest accuracy among all implemented models.

## ROC-AUC Analysis
The Random Forest model achieved a **ROC-AUC Score of 0.9366**, indicating excellent capability in distinguishing fraudulent and legitimate transactions.

## Visualizations
The project includes:
- Fraud vs Normal Transaction Count Plot
- Confusion Matrix Heatmap
- ROC-AUC Curve
  

## Project Structure

```text
credit-card-fraud-detection/
│
├── CreditCard_Fraud.ipynb
├── README.md
├── requirements.txt
└── images/
```

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/credit-card-fraud-detection.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook:

```bash
jupyter notebook
```


## Future Improvements
- Perform hyperparameter tuning for improved model optimization
- Deploy the model using Flask or Streamlit
- Build a real-time fraud detection API



