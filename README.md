# Used Cars Price Prediction

Capstone project — MIT Applied Data Science Program (via Great Learning).
Final submission score: **40 / 40**. Presented March 2025.

## Problem
Demand for used cars in the Indian market is growing, but prices are
uncertain and hard to predict — which makes profitable buying and reselling
a guessing game. This project builds a pricing model that predicts used-car
prices accurately, so a business can:
1. Set a maximum purchase price that stays profitable
2. Price resale cars within a reasonable, trust-building range
3. Target the right cars to the right buyer segments

## Dataset
Used-car listings for the Indian market, with attributes including:
- Year, kilometers driven, mileage, fuel and transmission type
- Engine and power specifications
- Asking price (target)

_Source: course-provided dataset (Great Learning)._

## Approach
1. **Data exploration & visualization** — univariate and bivariate analysis
   (scatter plots, heat maps, box plots)
2. **Feature engineering** — including log transform of kilometers driven
3. **Modeling** — compared Linear Regression, Ridge/Lasso Regression,
   Decision Tree, and Random Forest
4. **Hyperparameter tuning** — Decision Tree, Random Forest, and KNN
5. **Selection** — compared models on test R² and RMSE

## Results
- **Best model: Random Forest after hyperparameter tuning**
  — test R² **> 90%**, with relatively low RMSE on test data
- **Most important price drivers:** Power, Engine, Year,
  Transmission (manual), Mileage, log of kilometers driven
- **Business findings:**
  - Power and year relate positively to price — newer, higher-power cars
    resell higher
  - Automatic-transmission cars command higher prices and demand than
    manual — avoid buying manual cars for resale where possible

## Tools
Python · pandas · NumPy · scikit-learn · matplotlib / seaborn · Jupyter

## Repo contents
| File | What it is |
|---|---|
| `Capstone_Project_Reference_Notebook_Low_Code_Used_Cars_Price_Prediction.ipynb` | Full notebook: cleaning, EDA, modeling, tuning |
| `Used-Cars-Price-Prediction.pdf` | Final capstone report (submitted version) |
| `Live_Presentation_Slides_-_Used_Cars_Price_Prediction.pdf` | Capstone presentation deck |
| `data/` | Dataset or dataset notes |

## How to run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook
```
