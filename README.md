# Flu Vaccine Sentiment Analysis

A data science project that analyzes public sentiment toward influenza (flu) vaccines by combining data from multiple online sources and applying Natural Language Processing (NLP) and Machine Learning techniques.

---

## Overview

Public opinion plays an important role in vaccine acceptance and public health awareness. This project aims to analyze how people perceive flu vaccines by collecting and analyzing data from social media, news articles, and official medical reports.

Using sentiment analysis and machine learning, the project identifies whether public opinions are positive, neutral, or negative, providing valuable insights into vaccine discussions.

---

## Objectives

- Analyze public sentiment toward influenza vaccines.
- Compare opinions from different online sources.
- Perform exploratory data analysis (EDA) to identify trends and patterns.
- Build and compare multiple machine learning models for sentiment classification.
- Select the best-performing model using appropriate evaluation metrics.

---

## Data Sources

The project combines data from multiple publicly available sources:

- YouTube – User comments discussing flu vaccines.
- GNews – News articles related to influenza vaccines.
- OpenFDA – Official adverse event reports submitted to the FDA.

The secondary datasets were collected from Kaggle, including datasets associated with the Zindi Flu Vaccine Challenge, together with publicly available OpenFDA data.

---

## Data Preprocessing

The text data was cleaned and prepared using several NLP preprocessing techniques:

- Removing duplicate records
- Handling missing values
- Lowercasing text
- Removing URLs, punctuation, numbers, and special characters
- Removing stop words
- Lemmatization
- Text normalization
- TF-IDF Vectorization

---

## Exploratory Data Analysis

Several analyses were performed to better understand the datasets, including:

- Sentiment distribution
- Word frequency analysis
- Word clouds
- Publication trends over time
- Source comparison
- Vaccine-related discussion patterns

---

## Machine Learning Models

Three supervised classification models were implemented:

- Logistic Regression (Baseline)
- Support Vector Machine (Linear SVM)
- Random Forest

Because the dataset was imbalanced, different balancing techniques were explored:

- Oversampling
- Class weighting (`class_weight="balanced"`)

Oversampling did not improve performance, therefore class weighting was selected for the final models.

---

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Macro F1-score

Since the dataset is imbalanced, Macro F1-score was selected as the primary evaluation metric because it gives equal importance to all sentiment classes.

---

## Results

Among the evaluated models:

| Model | Performance |
|--------|-------------|
| Logistic Regression | Strong baseline |
| Support Vector Machine (SVM) | Best performing model |
| Random Forest | Lower overall performance |

The SVM model achieved the highest Macro F1-score and demonstrated the most balanced performance across the three sentiment classes.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- NLTK
- spaCy
- Matplotlib
- Seaborn
- Google Colab

---


## Team Members

This project was completed as part of a university Data Science course by a team of five students.

My contributions included:

- Preparing and cleaning datasets
- Building and evaluating the Support Vector Machine (SVM) model
- Experimenting with class balancing techniques
- Creating the project poster
- Contributing to the project report and presentation

---


