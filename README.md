Dataset
Human Activity Recognition Using Smartphones : http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Files
CodeBook.md a code book that describes the variables, the data, and any transformations or work that I performed to clean up the data

run_analysis.R performs the data preparation and then followed by the 5 steps required as described in the course project’s definition:

1. Merges the training and the test sets to create one data set.

2. Extracts only the measurements on the mean and standard deviation for each measurement.

3. Uses descriptive activity names to name the activities in the data set

4. Appropriately labels the data set with descriptive variable names.

5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

6. FinalData.txt is the exported final data after going through all the sequences described above.


CodeBook.md
A code book that describes the variables, the data, and transformations used to tidy the data.

FinalData
A text file containing the tidied data set. In order to view the data in R please use the following script: read.table("FinalData.txt", header=TRUE)

The code was written based on the instruction of this assignment
Read training and test dataset into R environment. Read variable names into R envrionment. Read subject index into R environment.

Merges the training and the test sets to create one data set. Use command rbind to combine training and test set
Extracts only the measurements on the mean and standard deviation for each measurement. Use grep command to get column indexes for variable name contains "mean()" or "std()"
Uses descriptive activity names to name the activities in the data set Convert activity labels to characters and add a new column as factor
Appropriately labels the data set with descriptive variable names. Give the selected descriptive names to variable columns
From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject. Use pipeline command to create a new tidy dataset with command group_by and summarize_each in dplyr package
