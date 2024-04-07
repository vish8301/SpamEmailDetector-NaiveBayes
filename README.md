# Spam eMail Detection using Naive Bayes Classification Algorithm

This project implements a Spam Email Classifier using the Naive Bayes supervised machine learning algorithm. <br>
The classifier is trained and tested on a dataset of emails, which are labeled as either 'Spam' or 'Not Spam'.


## Library Imports
The project uses the following Python libraries

- `os`
- `numpy`
- `collections.Counter`
- `sklearn` (for the Naive Bayes algorithm and accuracy metrics).

To install the sklearn library, run the following command:
```bash
pip install scikit-learn
```


## Methodology and Code Descriptions

**Function: make_Dictionary**

- This function processes a collection of emails to create a list of the 3000 most common words, excluding non-alphabetical words and single characters, which serves as the feature set for spam email classification.

**Function: extract_features**

- This function reads emails from the specified directory and extracts features for use in a spam classifier. It creates a feature matrix based on the frequency of the most common words (as per the provided dictionary) in each email. It also assigns labels to the emails, marking them as spam or not spam based on their filenames. The feature matrix and the labels are used for training and evaluating the machine learning model.

**Training and Testing the Classifier**

- The Naive Bayes classifier is trained using the extracted features and labels from the training dataset. It is then tested on a separate test dataset to evaluate its accuracy in classifying emails as spam or not spam.


## Results
The project includes a comprehensive analysis of the model's performance, including accuracy metrics and confusion matrices. These results provide insights into the model's ability to generalize and correctly identify spam emails, thereby showcasing the effectiveness of the chosen machine learning algorithm and methodologies.
