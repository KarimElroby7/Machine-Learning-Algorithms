# Datasets

All notebooks read their data from this folder using relative paths (`../data/<file>.csv`).

| File | Used in | Rows | Description |
|------|---------|------|-------------|
| `homeprices.csv` | 01 – house prices | 5 | Toy dataset: house area vs price |
| `Advertising.csv` | 01 – advertising sales | 200 | TV / Radio / Newspaper ad budgets vs Sales (ISLR) |
| `car_purchasing.csv` | 01 – linear regression from scratch | 500 | Customer age, salary, debt, net worth vs car purchase amount |
| `train_energy_data.csv`, `test_energy_data.csv` | 01 – energy consumption | 1000 / 100 | Building type, size, occupants, appliances, temperature vs energy consumption |
| `Heart_Disease_Prediction.csv` | 02 – logistic regression | 270 | Clinical features vs presence of heart disease |
| `loan_data.csv` | 03, 04 – trees & ensembles | 45,000 | Applicant profile vs loan approval status |
| `IMDB Dataset.csv` | 05 – naive bayes | 50,000 | Movie reviews labelled positive / negative |
| `Live.csv` | 07 – facebook live clustering | 7,050 | Facebook Live sellers in Thailand – post engagement (UCI) |
| `wine-clustering.csv` | 07 – wine clustering | 178 | Chemical analysis of wines (unlabelled) |
| `titanic_train.csv` | 08 – SVM | 891 | Kaggle Titanic passenger data |

The Iris dataset used in `06-KNN` is loaded directly from `sklearn.datasets`.

## Not included

`IMDB Dataset.csv` (~66 MB) is not committed because of its size.
Download it from Kaggle – [IMDB Dataset of 50K Movie Reviews](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews) – and place it in this folder.
