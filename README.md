# propensify  
Objective: Develop a predictive model to assess the likelihood of specific customer groups responding to a marketing campaign.

Data Loading: Import data from an Excel file and assess missing values.

Data Cleaning: Drop irrelevant columns (e.g., 'profit', 'contact', 'month') and handle null values by imputing with mode and median.

Exploratory Data Analysis (EDA):

Visualize age distribution and profession, marital status, and loan status, analyzing the response rates for each group.
Label Encoding: Convert the response column ('responded') into binary values (0 and 1).

Feature Engineering:

Separate numerical and categorical features.
Use StandardScaler for numerical features and OneHotEncoder for categorical features.
Data Preprocessing Pipeline:

Create a preprocessor pipeline with transformations for numerical and categorical columns.
Data Splitting: Divide the data into training and validation sets (90-10 split).

Model Training:

Implement a Random Forest Classifier.
Use RandomizedSearchCV for hyperparameter tuning with a specific grid.
Evaluation:

Assess model performance on the training and validation sets using accuracy.
Model Saving: Save the trained model as a .pkl file for future use.

Testing on New Data:

Load and preprocess the test dataset.
Ensure column compatibility with the training set, adding missing columns.
Prediction: Generate predictions and probabilities for the test set, storing the results in a DataFrame.
