About the project:

This project aims to provide a simple yet effective spam email classification system using machine learning techniques deployed via a Flask web application. The system allows users to input email content, and the application returns a classification result indicating whether the email is spam or not spam.



FEATURES :
Machine Learning Model: Utilizes a trained machine learning model to classify emails based on their content and 
Flask Web Application provides a user-friendly interface for interacting with the classification system.



Pre-requisites:
Python 3.x,
Flask,
Scikit-learn (for machine learning model) and 
Other dependencies listed in requirements.txt



Usage:
1. Train the machine learning model using your dataset (not provided in this repository).

2. Save the trained model as a '.pkl' file and save it in 'models'

3. Run the Flask application (python run.py)

4. Access the application in your web browser at http://localhost:5000.



Acknowledgement:
This project was inspired by the need for a practical application of machine learning in spam email detection.

Thanks to the Flask and Scikit-learn communities for their valuable contributions.

Training Method and Algorithm:

Training Method: The training method used in your program is supervised learning. This means that the algorithm learns from labeled data, where each email is labeled as either spam (1) or not spam (-1).

Algorithm: You used the Multinomial Naive Bayes algorithm for classification. Naive Bayes is a probabilistic classifier based on Bayes' theorem with the "naive" assumption of feature independence.
Dataset:

Source: The dataset used is loaded from a CSV file named "emails.csv".

Size: After preprocessing, the dataset contains 5694 email samples.

Features: The dataset consists of a single feature "text", which contains the text content of the emails.

Target Variable: The target variable is "spam", indicating whether an email is spam (1) or not spam (-1).

Training-Testing Split:

Method: The dataset is split into training and testing sets using the train_test_split function from scikit-learn.

Split Ratio: The data is split with 80% for training and 20% for testing.

Training Accuracy:

After training the Multinomial Naive Bayes classifier on the training data, you evaluated its performance on the testing data.
The accuracy achieved on the testing data is approximately 98.68%.

