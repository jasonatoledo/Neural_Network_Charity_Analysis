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

-  

https://github.com/jasonatoledo/Neural_Network_Charity_Analysis/blob/main/nn_layers_neurons.png

-

-

https://github.com/jasonatoledo/Neural_Network_Charity_Analysis/blob/main/nn_20_models.png


## Summary
