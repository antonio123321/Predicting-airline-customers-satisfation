This readme file includes some description and guidance for Airline Passenger Satisfaction Prediction, first using a decision tree algorithm and then a K-NN algorithm.





Airline Passenger Satisfaction Prediction Decision Tree.

This project aims to predict passenger satisfaction with airline services based on various features such as customer type, flight distance, in-flight services, and more. The dataset used in this project contains information about airline passengers and their satisfaction levels.


The dataset includes the following columns:

    Gender
    Age
    Customer Type
    Type of Travel
    Class
    Flight Distance
    Departure and Arrival Time Convenience
    ...

Part 1: Data Preprocessing
Handling Missing Values

In the first part of the code, missing values in the dataset were addressed. The missing values in the 'Arrival Delay' column were filled using an median..
Column Operations

Unnecessary columns, such as 'ID', were dropped from the dataset. The 'Age' column was shifted after the 'Class' column for standardization purposes. The 'Satisfaction' column was moved to the end of the dataset.
Correlation Analysis

A correlation matrix was computed to understand the relationships between different features in the dataset.

Part 2: Model Training and Evaluation
Feature and Target Variable

The dataset was split into feature variables (X) and the target variable (y), where 'X' represents the input features, and 'y' represents the passenger satisfaction labels.
Data Splitting

The data was divided into training and testing sets using the train_test_split function from scikit-learn.
Decision Tree Model

A Decision Tree Classifier was selected as the predictive model. Grid search was used to find the optimal hyperparameters for the Decision Tree.
Model Evaluation

The model was evaluated using accuracy, confusion matrix, and classification report metrics. The accuracy achieved on the test set was approximately 95.58%, indicating a robust performance.
Confusion Matrix Visualization




Airline Passenger Satisfaction Prediction K-nn.

This project aims to predict passenger satisfaction with airline services based on various features such as customer type, flight distance, in-flight services, and more. The dataset used in this project contains information about airline passengers and their satisfaction levels.


The dataset includes the following columns:

    Gender
    Age
    Customer Type
    Type of Travel
    Class
    Flight Distance
    Departure and Arrival Time Convenience
    ...
The The libraries are imported

Part 1: Data Preprocessing
Handling Missing Values

In the first part of the code, missing values in the dataset were addressed. The missing values in the 'Arrival Delay' column were filled using an median..
Column Operations

The categorical columns are transformed to numerical

Unnecessary columns, such as 'ID', were dropped from the dataset. The 'Age' column was shifted after the 'Class' column for standardization purposes. The 'Satisfaction' column was moved to the end of the dataset.
Correlation Analysis



Part 2: Model Training and Evaluation
Feature and Target Variable

The dataset was split into feature variables (X) and the target variable (y), where 'X' represents the input features, and 'y' represents the passenger satisfaction labels.
Data Splitting

The data was divided into training and testing sets using the train_test_split function from scikit-learn.

Data scaling
The data was scaled usingg Minmax scaler
Decision Tree Model

A K-nn Classifier was selected as the predictive model. Grid search was used to find the optimal hyperparameters for the K-nn.
Model Evaluation

The model was evaluated using accuracy, confusion matrix, and classification report metrics. The accuracy achieved on the test set was approximately 93.52%, indicating a robust performance.
Confusion Matrix Visualization

The confusion matrix was visualized using the seaborn heatmap, providing a clear overview of the model's true positive, true negative, false positive, and false negative predictions.
Conclusion

The Knn Classifier demonstrated strong predictive capabilities for passenger satisfaction based on the provided features. The high accuracy suggests that the model is effective in distinguishing between satisfied and unsatisfied passengers.
The confusion matrix was visualized using the seaborn heatmap, providing a clear overview of the model's true positive, true negative, false positive, and false negative predictions.
Conclusion

The Decision Tree Classifier demonstrated strong predictive capabilities for passenger satisfaction based on the provided features. The high accuracy suggests that the model is effective in distinguishing between satisfied and unsatisfied passengers.
