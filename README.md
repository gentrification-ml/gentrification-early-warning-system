# Gentrification Early Warning System Using Machine Learning

## 1. Project Overview

The Gentrification Early Warning System is a machine learning project designed to identify areas that may be at risk of gentrification using socioeconomic, housing, and demographic data.

The project compares different machine learning algorithms and evaluates their performance in predicting gentrification risk.

## 2. Objectives

- Identify areas with potential gentrification risk.
- Analyse socioeconomic and housing-related indicators.
- Compare the performance of multiple machine learning models.
- Improve prediction using engineered features.
- Demonstrate predictions through an interactive input-based system.

## 3. Features Used

The model uses the following original features:

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

Two additional features are calculated from the original data:

- **Home Value-to-Income Ratio:** Median home value divided by median household income.
- **Annual Rent-to-Income Ratio:** Annualised median gross rent divided by median household income.

These features help represent housing affordability in relation to income.

## 4. Machine Learning Models

The project compares the following algorithms:

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

The models are evaluated using the original features and the enhanced feature set.

## 5. Model Evaluation

The notebook uses the following evaluation methods:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion matrices
- ROC curves
- Feature importance analysis

## 6. Interactive Prediction

The notebook includes a live prediction demo. Users enter socioeconomic and housing-related values, and the system calculates the engineered features automatically before predicting the gentrification risk.

The prediction indicates a model-estimated risk, not a guarantee that gentrification will occur.

## 7. Technologies Used

- Python
- Google Colab / Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn

## 8. How to Run the Project

1. Open the notebook in Google Colab.
2. Upload or connect the required dataset.
3. Ensure the dataset filename and path match the notebook code.
4. Run the notebook cells in order.
5. Review the model evaluation results.
6. Run the interactive prediction demo and enter the required inputs.

## 9. Project Structure

- `Gentrification_Early_Warning_System_DEMO_READY.ipynb` — Main notebook containing data processing, feature engineering, model training, evaluation, and the live demo.
- `balanced_training_dataset.csv` — Dataset used for training and evaluation, if included in the repository.

*Note: Actual filenames may differ from those listed above.*

## 10. Reference Research

This project is informed by the research paper:

**A Proximity-Based Early Warning System for Gentrification in California** — Aakash Pattabi (2018).

The project explores a machine learning approach using socioeconomic and housing indicators, with two engineered affordability-related features as an extension.

## 11. Limitations

Predictions depend on the quality and representativeness of the dataset. The model identifies statistical patterns and should not be interpreted as definitive proof of future gentrification.
