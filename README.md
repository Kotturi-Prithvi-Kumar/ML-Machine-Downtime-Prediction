# 🏭 Machine Downtime Prediction

> Classification project predicting industrial machine downtime from operational data — so maintenance can happen before the breakdown, not after.

## The Problem
Unplanned machine downtime is expensive. Given operational/sensor readings, can we predict whether a machine is about to go down?

## The Data
Machine operational dataset (see `Data/`) with sensor and operating-condition features and a downtime event label.

## Approach
1. **EDA** — downtime rate, feature distributions for downtime vs normal operation, correlation with failure events.
2. **Feature engineering** — handling class imbalance (downtime is the rare class), scaling, encoding.
3. **Modeling** — train/test split; compared classifiers (e.g. Logistic Regression, Random Forest, XGBoost) with cross-validation; tuned for recall on the downtime class (missing a failure costs more than a false alarm).
4. **Evaluation** — accuracy, precision, recall, F1 and confusion matrix on the held-out test set.

## Key Results
- **Best model:** [fill in]
- **Test accuracy:** [fill in]% · **Recall (downtime class):** [fill in]
- **Strongest failure signals:** [fill in from your feature importances]

## Tech Stack
Python · Pandas · NumPy · Scikit-learn · Matplotlib · Seaborn · Jupyter

## Project Structure
```
├── Machine-Downtime-Prediction.ipynb   # Full workflow
└── Data/                               # Dataset
```

## How to Run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook Machine-Downtime-Prediction.ipynb
```
