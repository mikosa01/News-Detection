## Fake News Detection

This project aims to build a machine learning model to detect fake news using logistic regression. The Jupyter notebook contains all steps to preprocess the data, train the model, and evaluate its performance.

# Table of Contents
1. Installation
2. Usage
3. Project Structure
4. Data Preprocessing
5. Model Training
6. Evaluation
7. Results
8. License

# Installation
To run this notebook, you need to have Python installed along with the following libraries:

`pip install nltk pandas numpy matplotlib scikit-learn seaborn jupyter`

# Usage
Clone this repository.
Place your true.csv and fake.csv files in the data directory.
Open the Jupyter notebook fake_news_detection.ipynb and run the cells sequentially.

# Project Structure

├── data
│   ├── true.csv
│   ├── fake.csv
├── README.md
└── fake_news_detection.ipynb

# Data Preprocessing

Loading Data:
The data is loaded from true.csv and fake.csv files.
Combining Data:

A new column 'target' is added to both DataFrames (true and fake).
The DataFrames are concatenated into a single DataFrame df.
Cleaning Data:

Unnecessary columns ('date', 'title', 'subject') are dropped.
The text data is preprocessed by removing special characters, stopwords, and converting to lowercase.
Splitting Data:

The data is split into training (65%), validation (30%), and test (5%) sets.
Vectorizing Text:

The text data is converted into a document-term matrix using CountVectorizer.

Encoding Labels:
Labels are encoded into numerical format using LabelEncoder.

# Model Training
The logistic regression model is trained on the training data.

# Evaluation
Predictions are made on the validation set.
The model's performance is evaluated using accuracy, F1 score, and ROC curve.

# Results
The top words and labels in the dataset are identified.
The logistic regression model's confusion matrix is visualized using a heatmap.


# License
This project is licensed under the MIT License.

