# Student Performance Predictor — Multiple Linear Regression

## What this project does
Predicts student final grades (G3) using Multiple Linear 
Regression built with Sklearn on the UCI Student Performance 
dataset (395 students, 5 features).

## Concepts demonstrated
- Simple and Multiple Linear Regression with Sklearn
- Normalization using StandardScaler
- Train-Test Split (80/20)
- Manual p-value calculation with Scipy
- Adjusted R-squared calculation
- Feature Selection using backward elimination
- Real student grade prediction

## Key findings
- Grade2 is by far the strongest predictor — removing it 
  drops R² by 9%
- Study time has almost zero independent effect once 
  Grade2 is known
- Past failures turned out to add noise — removing it 
  slightly improved R²
- Model explains 78.2% of grade variability (R² = 0.7822)
- Predicted grade for a typical student: 12.71/20

## Model performance
| Metric | Value |
|--------|-------|
| R-squared | 0.7822 |
| Adjusted R-squared | 0.7673 |
| Difference | 0.0149 (small — all features helped) |

## Tools used
Python · Pandas · NumPy · Sklearn · Scipy · Matplotlib · Seaborn

## How to run
pip install pandas numpy scikit-learn scipy matplotlib seaborn
jupyter notebook notebooks/student_performance_sklearn.ipynb
