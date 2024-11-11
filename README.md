<h1>Heart Disease Detection</h1>
<p>This project utilizes the Cleveland Heart Disease dataset to build a predictive model for detecting heart disease presence. The dataset consists of 14 attributes, including age, sex, chest pain type, blood pressure, cholesterol levels, and other physiological metrics.</p>

    <h2>Workflow</h2>

    <h3>Data Inspection and Preprocessing</h3>
    <ul>
        <li>The dataset is loaded and examined for missing values and data types.</li>
        <li>Missing values are handled by removing the corresponding rows.</li>
        <li>Data types are converted to numeric format for compatibility with machine learning models.</li>
        <li>Exploratory data analysis is performed to understand variable distributions and their relationships.</li>
    </ul>

    <h3>Data Visualization</h3>
    <ul>
        <li>Histograms and density plots visualize the distribution of features for patients with and without heart disease.</li>
        <li>These visuals help identify important predictive features.</li>
        <li>The dataset is scaled using <code>StandardScaler</code> to ensure balanced feature influence and avoid large values.</li>
    </ul>

    <h2>Model Building and Training</h2>

    <h3>Categorical Classification</h3>
    <p>A categorical classification model predicts the severity of heart disease (0-4) using a Keras sequential model with:</p>
    <ul>
        <li>Three dense layers with ReLU activation in the hidden layers and softmax in the output layer.</li>
        <li>The model is trained using the Adam optimizer and categorical cross-entropy loss.</li>
    </ul>

    <h3>Binary Classification</h3>
    <p>The target variable is converted to binary (0 for no heart disease, 1 for presence of heart disease). A binary classification model is built using:</p>
    <ul>
        <li>Similar architecture to the categorical model, but with sigmoid activation in the output layer and binary cross-entropy loss.</li>
        <li>Data scaling is applied to enhance binary classification accuracy.</li>
    </ul>

    <h2>Evaluation and Results</h2>
    <ul>
        <li>Both models are evaluated using accuracy metrics and a classification report.</li>
        <li>Results indicate the model achieved good accuracy on the test set, highlighting its predictive capability.</li>
    </ul>

    <h2>Key Findings</h2>
    <p>Key predictive features include:</p>
    <ul>
        <li>Chest pain type, maximum heart rate achieved, and exercise-induced angina show distinct patterns between patients with and without heart disease.</li>
        <li>The model's success suggests machine learning's potential in heart disease diagnosis and risk assessment.</li>
        <li>Data scaling enhances model accuracy significantly.</li>
    </ul>

    <h2>Next Steps</h2>
    <ul>
        <li>Explore advanced feature engineering to improve model performance.</li>
        <li>Experiment with alternative models, hyperparameter tuning, and cross-validation.</li>
        <li>Validate the model on larger, independent datasets to assess robustness.</li>
        <li>Develop an interactive web application to make the model accessible to healthcare professionals.</li>
    </ul>
