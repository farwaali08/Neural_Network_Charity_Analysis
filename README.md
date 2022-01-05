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

* The model is composed of 2 hidden layers with 80 neurons in the first layer and 30 in the second
  * The input data has 43 features and 25,724 samples
  *  The following activation functions were used: 
     * **ReLU** for the hidden layers, to allow for a [faster](https://stats.stackexchange.com/questions/126238/what-are-the-advantages-of-relu-over-sigmoid-function-in-deep-neural-networks) training process 
     * **Sigmoid** for the output layer, as the model is intended to be a binary classifier
  * Optimizer: `adam` 
  * Loss function: `binary_crossentropy`

* The model's accuracy did **not** meet the target of `75%` in the initial run. In an attempt to improve the performance of the model, the following changes were made:
  * Increased the number of neurons in one of the hidden layers
  * Incorporated an additional hidden layer
  * Use a different activation function: `tanh` 

These changes did not improve the model's performance, and in fact, they seemed to lower its performance slightly. The highest accuracy achieved was about `72.5%`, which is not acceptable for this analysis.

## SUMMARY

The model achieved a maximum accuracy of only `72.5%`. This does not reach the target accuracy, which at 75% is not a great ask. This suggests that a different model would be better suited for this project. As the objective was to create a binary classifier, the Random Forest Classifier model would be a better fit, as it generally has higher accuracy/greater predictive capabilities.
