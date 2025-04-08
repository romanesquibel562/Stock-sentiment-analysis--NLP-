# Stock-sentiment-analysis--NLP-
NLP + Financial Modeling: Forecasting stock price using news sentiment (VADER + Loughran-McDonald), Ridge Regression, and Logistic Classification.

This project combines Natural Language Processing (NLP), sentiment analysis, and machine learning to forecast NVDA stock price movements using real-time financial news data. It integrates sentiment signals derived from financial headlines with historical market data to predict both price levels and directional changes.

Using data from the NewsAPI and Yahoo Finance, this pipeline applies the VADER sentiment model and adjusts sentiment using the Loughran-McDonald financial lexicon. It then feeds sentiment scores, technical indicators, and lag features into multiple machine learning models—including Ridge Regression and Logistic Regression—to evaluate their ability to predict stock movements.

---

## Project Overview

The pipeline includes:
- Fetching NVDA-related news articles using NewsAPI
- Extracting and preprocessing news titles using NLTK (tokenization, stopwords, punctuation removal)
- Calculating sentiment using:
  - VADER sentiment analyzer
  - Adjustments with the Loughran-McDonald Financial Sentiment Dictionary
- Fetching NVDA historical stock price data from Yahoo Finance
- Merging sentiment and stock data by date
- Engineering features including:
  - Lagged sentiment
  - 7-day moving average
  - Normalized price indicators
- Training and evaluating two types of models:
  - **Ridge Regression** (for price forecasting)
  - **Logistic Regression** (for movement classification)

---

## Features

- NLP-based sentiment scoring with financial context
- Real-time data integration from two APIs
- Support for both regression and classification models
- Custom sentiment adjustment based on financial sentiment dictionaries
- Feature engineering for predictive modeling (lagging, moving averages)
- Evaluation with RMSE, classification accuracy, and cross-validation
- Visualization of actual vs predicted stock prices

---

## Installation Instructions

Make sure Python 3.8+ and `pip` are installed, then run:

bash
pip install -r requirements.txt

## Run this project

python stock_sentiment_pipeline.py

Make sure your .env file contains your NewsAPI key:

NEWS_API_KEY=your_api_key_here

## Model Evaluation
Ridge Regression:

R-squared (R²) Score

RMSE

Feature importance using RFE (Recursive Feature Elimination)

Logistic Regression:

Classification accuracy

Precision, recall, F1-score

Directional movement prediction (up/down)

## Use Cases & Extensions
Real-time trading signal generation

Integration with technical indicators for hybrid forecasting models

Expansion to multi-stock or sector-level sentiment forecasting

Enhancement with deep learning models (e.g., LSTM, Transformers)

Streamlit dashboard for interactive model output

## Author
Roman Esquibel

Data Analyst | Financial Modeler | Machine Learning Practitioner


LinkedIn: https://www.linkedin.com/in/roman-esquibel-75b994223/

