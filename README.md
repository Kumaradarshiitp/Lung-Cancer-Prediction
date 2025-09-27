# Lung-Cancer-Prediction
Lung cancer prediction using 10 machine learning classification models with the Scikit-learn library in Python is a method for predicting the risk of lung cancer in patients based on various health and lifestyle factors. This approach employs multiple classification algorithms to identify lung cancer by analyzing patient data.
# Lung Cancer Prediction Model
This project aims to predict the likelihood of a person having lung cancer based on various health and lifestyle factors. It uses a dataset of survey responses and applies several machine learning classification algorithms to build and evaluate predictive models.

Dataset
The model uses a dataset named survey lung cancer.csv, which contains various attributes such as age, gender, smoking habits, and other symptoms like coughing, fatigue, and chest pain. The target variable is LUNG_CANCER, indicating a positive or negative diagnosis.

Methodology
The machine learning pipeline involves the following key steps:

Data Preprocessing: The raw data is cleaned and prepared for modeling.

Handling Duplicates: Duplicate rows are removed to ensure data integrity.

Encoding Categorical Data: All categorical features, including GENDER, SMOKING, ANXIETY, and others, are converted into numerical format using LabelEncoder. This is a necessary step for most machine learning algorithms.

Exploratory Data Analysis (EDA): The distribution of the target variable (LUNG_CANCER) is analyzed, and the relationship between various features and the target is visualized through bar plots.

Feature Engineering: A new feature, ANXYELFIN, is created by multiplying ANXIETY and YELLOW_FINGERS to potentially capture a combined effect of these two variables.

Handling Class Imbalance: The dataset is imbalanced (there are many more instances of one class than the other). To address this, the ADASYN (Adaptive Synthetic Sampling) technique is used to oversample the minority class, ensuring the model doesn't get biased towards the majority class.

Model Training and Evaluation: The balanced dataset is split into training and testing sets. Multiple machine learning models are trained and their performance is evaluated using classification reports (which include precision, recall, and F1-score) and K-Fold cross-validation to get a more robust estimate of their performance.

Models Used
The following classification models were implemented and compared in this project:

Logistic Regression

Decision Tree Classifier

K-Nearest Neighbors (KNN)

Gaussian Naive Bayes

Multinomial Naive Bayes

Support Vector Classifier (SVC)

Random Forest Classifier

XGBoost Classifier

Multi-layer Perceptron (MLP)

Gradient Boosting Classifier

Performance
The code evaluates each model's accuracy on the test set and through cross-validation. The results from the cross-validation provide a more reliable measure of a model's performance on unseen data. The final output displays the average accuracy score for each model.

How to Run
To run this project, you will need to:

1.Place the survey lung cancer.csv file in the same directory as the script.

2.Ensure you have all the necessary Python libraries installed, including pandas, numpy, matplotlib, seaborn, scikit-learn, imbalanced-learn, and xgboost.

3.Run the Python script.

