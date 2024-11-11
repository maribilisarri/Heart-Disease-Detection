Heart Disease Detection
This notebook explores the Cleveland Heart Disease dataset to build a model for predicting the presence of heart disease. The dataset contains 14 attributes, including age, sex, chest pain type, blood pressure, cholesterol levels, and various other physiological measurements.

Workflow:

Data Inspection and Preprocessing:

The notebook begins by loading and inspecting the dataset, checking for missing values and data types.
Missing values are handled by removing rows containing them.
Data types are converted to numeric for compatibility with machine learning models.
Exploratory data analysis is performed to understand the distribution of variables and relationships between them.
Data Visualization:

Histograms and density plots are used to visualize the distribution of individual features for patients with and without heart disease.
These visualizations provide insights into the importance of different features in predicting heart disease.
The data is scaled using StandardScaler to avoid any dominance of some features over others and also to avoid very high values.
Model Building and Training:

Categorical Classification:
The notebook builds a categorical classification model to predict the severity of heart disease (0-4).
It uses a Keras sequential model with three dense layers, ReLU activation in the hidden layers, and softmax activation in the output layer.
The model is trained using the Adam optimizer and categorical cross-entropy loss.
Binary Classification:
The target variable is converted into a binary representation (0 for no heart disease, 1 for presence of heart disease).
A separate binary classification model is built using a similar architecture as the categorical model.
It uses sigmoid activation in the output layer and binary cross-entropy loss.
Scaling the data is also used to perform binary classification
Evaluation and Results:

Both models are evaluated using accuracy and a classification report.
The results show that the model achieved decent accuracy on the test set, demonstrating its ability to predict heart disease.
Key Findings:

Several features, such as chest pain type, maximum heart rate achieved, and exercise-induced angina, show clear distinctions between patients with and without heart disease.
The model demonstrates the potential for using machine learning to assist in heart disease diagnosis and risk assessment.
By using a scaled dataset a better accuracy is obtained
Next Steps:

Explore advanced feature engineering techniques to further improve model performance.
Experiment with different models, hyperparameter tuning, and cross-validation to optimize the model.
Validate the model on a larger, independent dataset for robustness.
Develop an interactive web application to make the model accessible to healthcare professionals.
