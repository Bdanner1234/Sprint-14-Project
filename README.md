--Project Overview

This project analyzes movie reviews to predict whether a review expresses a positive or negative sentiment.
Using Natural Language Processing (NLP) and machine learning, the goal was to build a model capable of classifying sentiment automatically based on the text content of reviews.
This work was completed as part of the TripleTen Data Science Program.

--Data Description

The dataset consists of thousands of movie reviews labeled as positive or negative.
Each review is a line of free text that expresses an opinion about a film.

--Key columns include:
review — the movie review text
pos — the target variable (1 = positive, 0 = negative)

--Project Steps

Data Preprocessing
Removed HTML tags and punctuation.
Lowercased all text and tokenized it.
Removed stopwords using nltk and spaCy.
Applied lemmatization for word normalization.

--Feature Engineering

Transformed text using TF–IDF Vectorization to capture word importance.

--Model Training

Trained several classifiers:
Logistic Regression
Random Forest Classifier
LightGBM Classifier
Tuned hyperparameters using cross-validation.

--Evaluation

Measured model performance using:
Accuracy
Precision
Recall

F1-score (target ≥ 0.85)

--Results
Best Model: Logistic Regression with TF–IDF features

F1-score: ~0.88 (met and exceeded target)

The model successfully distinguishes between positive and negative reviews.

Business Value:
This model could be integrated into a review monitoring system to automatically flag negative customer sentiment for analysis and response.
