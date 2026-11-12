# Diabetes Prediction Using Machine Learning

## Project Overview

This project develops and compares machine learning classification models to predict diabetes based on demographic, lifestyle, clinical, and environmental factors.

## Dataset

- **Observations:** 1,879 patient records
- **Original features:** 45 predictors
- **Target variable:** `Diagnosis` (0 = No Diabetes, 1 = Diabetes)
- **Missing values:** None

## Methodology

1. **Exploratory Data Analysis:** Examined feature distributions and relationships using statistical summaries and visualizations.
2. **Data Preprocessing:** Removed `PatientID` and `DoctorInCharge`, standardized input features using StandardScaler, and split the data into training and testing sets (80:20).
3. **Model Development:** Trained five classification algorithms:
   - Logistic Regression
   - Decision Tree
   - Random Forest
   - Gradient Boosting
   - AdaBoost
4. **Model Evaluation:** Compared model performance using accuracy, precision, recall, F1-score, and ROC-AUC.

## Results

| Model               | Accuracy | Precision |  Recall | F1-score | ROC-AUC |
| ------------------- | -------: | --------: | ------: | -------: | ------: |
| Logistic Regression |      84% |       80% |     76% |      78% |    0.90 |
| Decision Tree       |      88% |       85% |     81% |      83% |    0.86 |
| Random Forest       |      91% |       95% |     82% |      88% |    0.95 |
| Gradient Boosting   |  **94%** |       95% |     87% |  **91%** |    0.95 |
| AdaBoost            |      93% |       91% | **89%** |      90% |    0.95 |

**Best Accuracy:** Gradient Boosting (94%)

## Technologies Used

- Python
- NumPy and Pandas
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook / Kaggle

## Future Improvements

- Feature importance and interpretability analysis.
- Hyperparameter tuning and cross-validation.
- Confusion matrix and additional diagnostic evaluation.
- Improved preprocessing and leakage-free model evaluation.

##
