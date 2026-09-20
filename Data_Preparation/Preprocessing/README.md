# Data Preprocessing

This folder contains the main data preprocessing work for the customer churn project.

## Work Completed

* Loaded and inspected the original dataset
* Checked missing values and blank strings
* Checked duplicate rows
* Checked invalid categorical values
* Checked impossible numerical values and outliers
* Corrected logical inconsistencies
* Encoded categorical variables using one-hot encoding
* Standardised continuous numerical variables
* Validated the processed data

The dataset contained 7,043 rows and 10 columns.

No missing values, blank strings, invalid categories or impossible numerical values were found. A total of 302 fully duplicated rows were retained because the dataset did not contain a unique customer ID.

A total of 260 logical conflicts were corrected. For these records, `MultipleLines` was changed to `No` when `PhoneService` was `No`.

## Main Files

* `data_preprocessing_pipeline.ipynb`: Complete preprocessing workflow
* `cleaned_dataset.csv`: Cleaned dataset before encoding and scaling
* `integrity_check_report.csv`: Results of the initial data integrity checks
* `preprocessing_summary.csv`: Summary of the transformations
* `post_transformation_validation.csv`: Final validation results
* `preprocessing_pipeline.joblib`: Saved preprocessing pipeline
