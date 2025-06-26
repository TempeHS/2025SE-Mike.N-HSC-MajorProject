# Project Title

SecureTrack Intruder Detection System.

## Description

From anonymized, labelled web-browsing data, SecureTrack predicts the probability that a certain session belongs to a particular user or not.

## Getting Started

### Dependencies

- Python 3.12
- The following dependencies (in requirements.txt):
  - numpy
  - matplotlib
  - pandas
  - scikit-learn
  - pickle
  - scipy
  - optuna
  - xgboost
  - eli5

### Installing

- No other installations

### Executing program

- How to run the program
- Run every notebook from top to bottom, in this order:
  - eda.ipynb
  - wrangling.ipynb
  - model_development.ipynb
- For new data:
  - Update train_sessions.csv

## Authors

Mike Nguyen
[@M1keNguy3n](https://github.com/M1keNguy3n)

## Version History

- 1.0.0
  - Added documentation to the README.md
  - Added a list of dependencies to requirements.txt
  - Added comments to notebooks.
- 0.3.4
  - Tested several approaches to handling unbalanced classes in a 2-class classification problem.
  - None of them worked, falling behind the baseline using only a vectorizer.
  - Added features only introduced more noised, which the model picked up, reducing the ROC AUC and average precision.
- 0.3.3
  - Removed some features, tuning them to better fit the positive class.
  - Slight improvment gained, yet still lower than the baseline.
- 0.3.2
  - Used engineered features for model training.
  - The new features added noise to the model, resulting in a dcrease in both ROC AUC and average precision.
  - Attempted resampling to mitigate class balances, which also failed to improve the model.
- 0.3.1
  - Imported some helper functions to streamline feature testing.
  - Make my first submission to the competition, with a leaderboard score of 0.91516.
  - From the fitted model, feature importances were extracted and visualized using eli5.
  - Hyperparameter optimization was implemented.
- 0.3.0
  - Make intial commit for model development.
  - Examine a range of different models and their performance.
  - LogisticRegressor was chosen as the final model for furthur development.
- 0.2.4
  - Changed the implementation of the vectorizer.
  - The new implementation converts site_IDs to URLs, making features more legible in model development.
- 0.2.3
  - Added a sprint review.
  - Exported tranformed train and test datasets to seperate files.
- 0.2.2
  - Reduced the number of added features due to overfitting.
  - Seperated scaled features from other features, as the transformations needs to be done seperately on the train and test sets.
- 0.2.1
  - Feature Engineering pipelines established.
  - Temporal and session-related features added.
  - Sequence frequency features added.
- 0.2.0
  - Added an agile artifact for sprint 2.
- 0.1.2
  - Added an explanation of the dataset.
- 0.1.1
  - Added a sprint review.
- 0.1.0
  - Exploratory Data Analysis

## License

This project is licensed under the GNU General Public License v3.0 - see the LICENSE.md file for details

## Acknowledgments

[Yury Kashnitsky's community prediction competition - Catch Me If You Can ("Alice")](https://www.kaggle.com/competitions/catch-me-if-you-can-intruder-detection-through-webpage-session-tracking2/overview)

[Yury Kashnitsky's notebook - Model validation in a competition.](https://www.kaggle.com/code/kashnitsky/model-validation-in-a-competition)

[Tim Nikitin's notebook - Using pipelines for faster feature testing](https://www.kaggle.com/code/artnikitin/using-pipelines-for-faster-feature-testing)

[Scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html)
