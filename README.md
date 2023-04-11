# Deep-Learning-Challenge

The Alphabet Soup Charity model was analyzed using a dataset of over 35,000 organizations that were previously funded by the charity. The aim was to develop a deep learning neural network model to predict the success or failure of future funding initiatives.

To create the model, the "IS_SUCCESSFUL" column was used as the target variable, and different feature sets were explored to assess their impact on loss and accuracy. The "EIN" and "NAME" variables were removed from all optimization attempts.

The main model consisted of two hidden layers with 80 and 30 neurons, respectively, and used the "relu" activation function in the hidden layers and the "sigmoid" activation function in the output layer. The model was trained for 100 epochs but only achieved an accuracy of approximately 72.76% with a loss of 55.85%, falling short of the target performance of 75%.

## Three optimization attempts were made to improve the model's performance: 

### Attempt #2
Involved increasing the number of epochs, adding a hidden layer with 60 neurons, modifying the binning structure of the "CLASSIFICATION" column, and adding more neurons to the hidden layers, but it resulted in lower accuracy and higher loss. 

### Attempt #3:
Involved dropping the 'STATUS' and 'SPECIAL_CONSIDERATION' variables, altering the binning structures of the 'APPLICATION_TYPE' and 'CLASSIFICATION' variables, and adding a new hidden layer with 60 neurons, but it also resulted in lower accuracy and higher loss. 

### Attempt #4:
Involved adding two more dense layers, resulting in a slight improvement in accuracy to 73.01% and a decrease in loss to 55.82%.

Despite Attempt #4's small positive impact, none of the optimization attempts significantly increased accuracy, and some even led to higher loss. Given the abundance of categorical data in the dataset, it may be worthwhile to explore decision tree or random forest methods for potentially better results.
