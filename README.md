# Gentrification Early Warning System Using Machine Learning

## 1. Project Overview

The **Gentrification Early Warning System** is a machine learning project that aims to identify areas that may be at risk of gentrification using demographic, socioeconomic, and housing-related indicators.

The project compares multiple machine learning algorithms and investigates whether engineered housing affordability features improve prediction performance. It also includes an interactive prediction demo.

## 2. Objectives

- Identify areas with potential gentrification risk.
- Analyse socioeconomic, demographic, and housing indicators.
- Compare the performance of different machine learning algorithms.
- Evaluate the effect of engineered affordability features.
- Demonstrate predictions using user-provided input values.

## 3. Dataset and Features

The dataset contains socioeconomic and housing-related indicators used to train and evaluate the classification models.

### Original Features

1. Total population
2. Median household income
3. Median gross rent
4. Median home value
5. Percentage with higher education
6. Poverty rate
7. Vacancy rate
8. Unemployment rate
9. Percentage of renter-occupied housing

### Engineered Features

The project introduces two additional features:

- **Home Value-to-Income Ratio:** Median home value divided by median household income.
- **Annual Rent-to-Income Ratio:** Annualised median gross rent divided by median household income.

These features represent housing costs relative to household income.

The notebook compares models using the original nine features and the enhanced eleven-feature set.

## 4. Machine Learning Models

The following algorithms are compared:

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

The notebook includes data preprocessing, model training, and performance evaluation.

## 5. Model Evaluation

Model performance is examined using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion matrices
- ROC curves
- Feature importance analysis, where applicable

These metrics help evaluate both overall classification performance and the models' ability to identify positive gentrification labels.

## 6. Interactive Prediction Demo

The notebook includes an input-based prediction demo. Users provide socioeconomic and housing-related values, and the system calculates the engineered features before generating a prediction.

The output represents a model-estimated risk based on the training data. It is not a guarantee that gentrification will occur.

## 7. Technologies Used

- Python
- Google Colab / Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn

## 8. Setup and Execution

### Requirements

- A Google account to use Google Colab, or a local Jupyter Notebook environment.
- The project notebook.
- The dataset file `balanced_training_dataset.csv`.
- The Python libraries required by the notebook.

### Running in Google Colab

1. Open the project notebook in Google Colab.
2. Make the dataset `balanced_training_dataset.csv` available to the notebook.
3. Check the dataset-loading cell and ensure the file path matches the location of the dataset.
4. Install any missing dependencies if the notebook does not already install them.
5. Run the notebook cells in order.
6. Review the evaluation metrics, confusion matrices, ROC curves, and feature importance results.
7. Execute the interactive prediction section and provide the required input values.

**Important:** The dataset must be loaded using the path expected by the notebook. If the notebook uses Google Drive, upload the dataset there and update the path as needed.

## 9. Project Structure

The repository contains the project notebook, dataset, and README.

- `README.md` — Project overview, methodology, and execution instructions.
- `balanced_training_dataset.csv` — Dataset used by the notebook.
- `Gentrification_Early_Warning_System_DEMO_READY.ipynb` — Main notebook for preprocessing, feature engineering, model training, evaluation, and prediction demo.

The notebook filename above should be updated if the actual filename in the repository differs.

## 10. Reference Research

**A Proximity-Based Early Warning System for Gentrification in California** — Aakash Pattabi (2018).

This research provides background for the project's early-warning approach. The current project uses socioeconomic and housing indicators with engineered affordability-related features. It should not be considered a reproduction of the reference paper's complete methodology.

## 11. Limitations

- Predictions depend on the quality and representativeness of the available dataset.
- The model identifies statistical patterns and does not establish that gentrification will occur.
- Performance metrics should be interpreted alongside class distribution and minority-class results.
- The engineered affordability ratios do not capture every factor influencing gentrification.
- Further validation on independent, geographically and temporally distinct data would be needed before real-world use.

## 12. Conclusion

This project demonstrates how machine learning can be applied to the early identification of potential gentrification risk using socioeconomic and housing indicators. By comparing multiple classifiers and testing engineered affordability features, the project provides a prototype for further research and development.
