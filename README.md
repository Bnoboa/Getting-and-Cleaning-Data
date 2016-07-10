# Getting-and-Cleaning-Data
Repository for Week 4 of the Getting and Cleaning Data course on Coursera
Getting and Cleaning Data Coursera course project. The R script, run_analysis.R, does the following:

    (1) Downloads the dataset if it does not already exist.
    (2) Loads the activity and feature information
    (3) Loads both the training and test datasets, and keeps only the columns which contain0 mean or standard deviation data
    (4) Loads the activity and subject data for each dataset, and merges those columns with the dataset
    (5) Merges datasets created in  (3) and (4)
    (6) Converts the activity and subject columns into factors
    (7) Creates a tidy dataset that consists of the mean values for each variable for each subject and activity combination.

The end result is shown in the file tidy_data.txt.