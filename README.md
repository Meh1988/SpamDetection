# SpamDetection
SMS Spam Classification: A machine learning project to classify SMS messages as "ham" (legitimate) or "spam" using natural language processing techniques. The project includes data preprocessing, model training, and evaluation with provided datasets.


This repository contains code for a natural language processing (NLP) and machine learning project aimed at classifying SMS messages as either "ham" (legitimate) or "spam." The task involves building a machine learning model using provided datasets and applying it to classify new messages.

Datasets
The project uses two datasets in CSV format:

train_data.csv: Contains 5,317 SMS messages with labels ("ham" or "spam") for training the model.
test_data.csv: Contains 1,410 SMS messages without labels for testing the model's performance.

Overview
The script performs the following steps:

Loads the training and test datasets.
Preprocesses the data.
Trains multiple classifiers on the training data.
Evaluates and visualizes the performance of each classifier.
Creates an ensemble classifier using a voting strategy and evaluates its performance.
Libraries Used
pandas: For data manipulation and analysis.
numpy: For numerical operations.
matplotlib and seaborn: For data visualization.
sklearn: For machine learning models and metrics.
shap: For interpreting the models (though not used explicitly in this script).

Results

Individual Classifiers: The script evaluates the following classifiers:
Naive Bayes
Logistic Regression
Support Vector Machine (SVM)
Random Forest
Gradient Boosting
Ensemble Model: A Voting Classifier is created combining all individual classifiers. The predictions from this ensemble model are saved in test_labels.csv.

Evaluation Metrics: For each classifier, the script provides:
Accuracy
Classification Report
Confusion Matrix (visualized using seaborn)


Output
Confusion Matrices: Plotted for each classifier to visualize performance on training data.
test_labels.csv: Contains predictions from the ensemble classifier.
