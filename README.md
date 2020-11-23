# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis was to build a machine learning model to help the Alphabet Soup charity in deciding which charities to approve requests for. I was tasked with pre-processing the data then building an initial model that was provided and in another delivable, I was tasked with tuning the model to achieve a higher accuracy %.


## Results

### Data Preprocessing

- The variable considered the target for the model is "IS_SUCCESSFUL" in this challenge

- The variables considered as features are application type, classification, use case, organization, and income

https://github.com/jasonatoledo/Neural_Network_Charity_Analysis/blob/main/nn_df_target_feat.png

- The variables that I removed from the input data were the two original columns, name and EIN, then I removed status and special considerations because the values of those columns were unbalanced and skewed at 99%+ for one side. I also consolidated the very minimal use case columns into a "use case other" column as well as the organization columns that had very tiny values <1% of the population.

### Compiling, Training, and Evaluating the model

-  I ended up training/revising 20 models, even though the challenge asked for at least 3. I tried a ton of different combinations, ranging from 2 hidden layers to 6 hidden layers. I tried several different activation functions, including relu, tanh, and sigmoid. I eventually settled on relu since I read a ton of blogs, medium and stack overflow that said it is the best performing right now and sigmoid for the output layer as it is a binary classifying activation function. I even tried different optimizer functions and expirimented for well over 12 hours in this challenge.

https://github.com/jasonatoledo/Neural_Network_Charity_Analysis/blob/main/nn_layers_neurons.png

- I was not able to achieve the 75% as intended, even with training a model for 2000 epochs, which I know could be overfitting the model for sure but I wanted to try all possible combinations that I was equipped with to get to 75%.

- The steps I took to increase model performance were:

 - Condense columns with very low percentage of population
 
 - Remove columns that didn't have a significance
 
 - Try different values of hidden layers, with the max of 200 for the 1st layer at one point
 
 - Tried at least 6 different activation functions, tried a different loss function, and tried 5 different optimizers
 
 - Played with 2, 3, 4, 5, 6 different hidden layers with varying neurons

https://github.com/jasonatoledo/Neural_Network_Charity_Analysis/blob/main/nn_20_models.png


## Summary

I wasn't thrilled with spending 12+ hours trying to perfect a model and couldn't even achieve 75% as asked with over 20+ different iterations of the model. I would like to learn more about setting learning rates as well as more context on decay and loss functions. I wasn't able to locate a feature importance function for neural networks and that wasn't mentioned in this particular module. I am very curious to know how many of my classmates got to the 75% as I believe I put in more effort and time than the average student would have.
