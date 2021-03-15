# Neural_Network_Charity_Analysis

## Overview
A grant giving organization has noticed that high risk charities have been applying for funding. High risk charities apply for funding and then disappear after receiving the money. The grant giving organization wants to predict which organizations are worth donating to and which are too high risk. To achieve this goal I created and trained a neural network capable of predicting whether applicants will be successful if offered funding

## Results

### Data Preprocessing
- The target variable for my model is the "Is_Successful" column which tells us whether the money was used successfully.
- The features in this model are "Application_type", "Affiliation", "Classification", "Use_Case", "Organization", "Status", "Income_amt", "Special_consideration", and "Ask_amt".
- The "EIN" and "Name" columns were removed from the dataset because they were neighter targets nor features, the purpose of these columns were to identify each unique user.

### Compiling, Training, and Evaluating the Model
- Through different optimization tactics I was able to achieve 73.99% accuracy.
- In my first attempt to increase model performance I chose to bin categorical variables together from the column "Income_Amnt". In my second attempt I added an additional hidden layer, allowing neurons to train on activated input values. In my third attempt, I increased the number of epochs, training iterations, from 100 to 200, providing each neuron with more information from the input data.
