# Datheon Machine Learning & Data Science Internship

This repository contains my project work for the Datheon Machine Learning & Data Science Internship. Each task is organized separately for easy review and reproducibility.

## Repository Structure

```text
Datheon_Machine_Learning_and_Data_Science_Internship/
├── README.md
├── Task_1/
│   └── Task_1_Notebook.ipynb
├── Task_2/
│   └── Task_2_Housing_Price_Prediction.ipynb
├── Task_3/
│   └── Task_3_Customer_Churn_Classification.ipynb
└── Task_4/
    └── Task_4_NLP_Sentiment_Classification.ipynb
```

Replace the Task 1 filename with your actual notebook filename. Include only files that exist in your repository.

## Task 1 — Completed Project

Task 1 notebook and its supporting files are stored in the `Task_1/` folder.

**Project objective:** Add the exact Task 1 title, dataset source, methodology, and findings from your completed notebook before submission.

## Task 2 — Real Estate Housing Price Prediction

**Objective:** Predict housing values and compare OLS, Ridge Regression, and Lasso Regression.

**Dataset:** California Housing dataset from scikit-learn.

**Methodology**
- Inspect and prepare the dataset.
- Handle missing values and engineer interaction features.
- Compare OLS, Ridge, and Lasso regression.
- Tune regularization using cross-validation and GridSearchCV.
- Evaluate using RMSE, MAE, and R².
- Review predicted-versus-actual and residual plots.

**Notebook:** `Task_2/Task_2_Housing_Price_Prediction.ipynb`

Add the actual metrics and findings after running the notebook successfully.

## Task 3 — Predictive Customer Churn Classification

**Objective:** Predict telecom customer churn using classification models.

**Dataset:** [IBM Telco Customer Churn CSV](https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv)

**Methodology**
- Validate the dataset and clean TotalCharges.
- Handle missing values and exclude customerID from predictors.
- One-hot encode categorical variables.
- Address class imbalance with class weighting.
- Train and compare Random Forest and XGBoost when available.
- Evaluate ROC-AUC, precision, recall, F1-score, and accuracy.
- Generate ROC curves, a confusion matrix, and feature importance plots.

**Notebook:** `Task_3/Task_3_Customer_Churn_Classification.ipynb`

Report actual evaluation results. Do not claim that ROC-AUC exceeds 0.80 unless your executed test results confirm it.

## Task 4 — NLP Sentiment Classification

**Objective:** Classify customer reviews as positive or negative using TF-IDF features.

**Dataset:** [UCI Sentiment Labelled Sentences](https://archive.ics.uci.edu/static/public/331/sentiment+labelled+sentences.zip), unless the Datheon portal specifies another required dataset.

**Methodology**
- Clean and validate review text.
- Convert text into TF-IDF features.
- Compare Multinomial Naive Bayes and Logistic Regression.
- Evaluate accuracy and the classification report.
- Plot a confusion matrix and inspect misclassified reviews.
- Test custom review text using a prediction function.

**Notebook:** `Task_4/Task_4_NLP_Sentiment_Classification.ipynb`

Add the actual metrics after running the notebook successfully.

## Environment Setup

Install the packages required by the notebooks:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyterlab xgboost
```

Open each notebook in Jupyter Notebook, JupyterLab, or Google Colab and run all cells from top to bottom. Internet access may be required to download datasets.

## Validation Before Submission

- Run each submitted notebook without errors.
- Save notebooks with actual outputs, metrics, and plots.
- Confirm dataset sources and file paths work.
- Ensure every notebook mentioned above is actually present.
- Replace the Task 1 placeholder with its exact title and findings.
- Do not include fabricated scores or unverified results.
- Never upload passwords, API keys, or private data.

## Project Notes

This repository documents learning projects and reproducible machine-learning workflows. Results may vary with data versions, preprocessing, library versions, and train/test splits. Benchmark results do not guarantee real-world performance.
