# deep-learning-challenge
# Neural Network Model Report for Alphabet Soup

## Overview of the Analysis

The aim of this analysis was to forecast the success of initiatives financed by Alphabet Soup by utilizing machine learning. The goal was to determine whether the money were likely to be used successfully by the groups receiving them by modeling past data of financed projects.

## Results

### Data Preprocessing

- **Target Variable**: The target variable for the model was `IS_SUCCESSFUL`, indicating the effectiveness of the fund usage.
- **Features**: The model included features such as `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, and `ASK_AMT`.
- **Removed Variables**: Identification columns `EIN` and `NAME` were removed from the dataset as they do not contribute to the predictive ability of the model.

### Compiling, Training, and Evaluating the Model

- **Neurons, Layers, and Activation Functions**: Our neural network consisted of four hidden layers with 128, 64, 32, and 16 neurons, respectively. Activation functions used were ReLU and LeakyReLU for hidden layers, and a sigmoid function for the output layer.
- **Model Performance**: The goal was to achieve an accuracy higher than 75%. The best model reached an accuracy of approximately 72.49%, just shy of the target.
- **Optimization Attempts**: To enhance model performance, I:
  - Increased the number of hidden layers and neurons.
  - Introduced dropout and batch normalization to combat overfitting.
  - Experimented with different activation functions.
  - Adjusted the optimizer's learning rate and used a learning rate scheduler.
  - Implemented early stopping to prevent overfitting during training.

## Summary

The predictive power of the deep learning model was shown to be moderate when it came to forecasting the outcome of Alphabet Soup funding applications. Even though it falls short of the desired accuracy, it provides a promising beginning point for more model optimization.

In order to improve performance for this kind of structured data, it is advised to investigate ensemble machine learning techniques like Random Forest classifiers and Gradient Boosting in the future. Furthermore, a deeper feature engineering process might improve the model's predictive power.

