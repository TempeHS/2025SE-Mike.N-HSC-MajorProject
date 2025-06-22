# Agile Artifact 2

**Sprint Backlog**

1. Feature Engineering

- [x] Temporal Features
- [x] Session-related Features
- [x] Bag-of-Words : Frequency of URLs

**Increment**

1. Utilize insights from exploratory data analysis to create features.
2. Develop a feature engineering pipeline for fast development and evaluation.

**Sprint Review**

Due to the extreme class imbalances, certain added features led to overfitting when using a base XGBClassifer model. Only some of the features explored in the EDA phase were added to the final train/test data. The Bag-of-Words approach made the train/test sets sparse matrixes, which greatly increase the difficulty in inspecting the quality of transformation processes. To mitigate this, two pipelines were implemented to isolate the vectorizer. This ensure that features can be implemented quickly, while maintaining data purity.

