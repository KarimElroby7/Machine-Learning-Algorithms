# 05 – Naive Bayes

| Notebook | Description | Result |
|---|---|---|
| [imdb_sentiment_naive_bayes](imdb_sentiment_naive_bayes.ipynb) | Sentiment analysis of 50k IMDB reviews: text cleaning → TF-IDF → Gaussian vs Multinomial Naive Bayes | Accuracy 0.81 (Gaussian) → 0.84 (Multinomial) |

> The IMDB dataset (~66 MB) is excluded by `.gitignore` – see [data/README.md](../data/README.md) for the download link.

**Key ideas:** Bayes' theorem, conditional independence assumption, TF-IDF text features.
