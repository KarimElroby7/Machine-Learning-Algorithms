# 03 – Decision Trees

Both notebooks use the **loan approval** dataset (45,000 applications, imbalanced target).

| Notebook | Description | Result |
|---|---|---|
| [loan_approval_decision_tree](loan_approval_decision_tree.ipynb) | EDA, encoding, depth-limited `DecisionTreeClassifier`, tree visualization | Test accuracy 0.92 |
| [decision_tree_from_scratch](decision_tree_from_scratch.ipynb) | Recursive tree built on entropy / information gain in NumPy vs scikit-learn | 0.90 vs 0.90 |

**Key ideas:** entropy, information gain, recursive splitting, controlling overfitting with `max_depth` / `min_samples_split`.
