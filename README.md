# deep-learning-challenge

## Overview

    This analysis is about building a neural network model to be able to predict the best chance of success of applicants so they can be chosen for funding. The data will be based from a csv file containing 34,000 organizations who have been fundded over the years and have recorded their success in the venture.

## Results

### Data Preprocessing

* What variable(s) are the target(s) for your model?
      The target data is the IS_SUCCESSFUL column.
* What variable(s) are the features for your model?
      The following are the feature data for my model, APPLICATION_TYPE, AFFILIATION CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT.
* What variable(s) should be removed from the input data because they are neither targets nor features?
      The variables 'EIN' and 'NAME' were removed and not used as inpute data as they contribute nothing to the logic of the model being created.

### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
    I have selected 50 neurons as a random value. There are 43 columns in total so I decided a value bigger than 43.
    There are 2 layers which indicates deep learning.
    I used relu function for the inner layers and sigmoid for the outer layer functions. These are the common but effective functions used in previous examples so I used the same. I think they are best best suited functions I know so far.
* Were you able to achieve the target model performance?
    Unfortunately, I was not able to reach the targeet of 75% accuracy. Below are the results of the 4 trials I did with the last 3 trials trying to optimaize the model performance.
    Accuracy: 0.7243148684501648
    Optimizations:
    1st - Accuracy: 0.7252478003501892
    2nd - Accuracy: 0.7250145673751831
    3rd - Accuracy: 0.7241982221603394

* What steps did you take in your attempts to increase model performance?
    My first optimizations was a simple increase in the number of nuerons from 50 to 100, which slightly increased the perfomance to 0.3%.
    My second optimization was to add the 3rd layer, which surprisingly, did not improve the performance from my first optimization.
    My third attempt was to further perform some bucketing of 3 more columns namely, Affiliation, Use-Case and Organization. But this did not make any improvements but made the performance degarde by 0.1%.


### Summary
    In general, my model was not successful in acieving the 75% accuracy.
    Looking at the results, it looks like the most effective optimization was adding more neurons. In this exercise, I wanted to try changing different variables like bucketing/binning, number of neurons and number of layers. Based on those options I tried, it looks like increasing the number of neurons made the most difference. I would recommend increasing the neurons more, and with the additional layer, I would think that the accuracy will improve.


## Submitted Files
* AlphabetSoupCharity.ipynb - main file containing initial model
* AlphabetSoupCharity.h5 - initial exported model
* AlphabetSoupCharity_Optimisation.ipynb - contains first try at optimizing model
* AlphabetSoupCharity_Optimisation.h5 - first try at optimizing model, exported model
* AlphabetSoupCharity_Optimisation2.ipynb - contains second try at optimizing model
* AlphabetSoupCharity_Optimisation2.h5 - second try at optimizing model, exported model
* AlphabetSoupCharity_Optimisation3.ipynb - contains third try at optimizing model
* AlphabetSoupCharity_Optimisation3.h5 - third try at optimizing model, exported model
