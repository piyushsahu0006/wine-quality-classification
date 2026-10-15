Wine Quality Classification
A machine learning project that explores the Red Wine Quality dataset and compares classification models to predict wine quality categories from physicochemical properties.
Project Overview
This project:
- Loads and explores the Red Wine Quality dataset.
- Checks missing values and duplicate records.
- Visualizes feature distributions, quality scores, and feature correlations.
- Groups wine quality scores into three categories:
  - Low: quality score ≤ 4
  - Medium: quality score 5–6
  - High: quality score ≥ 7
- Splits the data into training and test sets.
- Standardizes numeric features.
- Trains and evaluates three classifiers:
  - Random Forest
  - Stochastic Gradient Descent (SGD) Classifier
  - Support Vector Classifier (SVC)
- Compares model metrics and visualizes feature importance.
Dataset
The code expects the file winequality-red.csv in the project root directory.
The dataset is commonly distributed as part of the UCI Machine Learning Repository's Wine Quality dataset:
https://archive.ics.uci.edu/dataset/186/wine+quality
Download the red wine dataset and place winequality-red.csv beside wine_quality_classification.py.
Expected CSV separator: semicolon (;).
The dataset file is not included in this repository template. Follow the dataset source's terms and instructions when downloading or redistributing it.

Project Structure
wine-quality-classification/
├── README.md
├── wine_quality_classification.py
├── requirements.txt
├── .gitignore
└── data/
    └── README.md
Requirements
- Python 3.9 or newer
- pandas
- matplotlib
- seaborn
- scikit-learn
Install dependencies:
pip install -r requirements.txt
How to Run
1. Clone or download this repository.
2. Download winequality-red.csv and put it in the project root folder.
3. Install dependencies:
   pip install -r requirements.txt
4. Run the script:
   python wine_quality_classification.py
The script prints dataset information, classification reports, model comparison metrics, and feature importance. It also opens plots using Matplotlib.
Evaluation
The script evaluates each model using:
- Accuracy
- Precision
- Recall
- Weighted F1-score
- Macro F1-score
- Confusion matrix
Metrics are calculated from the test split when the script is run. Results can vary with changes to the dataset or code.
Important Note
The target categories are imbalanced, especially the Low category. Accuracy alone may not reflect performance on the minority classes, so review per-class precision, recall, F1-score, and the confusion matrices too.
Skills Demonstrated
Python · Pandas · Data Visualization · Exploratory Data Analysis · Scikit-learn · Classification · Model Evaluation
Author
Piyush Sahu
Add your GitHub profile and LinkedIn links here if you want them displayed.
