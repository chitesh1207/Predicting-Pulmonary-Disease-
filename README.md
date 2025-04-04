# Predicting Pulmonary Disease Using Machine Learning

This repository supports the coursework for the 7072CEM Machine Learning module at Coventry University by Chitesh Kumar Bedapudi. The project applies machine learning to classify pulmonary disease (YES/NO) using a 5000-sample dataset, achieving accuracies of 92% (XGBoost), 90% (Random Forest), and 88% (SVM). It’s documented in a scientific paper and viva video submitted on 7 April 2025.

## Project Overview
- **Objective**: Classify pulmonary disease presence and identify key predictors (e.g., oxygen saturation, smoking history).
- **Methods**: Random Forest, SVM, and XGBoost with preprocessing (SMOTE, PCA, RFE, scaling).
- **Results**: XGBoost excels (92% accuracy, 0.94 ROC-AUC); see paper for details.
- **Significance**: Enhances early detection in healthcare, with ethical considerations (e.g., GDPR compliance).

## Repository Structure
- `data/`: Dataset (e.g., `pulmonary_data.csv`) or placeholder if not included.
- `preprocessing.py`: Data cleaning and feature engineering.
- `models.py`: Model training and prediction.
- `evaluation.py`: Performance metrics and confusion matrices.
- `visualizations.py`: EDA and result plots.
- `main.ipynb`: Full pipeline in one notebook.
- `requirements.txt`: Python dependencies.



---

### README 2: About Code Only

```markdown
# Code for Predicting Pulmonary Disease Using Machine Learning

This repository contains the Python code for the 7072CEM coursework by Chitesh Kumar Bedapudi, implementing machine learning models to classify pulmonary disease.

## Code Files
- `Predicting_Pulmonary_Disease_using_ML.ipynb`: 
  - Handles missing data (mean/mode imputation).
  - Encodes categorical features (Label/One-Hot).
  - Scales features (`StandardScaler`).
  - Balances classes (`SMOTE`).
  - Reduces dimensions (`PCA`) and selects features (`RFE`).
- `models`: 
  - Trains Random Forest (`RandomForestClassifier`).
  - Trains SVM (`SVC` with kernel trick).
  - Trains XGBoost (`XGBClassifier` with hyperparameter tuning).
- `evaluation`: 
  - Computes accuracy, precision, recall, F1-score (`sklearn.metrics`).
  - Generates ROC-AUC scores and confusion matrices.
- `visualizations`: 
  - Plots EDA (histograms, heatmaps via `seaborn`).
  - Visualizes results (ROC curves, probability distributions).
- `main`: 
  - Combines all steps: preprocessing, training, evaluation, and visualization.

## Dependencies
Listed in `requirements`:
- `scikit-learn`
- `xgboost`
- `imblearn`
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

## Running the Code
1. requirements
2. Execute: 
   - `jupyter notebook Predicting_Pulmonary_Disease_using_ML.ipynb` (full pipeline)

## Notes
- Assumes dataset (`Lung_Cancer_Dataset.csv`) in `data/`. If absent, adjust paths.
- Outputs match paper results (e.g., XGBoost accuracy: 92%).
