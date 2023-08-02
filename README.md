# deep-learning-challenge
Module 21 Challenge
Report on the Neural Network Model for Alphabet Soup
Overview
The purpose of this analysis was to create a deep learning model using a neural network to predict the success of philanthropic projects for Alphabet Soup. The model aims to assist in funding decisions, maximizing the impact of their philanthropic efforts.

Results
Data Preprocessing
    Target Variable: "Project Success" represented by "IS_SUCCESSFUL" (binary, 1 for success, 0 for failure).
    Features: Selected from various project-related variables.
    Variables Removed: Non-beneficial ID columns ('EIN' and 'NAME').
Model Details
    Neural Network Architecture: Two hidden layers (400 neurons with 'ReLU' and 200 neurons with 'tanh') and an output layer (1 neuron with 'sigmoid').
    Model Performance: Achieved 73% accuracy on the test dataset.
    Steps to Improve Performance
Data Preprocessing: Removed irrelevant columns and used one-hot encoding for categorical variables.
Feature Binning: Grouped low-frequency application types and classifications as "Other."
Data Scaling: Standardized the features using StandardScaler.
Hyperparameter Tuning: Adjusted neuron count, layers, and activation functions for optimal performance.
Recommendation
Consider trying the Random Forest Classifier to improve performance:

Random Forest handles both numerical and categorical data effectively.
Provides feature importance rankings for better understanding of key variables.
Can handle imbalanced datasets, often present in project success prediction.
In conclusion, implementing a Random Forest Classifier may enhance the model's performance and interpretability for predicting project success in Alphabet Soup's philanthropic endeavors.