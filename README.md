Getting_Cleaning_Data
=====================
The R script named "run_analysis.R" will perform the following actions in order to clean the data and obtain a tidy data set:

Data Merging: Combination of the training set and the test set in one single data set, namely train/X_train.txt with test/X_test.txt, the result of which is a data frame with activity IDs. The R script reads features.txt and extracts only the measurements on the mean and standard deviation for each measurement. It also reads activity_labels.txt and applies descriptive activity names to name the activities in the data set:

sitting standing laying walking walkingupstairs walkingdownstairs

Labeling: The R script labels the data set with descriptive names and it merges the data frame containing features with 10299x1 data frames containing activity labels and subject IDs. The result is saved as merged_clean_data.txt. The first column contains subject IDs, the second column activity names, and the last Columns are measurements.

Tidy Data set: At the end, the script creates a 2nd, independent tidy data set with the average of each measurement for each activity and each subject. The result is saved as tidy_data.txt.

Columns:

subject IDs
activity names
averages for each of the attributes. There are 30 subjects and 6 activities. We will get 180 rows in this data set with averages.
Source of the original data: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Original description: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
