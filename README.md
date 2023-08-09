# TSclass

## This code takes in linkedIn profiles, train a ML model using semi-supervised learning, and predicts the liklihood that the profile has TS/SCI

## The TS SCI Classification model contains 4 sections:

### Section 1: Initialize functions

  import modules and define functions to be used later in the model

### Section 2: Build Training Dataset

  using the 'updated_datasets' folder, build the dataset used to train/test the model

### Section 3: Train CatBoost Model

  split the data into train/test split. Undersample the non TS majority class after the split to mitigate class imbalance.
  Conduct hyperparamter tunning on the training set and fit a model, then use model to create pseudo labels for the full dataset.
  Next use the best hyperpameters to fit a model on the full dataset and check performance.

### Section 4: write out predictions 

Write out predictions to csv file and analyze output
