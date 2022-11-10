# Neural_Network_Charity_Analysis

![deep-learning-brain-cutaway-800x450](https://user-images.githubusercontent.com/108313440/201224553-98ab0663-d790-41f6-b4a2-96cb39038d90.jpg)


## Overview of the Project
In this analysis, we help Alphabet Soup 's business team to determine if the money it donated was used effectively by organizations that it funded over the past years. The dataset contained 34,000 organizations that had received funding from Alphabet soup. In the dataset, columns included the application type, the industry sector, the government classification, the use case for funding, the type of organization, income classification, funding amount requestedand, and the effective useness of the money. There were three steps invovled in this project : 

1. Preprocessing the data for the neural network 

2. Compile, Train and Evaluate the Model 

3. Optimizing the model

To this end, I created neural network models using Scikit-Learn, Tensorflow and Keras to complete this analysis.


## Resources

* Data Source: [charity_data.csv](https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-online/module_19/charity_data.csv)

* Software: Python 3.7.7, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

## Results

### Data Preprocessing

* Identification information such as EIN and NAME has been removed from the input data.

* Column IS_SUCCESSFUL contains binary data that indicates whether charity donations were used effectively. Our deep learning neural 

* network uses this variable as its target.

* The following columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for our model.

* Categorical variables were encoded, split into training and testing datasets, and standardized.

### Neural Network Modeling

* An 80-neuron layer is the first layer and a 30-neuron layer is the second layer.

* Due to its binary classification, the output layer is composed of only one neuron.

* For the hidden layers, we use the activation function ReLU. We use Sigmoid on the output layer due to the binary nature of our output.

* For the compilation, the optimizer is adam and the loss function is binary_crossentropy.

### Optimization Procedure

My analysis showes that the model accuracy is below 75%, which does not provide a satisfactory performance when predicting the efficiency of charity donations.

* To improve the model's performance, we bucketed the ASK_AMT feature and organized the values by intervals (AlphabetSoupCharity_Optimzation).

* The number of neurons on one of the hidden layers was increased, and then the model was used with three hidden layers (AlphabetSoupCharity_Optimzation 2).

* My model also did not improve after trying different activation functions (tanh) (AlphabetSoupCharity_Optimzation 3).

## Summary

Despite a target of 75% accuracy, the deep learning neural network model failed to meet it. Based on what we can see from this target level, it is logic to state that the model doesn't outperform. Considering that we are dealing with binary classifications, we could use supervised machine learning models like Random Forest Classifier to improve the outcome. 
