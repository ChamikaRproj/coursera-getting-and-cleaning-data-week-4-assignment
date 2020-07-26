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
