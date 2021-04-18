# Code Book for the new dataset (step5table.txt)  
 
## Source Data  

The original data used corresponds to the [Human Activity Recognition Using Smartphones Dataset v1.0](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones) that can be downloaded [here](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip).  

It was collected during experiments carried out with a group of 30 volunteers (ages 19-48 years) in which each person performed six activities wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, scientists captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments were video-recorded to label the data manually.   

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, were separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force was assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.   

The original dataset includes a 561-feature vector with time (t) and frequency (f) domain variables that includes different summaries and transformations (mean(), std(), mad(), max(), min(), sma(), energy(), etc.) of the signals measured in feature variables such as BodyAcc-XYZ, GravityAcc-XYZ, BodyAccJerk-XYZ, BodyGyro-XYZ, BodyGyroJerk-XYZ, BodyAccMag, etc., where "-XYZ"" is used to denote 3-axial signals in the X, Y and Z directions.  


## Variables  

**ACTIVITY** (1 column)  
- WALKING  
- WALKING_UPSTAIRS  
- WALKING_DOWNSTAIRS  
- SITTING  
- STANDING  
- LAYING  

**SUBJECT** (1 column)  
- An identifier of the subject who carried out the experiment  

**AVERAGE FEATURE VARIABLES** (66 columns)  
- The dataset includes the AVERAGE per ACTIVITY per SUBJECT for each feature variable which described the mean (mean()) and standard deviation (std()) of each XYZ signal of each measurement.  

 
## Transformations  

The major transformations performed to generate this dataset are:  

1) Merging the training and the test sets to create one data set.  
2) Extracting only the measurements on the mean and standard deviation for each measurement.   
3) Using descriptive activity names to name the activities in the data set  
4) Labeling the data set with descriptive variable names.   
5) Creating a second, independent tidy data set with the average of each variable for each activity and each subject. 

