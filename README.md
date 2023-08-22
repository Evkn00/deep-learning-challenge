# deep-learning-challenge

## Deep learning model target:

This project has created a deep learning model for prediciting if funding applicants will be successful in their venturs if Alphabet Soup was to accept their application. The success target for this model was set at 75% and a dataset of 34,000+ previously funded organisations was used to train the model. 

## Results:

### 1. Data Preprocessing

Target Variable:
IS_SUCCESSFUL—Was the money used effectively. This could either be 1 for successful or 0 for not successful. 

Feature variables: 

APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested

Dropped variables:
EIN and NAMES were dropped from the dataset as each row had a unique one of each so no value as a feature. 

Compiling, Training, and Evaluating the Model
For the initial model, efficiency was prioritised and as hyperparameter tuning was intended as the optimisation method it was determined that basic high speed values were acceptable for this attempt. The initial model used two hidden layers with 8 and 5 nodes respectively
The model was reasonably successful achieving just under 73% accuracy, which gave considerable hope for the tuned model to achieve over 75%

![image](https://github.com/Evkn00/deep-learning-challenge/assets/69624124/71808f31-440d-43a2-9e12-c98bfb76e7cc)

Hyperparameter turning was selected as the best optimisation model and ranges were selected for the tuning that were likely considerably beyong the requirements, however since time and efficency are not huge factors for a model that will not be used live, the following parameters were tested:
- Activation: 'relu','tanh','sigmoid'
- Layers: 1 to 20 in steps of 2
- Starting nodes: 1 to 100 in steps of 5
- Max 20 epochs
  


What steps did you take in your attempts to increase model performance?
Summary: Summarise the overall results of the deep learning model. Include a recommendation for how a
