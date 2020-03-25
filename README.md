# Random Forest Grid Search Example
This Jupyter Notebook performs grid search of hyperparameters for random forests to find the best hyperparameters.  The data could stand a lot of feature engineering to better good predictions but I did not do that.  The purpose of this Notebook is to demonstrate how to do grid search for random forests.  If you decide to do feature engineering and get better results, please share!

# This Jupyter Notebook performs multiple processes
1. Import train/test and validation census data files
2. Use random forest with default parameters to predict income for each row, then run model against validation dataset
3. Perform grid search for multiple hyperparameters to determine which create hyperparameters best fit the data (produce highest accuracy)
4. Use random forest with optimal parameters determined from grid search to predict income for each row

# Files
The files used for analysis came from https://archive.ics.uci.edu/ml/datasets/Census+Income
* The original file from UCI named adult.test has 16,281 records.
* I renamed adult.test to adult_data_small...
* I changed all categorical fields with text to categorical with integers
* I manually split this file into 2 files.  One for train/test and one for validation:
  * adult_data_small_train_test has 14,500 records
  * adult_data small_val has 1,781 records


The original file from UCI named adult.data has 32,561 records
* I renamed adult.data to adult_data_large...
* I changed all categorical fields with text to categorical with integers
* I manually split this file into 2 files.  One for train/test and one for validation:
  * adult_data_large_train_test has 29,000 records
  *adult_data_large_val has 3,561 records

# General Notes
* I used the small files in the interest of run time.  The same process can be run using the large files.


