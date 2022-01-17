# Neural Network Charity Analysis

## Overview of Project

The purpose of this project is to create a a binary classifier that is capable of predicting whether applicants will be successful if funded by a fictional company "Alphabet Soup." After the data is preprocessed, a Neurnal Network Model is compiled, trained and evaluated. Finally, there is an attempt made to optimize the model by increasing the accuracy to 75% or higher.



## Results:

### Data Preprocessing
- "EIN" and "NAME" columns were dropped
- Columns with more than 10 unique values, such as the "CLASSIFICATION" and "APPLICATION_TYPE" columns
- list of categorical variables is generated and  then encoded using OneHotEncoder. 
- The variable considered the target for this model is "IS_SUCCESSFUL,"  and all other variables in the dataframe are considered features.

### Compiling, Training, and Evaluating the Model
- Rectified Linear Unit (ReLU) is used as the activation function for both the first and second hidden layers.
- For the output layer, a sigmoid activation function is used. While training the model.
- Callback saves the model's weights every 5 epochs. 
- After training, the model's Loss and Accuracy values are evaluated. 

Result was  an accuracy of 0.73 %  then  optimize the model by increasing the accuracy to 75% or higher but result was  an accuracy of 0.725

## Summary:

The following methods were attempted was use to optimization  in this analysis were able to produce a model with a predictive accuracy level of 75% or higher but none of them help to improve  Accuracy  value. 

- Dropping more or fewer columns.
- Creating more bins for rare occurrences in columns.
- Increasing or decreasing the number of values for each bin.
- Adding more neurons to a hidden layer.
- Adding more hidden layers.
- Using different activation functions for the hidden layers.
- Adding or reducing the number of epochs to the training regimen.

Instead of using a Deep Learning model in this binary classifiication project, it may be preferable to use a Random Forest Classifier. Whereas Deep Learning models are complex to setup and time consuming to train, Random Forest Classifiers are much simpler to setup and can be trained in a matter of seconds. it is recommended to use a Random Forest Classifier for future development on this project.
