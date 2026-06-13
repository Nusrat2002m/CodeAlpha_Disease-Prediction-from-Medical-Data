# Disease-Prediction-from-Medical-Data

## Files

| File | Task | Dataset | Models |
|---|---|---|---|
| `task4_disease_prediction.py` | Disease Prediction (Breast Cancer) | scikit-learn Breast Cancer Wisconsin dataset | Logistic Regression, Random Forest, SVM, Gradient Boosting |

## How to run

```bash
python3 task4_disease_prediction.py
```
All required libraries (`numpy`, `pandas`, `scikit-learn`, `matplotlib`)
are standard and install with:

```bash
pip install numpy pandas scikit-learn matplotlib
```
## Important honesty notes (please read before submitting)

**(Disease Prediction):** Uses the Breast Cancer Wisconsin
   dataset (built into scikit-learn, one of the datasets explicitly
   suggested in the brief). XGBoost was not installed in this environment,
   so Gradient Boosting (scikit-learn's native equivalent) is used as the
   4th algorithm alongside Logistic Regression, Random Forest, and SVM —
   all four reach 95–98% accuracy with ROC-AUC > 0.99.

## Results summary (from the runs in this environment)

- **Disease Prediction:** Logistic Regression and SVM tied for
  best performance (98.2% accuracy, ROC-AUC ~0.995). `worst perimeter`,
  `worst area`, and `worst concave points` were the top predictive
  features — matching established medical literature on tumor
  malignancy indicators.

## Risks / limitations to be aware of

- All accuracy numbers will vary slightly between runs unless random
  seeds are fixed (they are, here, via `random_state=42`).  
   
