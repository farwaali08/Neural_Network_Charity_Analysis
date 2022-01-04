# Neural_Network_Charity_Analysis 🧠

## OVERVIEW

This project looks at deep-learning neural networks, with an ultimate purpose of creating a binary classification model that is capable of predicting the success of donations. 

The workhorse of this analysis is Python's TensorFlow library. To help determine different methods of optimization, various models were tested in the [TensorFlow playground](https://playground.tensorflow.org) and the modifications were selected accordingly.

The analysis can be divided into the following parts:

* Data preprocessing 
* Compiling, training, and evaluating the model
* Optimization


## TOOLS & RESOURCES

### DATA

[charity_data.csv](https://github.com/farwaali08/Neural_Network_Charity_Analysis/blob/1624af9a41c1ddec87eced9033fc9d438cb2ed4d/Data/charity_data.csv)

### SOFTWARE

* Python 3.9.3
  * Scikit-learn, TensorFlow 
* Jupyter Notebook 6.3.0

### CODE

[AlphabetSoupCharity.ipynb](https://github.com/farwaali08/Neural_Network_Charity_Analysis/blob/69088162da47d789555afcca2e79e8ee77a853fe/Notebooks/AlphabetSoupCharity.ipynb)

[Optimization 1](https://github.com/farwaali08/Neural_Network_Charity_Analysis/blob/69088162da47d789555afcca2e79e8ee77a853fe/Notebooks/AlphabetSoupCharity_Optimzation1.ipynb)

[Optimization 2](https://github.com/farwaali08/Neural_Network_Charity_Analysis/blob/69088162da47d789555afcca2e79e8ee77a853fe/Notebooks/AlphabetSoupCharity_Optimzation2.ipynb)

[Optimization 3](https://github.com/farwaali08/Neural_Network_Charity_Analysis/blob/69088162da47d789555afcca2e79e8ee77a853fe/Notebooks/AlphabetSoupCharity_Optimzation3.ipynb)

## RESULTS

### DATA PRE-PROCESSING

* `IS_SUCCESSFUL` is the **target variable** in this analysis, as it represents whether the donation was used effectively
* The following are a list of variables that are **features** (along with description):
  * `APPLICATION_TYPE`—Alphabet Soup application type
  * `AFFILIATION`—Affiliated sector of industry
  * `CLASSIFICATION`—Government organization classification
  * `USE_CASE—Use`-case for funding
  * `ORGANIZATION`—Organization type
  * `STATUS`—Active status
  * `INCOME_AMT`—Income classification
  * `SPECIAL_CONSIDERATIONS`—Special consideration for application
  * `ASK_AMT—Funding amount`-requested
* `EIN` and `NAME`, which are indentification columns are neither targets nor features, and were **removed** from the input data

### COMPILING, TRAINING, & EVALUATING THE MODEL


## SUMMARY
