# Agile Artifact 3

**Sprint Backlog**

1. Model Development

- [x] Implement baseline classifiers (Logistic Regression, Random Forest, etc.)
- [x] Split data using TimeSeriesSplit for validation
- [x] Evaluate models using ROC AUC and other metrics
- [x] Visualize ROC curves for model comparison
- [x] Choose 1 model, providing reasoning
  - [x] Baseline Submission
- [x] Hyperparameter optimization
- [x] Final model training & fitting
- [x] Submission

**Increment**

1. Establish a robust baseline for model performance using multiple classifiers.
2. Develop a reproducible workflow for model training, validation, and evaluation.

**Sprint Review**

Using a few helper functions, we streamlined the training, validation and evaluation processes. We implemented 7 different approaches to improve the model's performance, addressed issues with the dataset and various remedies, tackled problems with the model that led to underfitting and overfitting. The best performing model is the baseline, which is a LogisticRegression relying on a vectorizer to implement website visit frequencies as features to predict probabilities.
