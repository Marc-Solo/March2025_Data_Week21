# March2025_Data_Week21
Built a deep learning model to predict the success of funding applicants for Alphabet Soup using TensorFlow and Keras. The project includes data preprocessing, model training, optimization, and performance evaluation.

Overview of the Analysis:
This analysis aims to build a deep learning model to predict whether an applicant will be successful if funded by Alphabet Soup. The goal is to classify organizations as successful or unsuccessful based on features such as application type, use case, and income. The model will help determine which applicants are likely to use the funding effectively.

Results
Data Preprocessing:
Target Variable:
The target variable is IS_SUCCESSFUL, which indicates whether the organization was successful or not.

Feature Variables:
The features include all columns except IS_SUCCESSFUL, EIN, and NAME. These are the predictors used to make the prediction.

Variables to Remove:
The EIN and NAME columns were removed as they are identifiers and do not help predict success.

Compiling, Training, and Evaluating the Model
Neurons, Layers, and Activation Functions:
The model consists of:

Input Layer: 16 neurons for each feature.
Hidden Layer 1: 64 neurons with ReLU activation.
Hidden Layer 2: 32 neurons with ReLU activation.
Output Layer: 1 neuron with sigmoid activation for binary classification (success or failure).
ReLU was used in the hidden layers to allow the model to learn complex patterns, and sigmoid was used in the output layer to predict a probability of success.

Target Model Performance:
The target accuracy was above 75%, but the model achieved:

Accuracy: 72.92%
Loss: 0.5677
Since the performance was below the target, more adjustments were needed.

Steps Taken to Improve Model Performance:
To improve the model, I:

Increased the number of neurons in the hidden layers.
Trained the model for more epochs.
Experimented with different architectures, but the accuracy still did not reach the target.
Summary
The model was trained to predict whether an applicant would be successful with Alphabet Soup funding. The model achieved an accuracy of 72.92%, which is below the target of 75%.

Model Evaluation:

Accuracy: 72.92%
Loss: 0.5677
Further optimization could improve the model's accuracy.

Alternative Model Recommendation:
If the neural network model doesn't meet the performance target, a Random Forest Classifier or Gradient Boosting Model (XGBoost) could be a good alternative. These models handle categorical data well and tend to perform better on structured datasets.
