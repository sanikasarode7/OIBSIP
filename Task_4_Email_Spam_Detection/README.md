# Email Spam Detection with Machine Learning

## Overview

This project develops a machine learning classification system to distinguish spam messages from legitimate (ham) messages using Natural Language Processing (NLP) techniques.

## Objective

To build and evaluate machine learning models that can classify SMS messages as either spam or ham.

## Dataset

The dataset contains SMS messages labeled as:
- Spam
- Ham

The dataset was cleaned by retaining the relevant message and label columns and removing duplicate records.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- WordCloud
- Jupyter Notebook

## Methodology

### 1. Data Loading and Cleaning

- Loaded the SMS spam dataset.
- Checked the dataset structure and missing values.
- Checked duplicate records.
- Retained the relevant label and message columns.
- Removed duplicate records.

### 2. Class Distribution

Analyzed the number and percentage of spam and ham messages to understand the class distribution in the dataset.

### 3. Text Preprocessing

The SMS messages were preprocessed using:
- Lowercase conversion
- Punctuation removal
- Stopword removal

### 4. TF-IDF Feature Extraction

TF-IDF (Term Frequency-Inverse Document Frequency) was used to convert text messages into numerical features suitable for machine learning.

It gives higher importance to words that are useful within a message while reducing the importance of words that occur frequently across the complete collection of messages.

### 5. Train-Test Split

The dataset was divided into training and testing sets using an 80:20 split with stratification to maintain the class distribution.

### 6. Machine Learning Models

Two classification models were developed:

- Multinomial Naive Bayes
- Logistic Regression

### 7. Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 8. Recall Analysis

Recall was discussed specifically for spam detection because false negatives represent spam messages incorrectly classified as ham.

### 9. Bonus Visualization

WordCloud visualizations were created separately for spam and ham messages to show frequently occurring words in each category.

## Project Structure

Task_4_Email_Spam_Detection/
├── Email_Spam_Detection.ipynb
├── spam.csv
└── README.md

## Conclusion

This project demonstrates an end-to-end NLP and machine learning workflow for SMS spam detection, including data cleaning, text preprocessing, TF-IDF feature extraction, classification, model evaluation, and visualization.
