# Random_Forest_Grid_Search
Script to perform grid search of hyperparameters for random forests

# This Jupyter Notebook performs multiple processes
1. Import train/test and validation census data files
2. Use random forest with default parameters to predict income for each row, then run model against validation dataset
3. Perform grid search for multiple hyperparameters to determine which create hyperparameters best fit the data (produce highest accuracy)
4. Use random forest with optimal parameters determined from grid search to predict income for each row

#H1 Files
# The original file from UCI named adult.test has 16,281 records
# https://archive.ics.uci.edu/ml/datasets/Census+Income
# Renamed adult.test to adult_data_small...
# Changed all categorical fields with text to categorical with integers
# Manually split this file into 2 files.  One for train/test and one for validation
# adult_data_small_train_test has 14,500 records
# adult_data small_val has 1,781 records


# The original file from UCI named adult.data has 32,561 records
# https://archive.ics.uci.edu/ml/datasets/Census+Income
# Renamed adult.data to adult_data_large...
# Changed all categorical fields with text to categorical with integers
# Manually split this file into 2 files.  One for train/test and one for validation
# adult_data_large_train_test has 29,000 records
# adult_data_large_val has 3,561 records
