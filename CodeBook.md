Overview
This codebook describes the variables, the data, and performed to clean up the data for ‘Human Activity Recognition Unsing Smartphones Data Set’. 

Data source
This dataset is derived from the "Human Activity Recognition Using Smartphones Data Set" which was originally made available here: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Variables:
•	x_train, y_train, x_test, y_test, subject_train and subject_test contain the data from the downloaded files.
•	x_data, y_data and subject_data merge the previous datasets to further analysis.
•	features contains the correct names for the x_data dataset, which are applied to the column names stored in

Work:
The run_analysis.R script does the following:
0. Downloading dataset
Unzip dataSet to /data directory
1. Merging the training and the test sets to create one data set:

1.1 Reading files

1.1.1 Reading trainings tables:

1.1.2 Reading testing tables:

1.1.3 Reading feature vector:

1.1.4 Reading activity labels:

1.2 Assigning column names:

1.3 Merging all data in one set:

2. Extracting only the measurements on the mean and standard deviation for each measurement

2.1 Reading column names:

2.2 Create vector for defining ID, mean and standard deviation:

2.3 Making nessesary subset from setAllInOne:

3. Using descriptive activity names to name the activities in the data set:

4. Appropriately labeling the data set with descriptive variable names.

This step was made in previos steps See 1.3, 2.2, 2.3.

5. Creating a second, independent tidy data set with the average of each variable for each activity and each subject:

5.1 Making second tidy data set

5.2 Writing second tidy data set in txt file


