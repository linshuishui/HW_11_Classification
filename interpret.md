# HW - classification

Build classification models to predict credit risk, given imbalanced labels. Use:

1. [Resampling](#Resampling)
2. [Ensemble Learning](#Ensemble-Learning)

## Files

[Resampling Starter Notebook](Starter_Code/credit_risk_resampling.ipynb)

[Ensemble Starter Notebook](Starter_Code/credit_risk_ensemble.ipynb)

[Lending Club Loans Data](Resources/LoanStats_2019Q1.csv.zip)

## Instructions

### Resampling

Resample the LendingClub data, and feed it to logistic regression classifiers.

1. import csv as df.

2. Split into Training/Testing.

3. Scale both data sets using `StandardScaler`.

4. Use the provided code to run a Simple Logistic Regression:
    * Fit the model.
    * Calculate the `balanced accuracy score`.
    * Print the `confusion matrix`.
    * Print the `imbalanced classification report`.

Then:

1. Oversample using `Naive Random Oversampler` and `SMOTE`.

2. Undersample using the `Cluster Centroids`.

3. Over- and undersample using `SMOTEENN`.


For each of the above:

1. Train a `logistic regression classifier` on resampled data.

2. Calculate the `balanced accuracy score`.

3. Display the `confusion matrix`.

4. Print the `imbalanced classification report`.


Answer:

* Which model had the best balanced accuracy score?

* Which model had the best recall score?

* Which model had the best geometric mean score?

### Ensemble Learning

Train and compare two different ensemble classifiers to predict loan risk. Use the [Balanced Random Forest Classifier](https://imbalanced-learn.org/stable/references/generated/imblearn.ensemble.BalancedRandomForestClassifier.html) and the [Easy Ensemble Classifier](https://imbalanced-learn.org/stable/references/generated/imblearn.ensemble.EasyEnsembleClassifier.html). Read the docs to find code examples.

Start by:

1. Read data into df using the starter code.

2. Split data into training/testing.

3. Scale training/testing using the `StandardScaler`.


Then, for each model:

1. Train the model using the quarterly data from LendingClub in the `Resource` folder.

2. Calculate the balanced accuracy score.

3. Display the confusion matrix.

4. Generate a classification report using the `imbalanced_classification_report`.

5. For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.


Answer:

* Which model had the best balanced accuracy score?

* Which model had the best recall score?

* Which model had the best geometric mean score?

* What are the top three features?

### Submission

* Create Jupyter notebooks for the homework and host the notebooks on GitHub.

* Include a markdown that summarizes your homework and include this report in your GitHub repository.

* Submit the link to your GitHub project to Bootcamp Spot.
