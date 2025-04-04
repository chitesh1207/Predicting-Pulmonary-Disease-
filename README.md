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

## Setup Instructions
1. **Clone**:
   ```bash
   git clone https://github.com/yourusername/pulmonary-disease-ml.git
   cd pulmonary-disease-ml
