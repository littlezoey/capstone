# capstone
Create a Customer Segmentation Report for Arvato Financial Services

Background
Arvato Financial Services is a mail-order sales company in Germany, the end goal of this project is to help the company use a data-driven instead of rule-based approach to identify the potential customers and target them in the company's marketing exercise. 
The problem can be solved because the historical demographics data for customers are given, we can use the data to train an neural network model, which can be used to predict the likelihood of potential customers from a general population. 

Problem statement
The problem we are trying to solve is to build a machine learning model to predict the likelihood of potential customers from a general population. The model should describe the data for the existing customers, and should be able to accurately predict who are the potential customers based on some key features. The measurement for predictive power should be accuracy ratio, which can be used to measure the performance of model for out of sample dataset.

Datasets and Inputs
We will be using the following three sets of data for feature extraction and modeling, including:
1. Demographics data for the general population of Germany, which includes 891 211 persons (rows) and 366 features (columns).
2. Demographics data for customers of a mail-order companym, which includes 191 652 persons (rows) and 369 features (columns).
3. Demographics data for individuals who were targets of a marketing campaign; 42 982 persons (rows) x 367 (columns). The last column is the label column, which provides information about who successfully were turned into customers, and who are not. 
The first two sets of data are useful for the understanding of the differences and key features between the company's customers and the general population. The third dataset will be split into train and test datasets, in order to train the model, and compute the accuracy ratio using the test data. 

Solution Statement
We will train a deep learning neural network model, including the input layer, hidden layers and the output layer. Neural network model is selected for this problem, because neural network creates a complicated system which will be useful to capture the deep layer relationship between the input and the output. Using neural network also allows us to automate the feature selection and extraction process, because the gradient descent technics will be used to train the model, in order to find the optimized coefficients to minimize the loss function. Last but not the least, neural network model with a sigmoid output layer can produce a binary classifier, which can be used to distinguish between potential customers and the general population, since sigmoid function produces 0 or 1 as output, which can be translated into a binary output problem.

Benchmark Model

