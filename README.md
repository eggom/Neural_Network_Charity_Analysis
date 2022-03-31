# Neural_Network_Charity_Analysis
Module 2 Challenge - ML Pathway - Trilogy Instructors
<br/><br/><br/>

## Overview of the analysis

A hypothetical nonprofit foundation, Alphabet Soup, needs help analyzing the impact of their donations and vetting potential recipients by predicting which organizations are worth donating to and which are too high risk. I designed a deep learning neural network that evaluates all types of input data and produces a clear decision making result using the Python TensorFlow library.
<br/><br/><br/><br/>




## The Data
We have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization
<br/><br/>


### Data Preprocessing
In this section we will try to answer the following questions.
<br/><br/>

**What variable(s) are considered the target(s) for your model?**
<br/>
Our target variable will be ```IS_SUCCESSFUL```which encodes if the money was used effectively.
<br/><br/>

**What variable(s) are considered to be the features for your model?**
<br/>
The rest of the variables in the CSV could be considered to be our features however some of them were dropped due to several reasons:
* *EIN* and *NAME*: Identification columns. High Cardinality
* *STATUS* and *SPECIAL_CONSIDERATIONS*: They were having very skewed distributions towards the target variable, hence its removal.
<br/><br/>

### Compiling, Training, and Evaluating the Model
<br/><br/>
**How many neurons, layers, and activation functions did you select for your neural network model, and why?**
<br/>
For the optimal model it was selected an ANN with 3 hidden layers starting with 24 neurons followed by 15 and finally 4 with activation functions of SOFTMAX. Final output layer, 1 neuron with Sigmoid. Number of inputs were 34 corresponding with the number of variables after dropping and one-hot-encoding.
<br/><br/>

**Were you able to achieve the target model performance?**
<br/>
Sadly I ended up just touching the requested value of 75%. My actual was 74.54%
<br/><br/>

**What steps did you take to try and increase model performance?**
<br/>
I basically touched on:
* number of neurons per layer.
* Number of actual hidden layers.
* Activation Function.
* Furthers Data Preprocessing and feature dropping (if I was having time I would have performed some fature engineering).
<br/><br/><br/><br/>



## Summary
Through the removal of noisy features, additional neurons and hidden layers and changed activation functions, the accuracy of my optimized model for predicting whether a donation is successful ended up being 0.7454.
<br/><br/>

## Recommendation
A random forest model could solve this classification problem by randomly sampling the preprocessed data and building several smaller, simpler decision trees. Some benefits of using a random forest model include how robust it is against overfitting of the data because all of the weak learners are trained on different pieces of the data, it can be used to rank the importance of input variables, it is robust to outliers and nonlinear data, and it can run efficiently on large datasets.
