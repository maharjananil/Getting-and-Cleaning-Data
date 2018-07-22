

Firstly this describers the steps in order to give some information about the course project related to Getting and Cleaning Data.

#About Data Source:
Source DATA for course project is taken from Human Activity Recognition Using Smart-phones Data Set.
A full description is available at the site where the data was obtained:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 
Below is the link of data for the project:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

#About R script:
The unzip package doesn't work in R version 3.3.1 I got error as "package ‘unzip’ is not available (for R version 3.3.1)" 
download manually from the link https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
 and unzip to the data into working R directory into folder name HAR Dataset then :

File with R code "run_analysis.R" perform 5 following steps as per course project task:
1. Merging the training and the test sets to create one data set.
1.1 Reading files
1.1.1 Reading trainings tables
1.1.2 Reading testing tables
1.1.3 Reading feature vector
1.1.4 Reading activity labels
1.2 Assigning column names
1.3 Merging all data in one set
2. Extracting only the measurements on the mean and standard deviation for each measurement
2.1 Reading column names
2.2 Create vector for defining ID, mean and standard deviation
2.3 Making necessary subset from setAllInOne
3. Using descriptive activity names to name the activities in the data set
4. Appropriately labelling the data set with descriptive variable names
5. Creating a second, independent tidy data set with the average of each variable for each activity and each subject
5.1 Making second tidy data set
5.2 Writing second tidy data set in .txt file. i.e tidy.txt

#About variables:
x_train, y_train, x_test, y_test, subject_train and subject_test contain the data from the downloaded files.
x_data, y_data and subject_data merge the previous datasets to further analysis.
features contains the correct names for the x_data dataset, which are applied to the column names stored in.

