# Machine Learning – Algorithms & Projects

A hands-on collection of classical machine-learning algorithms. Each algorithm is applied to a real dataset end to end (EDA → preprocessing → modelling → evaluation), and the core algorithms are also **implemented from scratch in NumPy** and checked against scikit-learn.

## Implemented from scratch

| Algorithm | Notebook | From scratch | scikit-learn |
|---|---|---|---|
| Linear Regression (gradient descent) | [linear_regression_from_scratch](01-Linear-Regression/linear_regression_from_scratch.ipynb) | R² 0.99999998 | R² 0.99999998 |
| Logistic Regression | [logistic_regression_from_scratch](02-Logistic-Regression/logistic_regression_from_scratch.ipynb) | Acc 0.85 | Acc 0.85 |
| Decision Tree (information gain) | [decision_tree_from_scratch](03-Decision-Trees/decision_tree_from_scratch.ipynb) | Acc 0.90 | Acc 0.90 |
| Random Forest (bagging + feature sampling) | [random_forest_from_scratch](04-Ensemble-Models/random_forest_from_scratch.ipynb) | Acc 0.92 | Acc 0.93 |
| K-Nearest Neighbours | [knn_from_scratch](06-KNN/knn_from_scratch.ipynb) | Acc 0.97 | Acc 0.97 |

## Projects

| # | Problem | Type | Dataset | Model(s) | Result |
|---|---|---|---|---|---|
| 01 | [Sales from advertising budgets](01-Linear-Regression/advertising_sales.ipynb) | Regression | Advertising (200) | Linear Regression | R² **0.90** |
| 01 | [Building energy consumption](01-Linear-Regression/energy_consumption.ipynb) | Regression | Energy (1,000) | Linear Regression | R² ≈ 1.0 (synthetic data) |
| 02 | [Heart disease prediction](02-Logistic-Regression/heart_disease_prediction.ipynb) | Binary classification | Heart Disease (270) | Logistic Regression | Acc **0.85**, recall 0.92 |
| 03 | [Loan approval](03-Decision-Trees/loan_approval_decision_tree.ipynb) | Binary classification | Loan data (45,000) | Decision Tree | Acc **0.92** |
| 04 | [Loan approval – random forest](04-Ensemble-Models/random_forest.ipynb) | Binary classification | Loan data (45,000) | Random Forest | Acc **0.93** |
| 04 | [Ensemble comparison](04-Ensemble-Models/ensemble_models.ipynb) | Binary classification | Loan data (45,000) | RF, AdaBoost, GBM, XGBoost, Stacking | XGBoost 5-fold CV **0.934** |
| 05 | [IMDB sentiment analysis](05-Naive-Bayes/imdb_sentiment_naive_bayes.ipynb) | NLP / text classification | IMDB (50,000) | TF-IDF + Naive Bayes | Acc **0.84** (MultinomialNB) |
| 07 | [Facebook Live engagement clustering](07-KMeans/facebook_live_clustering.ipynb) | Clustering | Facebook Live (7,050) | K-Means + PCA | Silhouette **0.89** (K=2) |
| 07 | [Wine clustering](07-KMeans/wine_clustering.ipynb) | Clustering | Wine (178) | K-Means + PCA | Silhouette **0.33** (K=4) |
| 08 | [Titanic survival](08-SVM/titanic_svm.ipynb) | Binary classification | Titanic (891) | SVM + GridSearchCV | Acc **0.82** |

## What's covered

- **Supervised learning:** linear & logistic regression, decision trees, random forest, boosting (AdaBoost, Gradient Boosting, XGBoost), stacking, Naive Bayes, KNN, SVM
- **Unsupervised learning:** K-Means, elbow method, silhouette score, PCA
- **Data preparation:** missing values, IQR outlier detection, one-hot / ordinal / label encoding, Standard & Robust scaling (fitted on the training set), text cleaning and TF-IDF
- **Evaluation:** MAE / RMSE / R², accuracy, precision, recall, F1, confusion matrix, K-fold cross-validation, hyperparameter tuning with `GridSearchCV`

## Repository structure

```
├── 01-Linear-Regression/
├── 02-Logistic-Regression/
├── 03-Decision-Trees/
├── 04-Ensemble-Models/
├── 05-Naive-Bayes/
├── 06-KNN/
├── 07-KMeans/
├── 08-SVM/
├── data/              # all datasets (see data/README.md)
└── requirements.txt
```

Every folder has its own README describing the notebooks inside it.

## How to run

```bash
git clone https://github.com/KarimElroby7/Machine-Learning-Algorithms.git
cd Machine-Learning-Algorithms
pip install -r requirements.txt
jupyter notebook
```

All datasets are in [`data/`](data/), except the IMDB reviews dataset (~66 MB), which is too large for the repo – the download link is in [data/README.md](data/README.md).
