# diabetes-classification-ml
Diabetes Prediction Using Machine Learning

# Project Overview
This project uses machine learning to predict whether a person reported having diabetes, based on health indicators from the BRFSS dataset.
The goal is to compare different machine learning models and understand how well they identify people in the diabetes group.

# Dataset
- Dataset: BRFSS Diabetes Health Indicators
- Original size: 253,680 rows and 22 columns
- After removing duplicates: 229,474 rows
- Target: Diabetes_binary
  - 0: No reported diabetes
  - 1: Reported diabetes

# What I Did
1. Explored and cleaned the dataset.
2. Removed duplicate rows.
3. Split the data into training, validation, and test sets.
4. Trained and compared 10 machine learning experiments.
5. Tested class weighting, dropout, early stopping, and engineered features.
6. Evaluated the models using accuracy, precision, recall, F1-score, ROC-AUC, and PR-AUC.
Best Model Results
The final tuned HistGradientBoosting model achieved the following results on the test set:
Metric	Result
Accuracy	70.37%
Precision	31.48%
Recall	79.64%
F1-score	45.12%
ROC-AUC	81.59%
PR-AUC	43.68%


Recall was prioritized because the project aimed to identify as many people in the diabetes group as possible. Precision is lower, so some predictions may be false positives.
Tools Used
- Python
- pandas
- NumPy
- scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook
How to Run
1. Clone this repository:git clone <repository-url>
2. Open the project folder:cd <repository-folder>
3. Install the required libraries:pip install pandas numpy scikit-learn matplotlib seaborn jupyter
4. Open Jupyter Notebook:jupyter notebook
5. Open the project notebook and run the cells.
Important Note
This project predicts diabetes status recorded in survey data. It does not diagnose diabetes and should not be used as a medical tool.

# Author
Yohan Kouame