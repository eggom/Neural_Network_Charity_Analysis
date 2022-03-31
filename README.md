# Neural_Network_Charity_Analysis
Module 2 Challenge - ML Pathway - Trilogy Instructors
<br/><br/><br/>

## Overview of the analysis

This repo contains several NN ML Models (binary classifiers) to help the foundation predict where to make investments in the future towards getting successful results of the investment.
<br/><br/>




## The Data
We have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization
<br/><br/>


### Data Preprocessing
In this section we will try to answer the following questions.
<br/><br/>

**What variable(s) are considered the target(s) for your model?**
Our target variable will be ```IS_SUCCESSFUL```which encodes if the money was used effectively.
<br/><br/>

**What variable(s) are considered to be the features for your model?**
The rest of the variables in the CSV could be considered to be our features however some of them were dropped due to several reasons:
* *EIN* and *NAME*: Identification columns. High Cardinality
* *STATUS* and *SPECIAL_CONSIDERATIONS*: They were having very skewed distributions towards the target variable, hence its removal.
<br/><br/><br/><br/>

### Compiling, Training, and Evaluating the Mode
