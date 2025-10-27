# IMDB Movie Review Sentiment Analysis

A comprehensive Natural Language Processing (NLP) project that classifies IMDB movie reviews as positive or negative using various Machine Learning algorithms.

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.0%2B-orange)
![NLTK](https://img.shields.io/badge/NLTK-Latest-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

## 📋 Project Overview

This project implements a complete NLP pipeline for sentiment analysis on IMDB movie reviews. The system processes raw text data, applies various preprocessing techniques, and trains multiple Naive Bayes classifiers to predict review sentiment with over 81% accuracy.

## 🚀 Features

- **End-to-End NLP Pipeline**: Data cleaning, text preprocessing, feature engineering, model training, and evaluation
- **Multiple Algorithms**: Comparison of GaussianNB, MultinomialNB, and BernoulliNB
- **Comprehensive Text Preprocessing**:
  - HTML tag removal
  - Lowercasing and special character removal
  - Stopword removal and stemming
  - Bag-of-Words vectorization
- **Model Evaluation**: Accuracy scores and performance comparison

## 📊 Results

| Model | Accuracy |
|-------|----------|
| Multinomial Naive Bayes | 81.5% |
| Bernoulli Naive Bayes | 77.75% |
| Gaussian Naive Bayes | 76.5% |

*Multinomial Naive Bayes achieved the best performance with 81.5% accuracy.*

## 🛠️ Installation

### Prerequisites
- Python 3.7+
- pip package manager




