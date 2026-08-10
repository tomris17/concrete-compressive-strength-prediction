# Concrete Compressive Strength Prediction & Classification

This project aims to predict the compressive strength of concrete based on its material components and age, as well as classify the concrete into structural application categories using traditional Machine Learning models and Deep Learning Neural Networks.

##  Project Overview
- **Regression Analysis:** Continuous prediction of concrete compressive strength (MPa) using 13 different ML algorithms and a Deep Learning model (ANN).
- **Classification Analysis:** Feature engineering to categorize concrete into classes (`non-structural`, `residential`, `commercial`, `high-strength`) and environmental feature encoding (`Green`), evaluated using an Artificial Neural Network.
- **Top Performer:** XGBoost Regressor achieved the best performance with an **$R^2$ score of 0.92**.

##  Dataset Features
The dataset (`Concrete_Data.xls`) contains parameters describing concrete mix designs:
- **Cement:** Kg in a $m^3$ mixture
- **Blast Furnace Slag:** Kg in a $m^3$ mixture
- **Fly Ash:** Kg in a $m^3$ mixture
- **Water:** Kg in a $m^3$ mixture
- **Superplasticizer:** Kg in a $m^3$ mixture
- **Coarse Aggregate:** Kg in a $m^3$ mixture
- **Fine Aggregate:** Kg in a $m^3$ mixture
- **Age:** Days (1–365)
- **Strength (Target):** Concrete compressive strength in MPa

##  Tools & Libraries
- **Language:** Python 3.x
- **Data Manipulation:** `pandas`, `numpy`
- **Machine Learning:** `scikit-learn`, `xgboost`
- **Deep Learning:** `tensorflow`, `keras`
- **Visualization:** `matplotlib`, `seaborn`

##  Key Results

### Regression Models Performance
| Model | $R^2$ Score | RMSE | MAE |
| :--- | :--- | :--- | :--- |
| **XGBoost Regressor** | **0.9230** | **4.45** | **2.90** |
| Gradient Boosting | 0.8808 | 5.54 | 4.09 |
| Deep Learning (ANN) | 0.8514 | 6.18 | - |
| Decision Tree | 0.8098 | 6.99 | 4.53 |
| Random Forest / Extra Trees | 0.7778 | 7.56 | 4.94 |
| Linear Regression | 0.6275 | 9.79 | 7.74 |

### Classification Performance
- **Neural Network Accuracy:** ~82.5% on multi-class concrete strength classification utilizing early stopping callbacks.

##  How to Run
1. Clone this repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/concrete-compressive-strength-prediction.git](https://github.com/YOUR_USERNAME/concrete-compressive-strength-prediction.git)
