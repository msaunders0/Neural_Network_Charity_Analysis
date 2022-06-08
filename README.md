# Neural_Network_Charity_Analysis

## Overview

Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

## Results
### Data Preprocessing

- What variable(s) are considered the target(s) for your model?
    - The target variable for my model was the 'IS_SUCCESSFUL' column.  

- What variable(s) are considered to be the features for your model?
    - The features for my model were APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and SPECIAL_CONSIDERATIONS.

- What variable(s) are neither targets nor features, and should be removed from the input data?
    - EIN and NAME were dropped for having no benefit to the accuracy rate of the model.

### Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - For my Sequential model, I initially selected 2 layers, the first with 80 neurons and the second with 30 neurons, using the ReLU activation function for both processing layers and the Sigmoid activation function for the output layer. I felt that this would likely be a good starting point, but expected to optimize these selections.

- Were you able to achieve the target model performance?
    - Unfortunately, no I was not. The highest average accuracy rate I was able to achieve with my model was 73%, which fell short of the 80% specification.

- What steps did you take to try and increase model performance?
    - I adjusted the number of layers, adjusted the number of neurons for each layer, and dropped the STATUS column, all with the hopeful expectation to increase the accuracy rate. These attempts were unsuccessful, although the average accuracy rate did improve by 1% through my optimization attempts.

## Summary
Unfortunately, I was unable to reach a model accuracy rate of 80%. In the future, I could attempt to use a different classification model (non-sequential or SVM to avoid overfitting?). I could also reduce the number of hidden layers to 1 instead of 2-3. Reducing complexity can often have a positive affect on the accuracy score.  