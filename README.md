# **Severity-Prediction**

**Traffic Accident Severity Prediction**
This project aims to predict the severity of traffic accidents using machine learning techniques.

# **Steps Followed** 
1. **Data Loading**

- Loaded the dataset with over 7 million records, including features like location, weather, and traffic information.
- Dataset Target Columns Severity have (2) 6156981, (3) 1299337, (4) 204710, (1) 67366

2. **Exploratory Data Analysis (EDA)**

- Analyzed missing values, feature distributions, and class imbalance.

- Visualized relationships between features and severity.

3. **Data Preprocessing**

- Handled missing values through imputation.
- Encoded categorical features.
- Data Split Based on Majority of Class Then Build Binary Classification like High Impact and Low Impact.

4. **Feature Engineering**

- Created a new feature: accident Duration.
- Extracted temporal features like Hour, Day_of_Week, and Month.

5. **Data Splitting**

- Split the dataset into training, testing and validation sets.
- Balanced class distribution using techniques like SMOTE.

6. **Feature Selection**

- Used RandomForestClassifier to rank features based on importance.
- Retained only the most impactful features.

7. **Model Building**

- Trained a RandomForestClassifier on the preprocessed and balanced data.
- Adjusted hyperparameters for optimal performance.

8. **Model Evaluation**

- Evaluated the model using accuracy, precision, recall, and F1-score.
- Validation results showed a weighted accuracy of 92%.

9. **Prediction**

- Comparing Actual Class and predicted class using test data.
- Built a Flask API for real-time predictions of accident severity.
- Mapped predictions into low impact (1 & 2) and high impact (3 & 4) categories.
