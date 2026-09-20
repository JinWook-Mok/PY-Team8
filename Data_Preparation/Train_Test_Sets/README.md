# Training and Testing Sets

This folder contains the processed training and testing datasets.

The cleaned dataset was divided using an 80:20 stratified split.

* Training set: 5,634 records
* Testing set: 1,409 records
* Target variable: `Churn`
* Churn rate in the full dataset: 26.54%
* Churn rate in the training set: 26.54%
* Churn rate in the testing set: 26.54%
* Random state: 42

Stratification was used to preserve the churn proportion in both datasets. The fixed random state ensures that the same split can be reproduced.

## Files

* `X_train_processed.csv`: Processed input features for training
* `y_train.csv`: Churn target values for training
* `X_test_processed.csv`: Processed input features for testing
* `y_test.csv`: Churn target values for testing
* `train_test_split_summary.csv`: Summary of the dataset split

The preprocessing pipeline was fitted only on the training data. The fitted pipeline was then used to transform the testing data. This process prevents data leakage.
