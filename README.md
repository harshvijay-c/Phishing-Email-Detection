# Phishing Email Detection using Machine Learning

An end-to-end machine learning project for detecting phishing emails using Natural Language Processing (NLP), feature engineering, classical machine learning algorithms, and neural network based approaches.

The project focuses on analyzing email metadata and textual content to classify emails as legitimate or phishing.

---

## Project Overview

Phishing emails are one of the most common cybersecurity threats, where attackers attempt to obtain sensitive information by impersonating trustworthy sources.

This project builds and compares multiple machine learning models for phishing email classification using:

- Email subject and body text
- Sender and receiver information
- URL presence indicators
- Engineered textual and metadata features

---

## Dataset

The dataset contains labelled emails with the following features:

| Feature | Description |
|---|---|
| Sender | Sender email address |
| Receiver | Receiver email address |
| Date | Email timestamp |
| Subject | Email subject line |
| Body | Email content |
| URL | Indicates presence of URLs |
| Label | Phishing or legitimate email |

---

## Machine Learning Pipeline

The overall workflow:

```
Dataset
   |
   v
Exploratory Data Analysis
   |
   v
Text Cleaning & Preprocessing
   |
   v
Feature Engineering
   |
   v
TF-IDF Vectorization
   |
   v
Model Training
   |
   v
Evaluation
```

---

## Text Preprocessing

The email subject and body were cleaned using:

- Lowercasing
- HTML tag removal
- URL removal
- Punctuation cleaning
- Stopword removal
- Lemmatization

The cleaned subject and body text were combined and transformed into numerical representations using TF-IDF vectorization.

---

## Feature Engineering

Additional features were extracted from emails, including:

- Subject length
- Body length
- Number of special characters
- Uppercase word patterns
- URL presence
- Sender-based features
- Date/time-based features

These features were combined with TF-IDF representations for model training.

---

## Models Implemented

### Classical Machine Learning Models

The following models were trained and compared:

- Logistic Regression
- Support Vector Machine (SVM)
- Multinomial Naive Bayes
- Random Forest Classifier
- XGBoost Classifier

Techniques used:

- Train-test split
- Cross-validation
- Hyperparameter tuning
- Model comparison

---

## Neural Network Approach

A basic Artificial Neural Network (ANN) / Multi-Layer Perceptron (MLP) classifier was implemented using PyTorch.

The neural model was trained using vectorized email representations and compared with traditional machine learning models.

---

## Evaluation Metrics

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC score
- Confusion Matrix

Since phishing detection is a security-sensitive problem, emphasis was placed on reducing false negatives and improving recall.

---

## Repository Structure

```
Phishing-Email-Detection/

├── data/
│   └── Dataset files

├── notebooks/
│   ├── Classical ML experiments
│   └── Neural network experiments

├── results/
│   ├── Model performance results
│   └── Evaluation plots

├── README.md
└── requirements.txt
```

---

## Technologies Used

- Python
- NumPy
- Pandas
- Scikit-Learn
- XGBoost
- PyTorch
- NLTK
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Future Improvements

Planned extensions:

- Implement recurrent neural networks (LSTM/BiLSTM)
- Experiment with transformer-based models such as BERT
- Improve feature extraction from email metadata
- Deploy the classifier as a web application/API
- Add explainability techniques for model interpretation

---

## Results

Model comparison:

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---|---|---|---|
| Logistic Regression | - | - | - | - |
| SVM | - | - | - | - |
| Naive Bayes | - | - | - | - |
| Random Forest | - | - | - | - |
| XGBoost | - | - | - | - |
| MLP | - | - | - | - |

(Results will be updated as experiments are refined.)

---

## Author

Developed as a machine learning project exploring NLP-based cybersecurity applications.
