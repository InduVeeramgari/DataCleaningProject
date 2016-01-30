
Getting and Cleaning Data Project
Run_Analysis.R

This is a  cleanup script (Run_Analysis.R) does the following:

Merges the training and the test sets to create one data set.
Extracts only the measurements on the mean and standard deviation for each measurement.
Uses descriptive activity names to name the activities in the data set
Appropriately labels the data set with descriptive activity names.
Creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Running the script
For both the test and train datasets, produce an interim dataset:
Extract the mean and standard deviation features (listed in CodeBook.md, section 'Extracted Features'). This is the values table.
Get the list of activities.
Put the activity labels (not numbers) into the values table.
Get the list of subjects.
Put the subject IDs into the values table.
Join the test and train interim datasets.
Put each variable on its own row.
Rejoin the entire table, keying on subject/acitivity pairs, applying the mean function to each vector of values in each subject/activity pair. This is the clean dataset.
Write the clean dataset to disk.
Cleaned Data
  
 