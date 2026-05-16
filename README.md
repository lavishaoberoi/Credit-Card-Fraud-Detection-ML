# Credit Card Fraud Detection using Machine Learning

## Overview
This project focuses on detecting fraudulent credit card transactions using multiple Machine Learning classification algorithms. The objective is to compare different ML models and identify which model performs best for fraud detection on highly imbalanced transaction data.

The project includes:
- Data preprocessing
- Exploratory Data Analysis (EDA)
- Model training and evaluation
- Accuracy comparison of multiple classifiers
- Confusion matrix visualization

## Dataset
The dataset used is the popular **Credit Card Fraud Detection Dataset** containing anonymized transaction features.

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

### 2. Exploratory Data Analysis
- Visualized fraud vs normal transactions
- Analyzed class imbalance

### 3. Model Training
- Split dataset into training and testing sets
- Trained multiple ML classification models

### 4. Model Evaluation
Models were evaluated using:
- Accuracy Score
- Confusion Matrix
- Classification Report


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

### Best Performing Model
- **Random Forest Classifier**
- Achieved the highest accuracy on the dataset.



## Visualizations
The project includes:
- Fraud vs Normal Transaction Count Plot
- Confusion Matrix Heatmap

## Project Structure

```text
credit-card-fraud-detection/
│
├── CreditCard_Fraud.ipynb
├── README.md
├── requirements.txt
└── images/
```

---

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

---

## Future Improvements

- Apply feature scaling
- Handle class imbalance using SMOTE
- Add ROC-AUC analysis
- Deploy using Flask or Streamlit
- Build a real-time fraud detection API



