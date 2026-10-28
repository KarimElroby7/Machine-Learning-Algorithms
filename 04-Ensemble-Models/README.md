# 04 – Ensemble Models

Same loan approval dataset as `03-Decision-Trees`, so results can be compared directly with a single tree (0.92).

| Notebook | Description | Result |
|---|---|---|
| [random_forest](random_forest.ipynb) | scikit-learn `RandomForestClassifier` | Test accuracy 0.93 |
| [random_forest_from_scratch](random_forest_from_scratch.ipynb) | Bootstrap sampling + random feature subsets + majority vote, built on the from-scratch tree | 0.92 vs 0.93 (scikit-learn) |
| [ensemble_models](ensemble_models.ipynb) | Bagging vs boosting (AdaBoost, Gradient Boosting, XGBoost) vs stacking, plus 5-fold CV | Best: XGBoost, CV 0.934 |

**Key ideas:** bias–variance trade-off, bagging, boosting, stacking, K-fold cross-validation.
