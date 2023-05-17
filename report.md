## Overview of Analysis

The purpose of this analysis is to develop a classifier that can accurately predict which applicants applying for funding, have the best chance of success in their ventures.  To complete the analysis, we utilized a dataset of past organizations that have received funding from Alphabet Soup previously.  

## Results

* Preprocessing
    - the target variable for the model is the 'IS_SUCCESSFUL column, which tells us if the funding received was used effectively
    - the feature variable for the model is all columns in the data set besides the target variable (IS_SUCCESSFUL)
    - we removed the 'EIN' and 'NAME' columns, as they did not provide us with any info that could be used for the analysis

* Compile, Train, and Evaluate the Model
    - the model had an accuracy score of 72.69% on the test data, and a loss of .5520
    - to improve the accuracy of the model, we binned low-frequency values in the 'APPLICATION_TYPE' and 'CLASSIFICATION' columns, as well as standardized the data with StandardScaler.

## Summary

The deep learning model ultimatelty achieved an accuracy score of 72.69% to predict the success applicants will have with funding they received for their business ventures.  Now, this is not a terrible reading, however, further steps can be taken to improve the accuracy of this model. To improve the classifcation accuracy, we could have deployed a RandomForest classifier.

In conclusion, while the model is not too bad for predicting these successes, alternative methods should be used to better predict, and find the best performing model. 