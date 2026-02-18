# Predicting Wine Quality with Machine Learning

This project predicts wine **quality** from physicochemical lab measurements (acidity, sugar, chlorides, alcohol, etc.). The notebook compares several regression models and reports cross-validation metrics (RMSE and R²) for red and white wines.

## Dataset
- Source: UCI Machine Learning Repository (Wine Quality dataset)
- Target: `quality`
- Features: physicochemical measurements (and wine type when combining red + white)

The notebook pulls the dataset using `ucimlrepo` (no manual download needed).

## What’s in this repo
- `AA1_500_Team_4_Final_Project.ipynb`  Full workflow: load data, prep, train, evaluate
- `README.md`  Project overview + run instructions

## Models evaluated
- Dummy baseline (mean predictor)
- Linear Regression
- Ridge, Lasso
- Random Forest Regressor
- Gradient Boosting Regressor
- Support Vector Regression (SVR)

## Results
Run the notebook to reproduce results. After you run it once, copy your final CV metrics into the tables below.

### Red wine (cross-validation)
| Model | CV RMSE (mean) | CV RMSE (std) | CV R² (mean) |
|---|---:|---:|---:|
| Random Forest |  |  |  |
| Gradient Boosting |  |  |  |
| Ridge |  |  |  |
| Lasso |  |  |  |
| Linear Regression |  |  |  |
| SVR |  |  |  |
| Dummy (mean) |  |  |  |

### White wine (cross-validation)
| Model | CV RMSE (mean) | CV RMSE (std) | CV R² (mean) |
|---|---:|---:|---:|
| Random Forest |  |  |  |
| Gradient Boosting |  |  |  |
| Ridge |  |  |  |
| Lasso |  |  |  |
| Linear Regression |  |  |  |
| SVR |  |  |  |
| Dummy (mean) |  |  |  |

## Quick start (local)

```bash
git clone https://github.com/jazz1416/Predicting-Wine-Quality-with-Machine-Learning.git
cd Predicting-Wine-Quality-with-Machine-Learning

python -m venv .venv

# macOS/Linux:
source .venv/bin/activate
# Windows (PowerShell):
# .\.venv\Scripts\Activate.ps1

python -m pip install -U pip
python -m pip install numpy pandas matplotlib seaborn scikit-learn ucimlrepo jupyter

jupyter notebook AA1_500_Team_4_Final_Project.ipynb


## Notes
- Results can vary slightly depending on random seeds and library versions.
- Next step: hyperparameter tuning (GridSearchCV/RandomizedSearchCV) for Random Forest, Gradient Boosting, and SVR.

## Reference
Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009). Modeling wine preferences by data mining from physicochemical properties. *Decision Support Systems*.


