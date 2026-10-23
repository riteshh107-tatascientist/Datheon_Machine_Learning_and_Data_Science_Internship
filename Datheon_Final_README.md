# Datheon Machine Learning & Data Science Internship

This repository contains my project work for the **Datheon Machine Learning & Data Science Internship**. Each task is organized separately so the code, documentation, and results can be reviewed independently.

## Repository Structure

```text
Datheon_Machine_Learning_and_Data_Science_Internship/
├── README.md
├── Task_1/
│   ├── Task_1_Notebook.ipynb
│   └── (supporting files, if required)
├── Task_2/
│   └── Task_2_Housing_Price_Prediction.ipynb
├── Task_3/
│   └── Task_3_Customer_Churn_Classification.ipynb
└── Task_4/
    └── Task_4_NLP_Sentiment_Classification.ipynb
```

Use the actual Task 1 notebook filename in place of `Task_1_Notebook.ipynb`. Add only files that are genuinely part of your project. Keep each task's supporting data or helper files inside its folder when needed.

## Task 1 — Completed Project

Task 1 is included as a separate notebook. See the `Task_1/` folder for the implementation and outputs.

**Before publishing:** replace this description with the exact Task 1 project title, dataset source, objective, and main results from your completed notebook. Do not claim results that are not present in the notebook.

## Task 2 — Real Estate Housing Price Prediction

**Objective:** Predict housing values and compare ordinary least squares (OLS), Ridge Regression, and Lasso Regression.

**Approach**
- Load and inspect the California Housing dataset from scikit-learn.
- Split the data into training and test sets.
- Apply preprocessing and feature engineering, including interaction features.
- Tune regularized models using cross-validation and `GridSearchCV`.
- Evaluate predictions using RMSE, MAE, and R².
- Review predicted-versus-actual and residual plots.

**Notebook:** `Task_2/Task_2_Housing_Price_Prediction.ipynb`

**Results:** The notebook should be run before submission. Use its actual test-set metrics and plots to describe the final model; do not insert estimated or fabricated scores.

## Task 3 — Predictive Customer Churn Classification

**Objective:** Predict whether a telecom customer is likely to churn, and compare Random Forest with XGBoost when the XGBoost dependency is available.

**Dataset source:** [IBM Telco Customer Churn CSV](https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv)

**Approach**
- Load and validate the public IBM Telco Customer Churn dataset.
- Clean `TotalCharges`, handle missing values, and exclude the customer identifier from model features.
- Encode categorical features using one-hot encoding.
- Address class imbalance using model class weighting / an imbalance-aware setting.
- Train and evaluate classification models.
- Report ROC-AUC, precision, recall, F1-score, and accuracy.
- Include ROC curve(s), a confusion matrix, and a top-feature-importance chart where supported.

**Notebook:** `Task_3/Task_3_Customer_Churn_Classification.ipynb`

**Results:** Run the notebook and report the actual test metrics. Do not state that ROC-AUC exceeds 0.80 unless the executed evaluation confirms it. The dataset is publicly available from IBM; do not describe it as a Datheon-created dataset unless Datheon confirms that.

## Task 4 — NLP Sentiment Classification on Customer Reviews

**Objective:** Classify customer reviews as positive or negative using TF-IDF text features.

**Dataset source:** [UCI Sentiment Labelled Sentences](https://archive.ics.uci.edu/static/public/331/sentiment+labelled+sentences.zip)

**Approach**
- Load and validate labelled review data.
- Clean text by lowercasing and removing HTML fragments, URLs, punctuation, and extra whitespace.
- Convert text into TF-IDF features.
- Compare Multinomial Naive Bayes and Logistic Regression.
- Evaluate using accuracy and a classification report.
- Plot a confusion matrix, inspect misclassified examples, and test custom review text.

**Notebook:** `Task_4/Task_4_NLP_Sentiment_Classification.ipynb`

**Results:** Run the notebook and add its actual evaluation results. The UCI dataset is used as the project data source unless the Datheon portal's download button specifies a different required dataset.

## Environment Setup

Install the packages used by the notebooks:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyterlab xgboost
```

Open the relevant notebook in Jupyter Notebook, JupyterLab, or Google Colab and run the cells from top to bottom. Some notebooks download public datasets, so an internet connection may be required. If a task has its own `requirements.txt`, use that file for the task-specific environment.

## Validation Before Submission

- Run each notebook from the first cell to the last without errors.
- Save the notebooks with their real outputs, metrics, and visualizations.
- Check that dataset sources are documented and data loading succeeds.
- Ensure the repository contains the notebooks and supporting files required to reproduce the work.
- Replace any remaining placeholders, especially the exact Task 1 title and results.
- Do not commit passwords, API keys, personal data, or unnecessary large dataset files.

## Project Notes

This repository is intended to document reproducible learning projects. Metrics may vary with data versions, library versions, preprocessing, and train/test splits. Interpret model results in the context of each dataset and avoid treating benchmark results as guarantees for real-world performance.
