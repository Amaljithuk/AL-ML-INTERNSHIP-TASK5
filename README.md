Heart Disease Classification with Decision Trees and Random Forests
Task Overview
This repository contains the solution for Task 5 of the Elevate AI & ML Internship. The objective is to implement tree-based models (decision tree and random forest) on the Heart Disease Dataset to predict target (0: No Heart Disease, 1: Heart Disease).
Steps Performed

Data Preprocessing:
Loaded heart.csv and standardized numerical features.
Saved cleaned dataset as Heart_Disease_Cleaned.csv.


Exploratory Data Analysis:
Generated summary statistics and class distribution plot.
Created a correlation matrix for key features.


Decision Tree Classifier:
Trained a decision tree and visualized it using Graphviz.
Analyzed overfitting by varying max_depth and optimized with max_depth=3.


Random Forest Classifier:
Trained a random forest and compared accuracy with the decision tree.
Evaluated feature importances.


Cross-Validation:
Performed 5-fold cross-validation for both models to assess stability.



Files

heart_disease_decision_trees.ipynb: Jupyter Notebook with preprocessing, EDA, and model implementation.
heart.csv: Original Heart Disease Dataset.
Heart_Disease_Cleaned.csv: Preprocessed dataset.
class_distribution.png: Bar plot of class distribution.
correlation_matrix.png: Correlation matrix heatmap.
decision_tree.png: Visualized decision tree.
depth_tuning.png: Train vs. test accuracy by tree depth.
feature_importances.png: Random forest feature importance plot.
interview_questions.md: Answers to provided interview questions.
README.md: This documentation file.

Tools Used

Python 3
Jupyter Notebook
Pandas
NumPy
Matplotlib
Seaborn
scikit-learn
Graphviz

How to Run

Clone this repository:git clone https://github.com/Amaljithuk/AI-ML INTERNSHIP-TASK5.git


Install required dependencies:pip install pandas numpy matplotlib seaborn scikit-learn jupyter graphviz


Install Graphviz for visualization:
Install Graphviz (sudo apt install graphviz on Linux, brew install graphviz on macOS, or download from https://graphviz.org/ for Windows).
Ensure Graphviz is in your system PATH.


Launch Jupyter Notebook:jupyter notebook


Open heart_disease_decision_trees.ipynb and run all cells to:
Generate the cleaned dataset (Heart_Disease_Cleaned.csv).
Save visualizations (class_distribution.png, correlation_matrix.png, decision_tree.png, depth_tuning.png, feature_importances.png).
Display model metrics and cross-validation results.



Observations

EDA: The dataset is balanced, with similar counts of target 0 and 1. Features like cp, thalach, and oldpeak correlate with target.
Decision Tree: Prone to overfitting with high depth; max_depth=3 improves generalization.
Random Forest: Outperforms decision tree in accuracy and stability due to ensemble learning.
Feature Importance: cp (chest pain type), thalach (max heart rate), and oldpeak (ST depression) are key predictors.
Cross-Validation: Random forest shows higher and more stable accuracy across folds.

Notes

The notebook suppresses warnings for cleaner output.
Graphviz is required for decision tree visualization; ensure it’s installed.
The cleaned dataset is suitable for classification tasks.
Visualizations and metrics provide insights into model performance and feature importance.

Submission
This repository is submitted for Task 5 of the Elevate AI & ML Internship, completed on July 1, 2025, within the 10:00 AM to 10:00 PM submission window.
