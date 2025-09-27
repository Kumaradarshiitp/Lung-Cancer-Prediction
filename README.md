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

Output:
 1.Lung cancer target distribution: https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/lung%20cancer%20target%20distribution.png
 
 2.Exploratory data analysis and feature-target relationship visualization :https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/%20exploratory%20data%20analysis%20and%20feature-target%20relationship%20visualization.png
 
 3.Pain is distributed with respect to lung cancer : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/%20pain%20is%20distributed%20with%20respect%20to%20lung%20cancer.png
 
 4.Peer pressure, as a psychosocial factor :https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/%20peer%20pressure%2C%20as%20a%20psychosocial%20factor.png
 
 5.Presence or absence of fatigue is distributed among lung cancer cases : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/%20presence%20or%20absence%20of%20fatigue%20is%20distributed%20among%20lung%20cancer%20cases.png
 
 6.Presence or absence of swallowing difficulty : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/%20presence%20or%20absence%20of%20swallowing%20difficulty.png
 
 7.Presence or absence of wheezing correlates with lung cancer cases : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/%20presence%20or%20absence%20of%20wheezing%20correlates%20with%20lung%20cancer%20cases%20.png
 
 8.This heatmap displays pairwise correlations between clinical features : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/This%20heatmap%20displays%20pairwise%20correlations%20between%20clinical%20features%20.png
 
 9.Alcohol consumption : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/alcohol%20consumption.png
 
 10.Chronic diseases and the likelihood of lung cancer : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/chronic%20diseases%20and%20the%20likelihood%20of%20lung%20cancer.png
 
 11.Correlation matrix, enabling identification : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/correlation%20matrix%2C%20enabling%20identification.png
 
 12.Lung cancer positivity (class 1) and negativity (class 0) : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/lung%20cancer%20positivity%20(class%201)%20and%20negativity%20(class%200).png
 
 13.Presence of yellow fingers (typically a sign of heavy smoking) : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/presence%20of%20yellow%20fingers%20(typically%20a%20sign%20of%20heavy%20smoking).png
 
 14.Presence or absence of allergy : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/presence%20or%20absence%20of%20allergy%20.png
 
 15.Presence or absence of coughing aligns with lung cancer diagnosis : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/presence%20or%20absence%20of%20coughing%20aligns%20with%20lung%20cancer%20diagnosis.png
 
 16.Presence or absence of smoking : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/presence%20or%20absence%20of%20smoking.png
 
 17.Shortness of breath, a key respiratory symptom : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/shortness%20of%20breath%2C%20a%20key%20respiratory%20symptom.png
 
 18.The presence of anxiety, a psychological factor : https://github.com/Kumaradarshiitp/Lung-Cancer-Prediction/blob/main/the%20presence%20of%20anxiety%2C%20a%20psychological%20factor.png
 

