Code Book
=================
This code book summarizes the resulting data fields in tidy.txt. Information pertaining to the description of variables in the "Measurements" section is sourced from the "features_info.txt" downloaded as part of the assignment.

The script performeds the following functions, as also mentioned in the README.txt file:

    (1) Downloads the dataset if it does not already exist.
    (2) Loads the activity and feature information
    (3) Loads both the training and test datasets, and keeps only the columns which contain0 mean or standard deviation data
    (4) Loads the activity and subject data for each dataset, and merges those columns with the dataset
    (5) Merges datasets created in  (3) and (4)
    (6) Converts the activity and subject columns into factors
    (7) Creates a tidy dataset that consists of the mean values for each variable for each subject and activity combination.

The end result is shown in the file tidy_data.txt.

Identifiers
=================
    subject - ID of the test subject
    activity - The type of activity performed when the measurements were taken

Measurements
=================
Feature Selection 


The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

tBodyAcc-XYZ
tGravityAcc-XYZ
tBodyAccJerk-XYZ
tBodyGyro-XYZ
tBodyGyroJerk-XYZ
tBodyAccMag
tGravityAccMag
tBodyAccJerkMag
tBodyGyroMag
tBodyGyroJerkMag
fBodyAcc-XYZ
fBodyAccJerk-XYZ
fBodyGyro-XYZ
fBodyAccMag
fBodyAccJerkMag
fBodyGyroMag
fBodyGyroJerkMag

The set of variables that were estimated from these signals are: 

mean(): Mean value
std(): Standard deviation


Additional vectors obtained by averaging the signals in a signal window sample. These are used on the angle() variable:

gravityMean
tBodyAccMean
tBodyAccJerkMean
tBodyGyroMean
tBodyGyroJerkMean

The complete list of variables of each feature vector is available in 'features.txt'

Activity Labels
=================
    WALKING (value 1): subject walking during the test
    WALKING_UPSTAIRS (value 2): subject walking up a stairs during test
    WALKING_DOWNSTAIRS (value 3): subject walking down a stairs during test
    SITTING (value 4): subject sat during test
    STANDING (value 5): subject stood during test
    LAYING (value 6): subject was laying down during the test
