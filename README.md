# 🎛️ Task 16: Hyperparameter Tuning

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit_Learn-orange?logo=scikit-learn)

## 📖 Overview
**Task 16** explores Optimization. We used the **Titanic Dataset** to demonstrate how tuning hyperparameters can reduce overfitting and improve accuracy using `GridSearchCV`.

## ⚙️ Workflow
1.  **Baseline:** Trained a `RandomForestClassifier` with default settings.
2.  **Grid Design:** Tested combinations of:
    * `n_estimators`: [50, 100, 200]
    * `max_depth`: [None, 10, 20]
    * `criterion`: ['gini', 'entropy']
    * `min_samples_split`: [2, 5, 10]
3.  **Search:** Used `GridSearchCV` with 5-fold cross-validation.

## 📊 Results

| Model | Accuracy |
| :--- | :--- |
| **Default Random Forest** | 82.68% |
| **Tuned Random Forest** | **83.80%** |

*Note: The tuning improved accuracy by **+1.12%**. The best model used `entropy` with a `max_depth` of 10, which prevented the trees from growing too deep and memorizing noise.*

## 📂 Files
* [📓 Jupyter Notebook](./Task_16.ipynb)
