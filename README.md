# Getting and Cleaning Data Course- Final Project  


## Documents included in the GettingAndCleaningDataCourseProject repository

1) CodeBook.md
2) run_analysis.R
3) step5table.txt

Each document is described below


## 1) Codebook.md

Describes the source data, variables, and transformations that were loaded and performed in the R script "run_analysis.R".


## 2) run_analysis.R

Includes all the code used to load, clean, transform and write the final data, which is contained in the text file "step5table.txt".
In summary, this script performs the following operations:


**Initial steps:**  
- load dplyr library  
- set working directory   

**To prepare tidy data set:**  
- Incorporate train and test data sets and combine them by row  
- Incorporate feature data to label variables in data  
- Select variables that include the mean() and std() features in the combined data set  
- Load and bind train and test activity label data, then match with class labels and replace with descriptive activity names  
- Load and bind train and test activity subject data  
- Create tidy data set by binding the activity label variable, subject variable, and the selected data set for mean and std variables  

**Clean global environment**  
- remove all objects except the tidy data  

**Create second independent data set**  
- create data set with the average of each variable for each activity and each subject and adding the string "average" at the beginning of each modified variable name  
- write a txt file with the second data set  


## 3) step5table.txt

The final dataset that includes the variables activity, subject, and summary feature variables the indicate the average per activity per subject of specific measurements.

