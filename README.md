# Breast Cancer Classification Using Logistic Regression

## 1. Context

Early and accurate detection of breast cancer is important for improving patient outcomes. This project explores the use of machine learning to distinguish between benign and malignant breast tumours based on measurements of cell nuclei extracted from digitised fine-needle aspiration (FNA) biopsy images.

The objective was to develop a Logistic Regression model to classify tumours as either benign (non-cancerous) or malignant (cancerous).

The dataset was obtained from [Kaggle](https://www.kaggle.com/datasets/wasiqaliyasir/breast-cancer-dataset) and contains 569 rows and 33 columns.

The analysis was conducted using Jupyter Notebook in Visual Studio Code, with the following Python libraries:

- Pandas
- Matplotlib
- Scikit-learn

## 2. Methodology

- Explored the dataset to understand its structure and identify potential issues.
- Removed the ID column and an empty column.
- Encoded the target feature
- Separated the features and target variable.
- Split the data into training and testing sets.
- Scaled the features using `StandardScaler`, fitting the scaler on the training data and applying it to the test data.
- Trained a Logistic Regression model.
- Evaluated model performance using accuracy, precision, recall, F1-score and a confusion matrix.

## 3. Results

The Logistic Regression model achieved **97.37% accuracy** on the test dataset, correctly classifying 111 out of 114 samples. A confusion matrix of the results:

Classification Report

| Class      | Precision | Recall | F1-score | Support |
|------------|-----------|--------|----------|---------|
| Benign (0) | 0.97      | 0.99   | 0.98     | 71      |
| Malignant (1) | 0.98   | 0.95   | 0.96     | 43      |
|------------|-----------|--------|----------|---------|
| Accuracy   |           |        | 0.97     | 114     |
| Macro Avg  | 0.97      | 0.97   | 0.97     | 114     |
| Weighted Avg | 0.97    | 0.97   | 0.97     | 114     |
