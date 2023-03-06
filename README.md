# Deep-learning

## Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## Overview

The purpose of the analysis is to create a binary classifier, using the features in the given dataset, that can predict whether the applicants will be successful if funded by the Alphabet Soup. Analyzed using the neural network model and based on the accuracy, further adjustments are made to optimize the performance of the model. Results

## Data Preprocessing

1. The target variable in the model is 'IS_SUCCESSFUL.'

2. Dropping NAME and EIN, below are the features used in the initial analysis of the model.

- APPLICATION_TYPE
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- STATUS
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- ASK_AMT

3. For Optimizing the model made some adjustments by adding and removing few features.

- STATUS-it had 34294 number of 1’s and 5 in number of 0’s.
- SPECIAL_CONSIDERATIONS-it had 34272 number of N values and 27 Y values.

![imige](https://github.com/jennykardashov/deep-learning-challenge/blob/main/Screenshots/1.png)

The above two features were removed and added NAME feature

So, the final model had the following features.

- NAME
- APPLICATION_TYPE
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- INCOME_AMT
- ASK_AMT

## Compiling, Training, and Evaluating the Model

1. The initial analysis had 2 layers, with 80 neurons in first hidden layer and 30 neurons in the second hidden layer. The model used two different activation functions- relu and sigmoid.

![imige](https://github.com/jennykardashov/deep-learning-challenge/blob/main/Screenshots/2.png)

2. The target predictive accuracy was 73%

![imige](https://github.com/jennykardashov/deep-learning-challenge/blob/main/Screenshots/3.png)

3. In order to increase the performance, further adjustments were made to optimize the model by removing the features “STATUS” and “SPECIAL_CONSIDERATIONS“ and added the feature “NAME”. • Created binning for the rare occurrences in the columns “AFFLIATION “and “NAME”.

![imige](https://github.com/jennykardashov/deep-learning-challenge/blob/main/Screenshots/4.png)

![imige](https://github.com/jennykardashov/deep-learning-challenge/blob/main/Screenshots/5.png)

4. Added more neurons to the hidden layers. • Used 3rd hidden layer. • Used different activation functions for the hidden layers.

![imige](https://github.com/jennykardashov/deep-learning-challenge/blob/main/Screenshots/6.png)

5. The model exceeded the target performance of 75%.

![imige](https://github.com/jennykardashov/deep-learning-challenge/blob/main/Screenshots/7.png)

## Summary

The initial model could achieve the accuracy of 73%. To further improve the accuracy, the model was optimized and reached an accuracy of79%.This was achieved by considering the NAME column and adding binning to them, removing the SPECIAL_CONSIDERATIONS and STATUS columns as there were more variability in the values and finally adding more number of neurons, 3rd hidden layer and changing the activation functions. As per the requirement, I tried using Logistic Regression and Random Forest Classifier to predict the accuracy and was able to get 78% accuracy in both the models.

![imige](https://github.com/jennykardashov/deep-learning-challenge/blob/main/Screenshots/8.png)


